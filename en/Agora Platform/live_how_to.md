
---
title: Interactive Broadcast-related Issues
description: 
platform: Live Broadcast-related Issues
updatedAt: Thu Nov 22 2018 09:14:10 GMT+0000 (UTC)
---
# Interactive Broadcast-related Issues
### How do you ban a user in a live broadcast?
You can ban a user from the server. See [Dashboard RESTful API](http://https://docs.agora.io/en/Interactive%20Broadcast/dashboard_restful_live?platform=All_Platforms).

### How do you adjust the layout of a CDN live broadcast?
Call the `setLiveTranscoding` method.

### Why is there a 30-second freeze when I stop recording a stream?
To prevent the RTMP stream from being interrupted when the host is disconnected or temporarily offline, the recording service allocates 30 seconds for static data. Therefore, the recording lasts for 30 seconds after the hosts leave the channel.

### Why do I encounter cross-domain issues when I use the test CDN address?
This issue occurs because the test address is used in a test environment and cross.xml is not configured on the CDN.

### Can a host create a live broadcast consisting of two video streams in the same room at the same time?
Yes, you can do this with the following methods:
* The app captures the videos of the screen and the host, mixes and encodes them, and sends the data to the Agora SDK. Do not use the screenshot output stream of the SDK because it may affect efficiency. Agora provides technical support for PC screen capture.
* A host can join the room as a guest host and start a live broadcast in a smaller window on a mobile phone while staying in the live broadcast on the PC. The application on the PC adds the live broadcast of the guest host to the live broadcast of the PC.
