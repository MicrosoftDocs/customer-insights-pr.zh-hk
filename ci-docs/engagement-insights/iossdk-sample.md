---
title: 執行 iOS SDK 範例
description: 用專案範例了解 iOS SDK
author: britl
ms.reviewer: mhart
ms.author: britl
ms.date: 06/23/2021
ms.service: customer-insights
ms.subservice: engagement-insights
ms.topic: conceptual
ms.manager: shellyha
ms.openlocfilehash: 053e626d06d3e17b39b448987410058e45e8ae0385f3ecdef40314cb46ae4bf4
ms.sourcegitcommit: aa0cfbf6240a9f560e3131bdec63e051a8786dd4
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 08/10/2021
ms.locfileid: "7036855"
---
# <a name="run-the-ios-sdk-sample"></a>執行 iOS SDK 範例

[!INCLUDE [cc-beta-prerelease-disclaimer](includes/cc-beta-prerelease-disclaimer.md)]

此範例 iOS 專案可協助您了解 SDK 在應用程式中的運作方式。 您不需要撰寫程式碼。 只要新增您的擷取金鑰，您就可以立即查看工作區中的事件。

## <a name="prerequisites"></a>先決條件

- [Xcode 版本 9+](https://developer.apple.com/xcode/downloads/)
- [擷取金鑰](get-started-ios.md)

## <a name="download-the-ios-sdk-sample"></a>下載 iOS SDK 範例

1. [下載參與度見解 iOS SDK 範例](https://download.pi.dynamics.com/sdk/EI-SDKs/ei-ios-sample.zip)。
1. 解壓縮 `ei-ios-sample.zip` 檔案。
1. 在 Xcode 中打開範例應用程式專案。
1. 在 `EIConfig.plist` 檔案中，將欄位 `ingestionKey` 中的字串 `“YOUR-INGESTION-KEY”` 替換為參與度見解底下 **系統管理** > **工作區** > **安裝指南** 中的工作區擷取金鑰。
1. 若要開始範例專案，請選取 **執行**。
1. 查看工作區中的事件。

[!INCLUDE[footer-include](../includes/footer-banner.md)]
