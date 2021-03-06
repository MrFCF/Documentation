
---
title: Integrate the SDK
description: 
platform: Windows
updatedAt: Mon Dec 31 2018 21:53:16 GMT+0000 (UTC)
---
# Integrate the SDK
## Prerequisites

-   OS: Microsoft Windows 7+

-   Compiler: Microsoft Visual C++ 2013+

-   Development environment: Microsoft Visual Studio 2013 (Recommended)


> If you use Microsoft Visual Studio 2013+, you may encounter compatibility issues.

## Create an Agora Account and Get an App ID

1. Sign up for a developer account at [https://dashboard.agora.io/](https://dashboard.agora.io/).

2. Click **Add New Project** on the **Projects** page in [Dashboard](https://dashboard.agora.io/).

   <img alt="../_images/appid_1.jpg" src="https://web-cdn.agora.io/docs-files/en/appid_1.jpg" />

3. Fill in the **Project Name** and click **Submit**. You have created your first project at Agora.

4. Find the **App ID** under the created project.

   <img alt="../_images/appid_2.jpg" src="https://web-cdn.agora.io/docs-files/en/appid_2.jpg" />


## Add the Agora SDK to Your Project

1.  Download the [Windows SDK](https://docs.agora.io/en/Agora%20Platform/downloads), and unzip it.
2.  Add the `sdk/include` folder to the INCLUDE directory of your project.
3.  Add the `sdk/lib` folder to the LIB directory of your project, and ensure that agora_rtc_sdk.lib is linked to your project.
4.  Copy all *dll* files under `sdk/dll`  to the directory of your executable file.

## Next Steps
You have set up the Windows development environment and can start a call/live broadcast following the steps under **Quickstart Guide**:
- Initialize the SDK
- Join a Channel
- Publish and Subscribe to Streams



