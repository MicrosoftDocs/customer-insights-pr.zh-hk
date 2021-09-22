---
title: Android SDK 範例
description: 用專案範例了解 Android SDK
author: britl
ms.reviewer: m-hartmann
ms.author: britl
ms.date: 06/23/2021
ms.service: customer-insights
ms.subservice: engagement-insights
ms.topic: conceptual
ms.manager: shellyha
ms.openlocfilehash: ba51961bc7f9555d7dba5b6a21c8636011438d75cba87bc132b896841c467a33
ms.sourcegitcommit: aa0cfbf6240a9f560e3131bdec63e051a8786dd4
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 08/10/2021
ms.locfileid: "7035853"
---
# <a name="run-the-android-sdk-sample"></a>執行 Android SDK 範例

[!INCLUDE [cc-beta-prerelease-disclaimer](includes/cc-beta-prerelease-disclaimer.md)]

此範例 Android 專案可協助您了解 SDK 在應用程式中的運作方式。 您不需要撰寫程式碼。 只要新增您的擷取金鑰，您就可以立即查看工作區中的事件。

## <a name="prerequisites"></a>先決條件

- [Android Studio](https://developer.android.com/studio)
- [擷取金鑰](get-started-android.md)

## <a name="download-the-android-sdk-sample"></a>下載 Android SDK 範例

1. [下載參與度見解 Android SDK 範例](https://download.pi.dynamics.com/sdk/EI-SDKs/ei-android-sample.zip)。
1. 解壓縮 `ei-android-sample.zip` 檔案。
1. 在 Android Studio 打開解壓縮後的資料夾 。
1. 在 `AndroidManifest.xml` 檔案中，將字串 `"Your-Ingestion-Key"` 替換為參與度見解底下 **系統管理** > **工作區** > **安裝指南** 中的工作區擷取金鑰。 

   > [!NOTE]
   > 您不需要更換 `${applicationId}`區段。 它應該自動填入。

   ```xml
   <application>
   ...
       <provider
           android:authorities="${applicationId}.com.microsoft.engagementinsights.eiandroidsdk.AnalyticsContentProvider"
           android:name="microsoft.dynamics.engagementinsights.eiandroidsdk.AnalyticsContentProvider" />
       <meta-data
           android:name="com.microsoft.engagementinsights.ingestionKey"
           android:value="Your-Ingestion-Key" />
       <meta-data
           android:name="com.microsoft.engagementinsights.autoCapture"
           android:value="true" />
   ...
   </application>
   ```

1. 若要開始範例專案，請選取 **執行**。
1. 查看工作區中的事件。


[!INCLUDE[footer-include](../includes/footer-banner.md)]
