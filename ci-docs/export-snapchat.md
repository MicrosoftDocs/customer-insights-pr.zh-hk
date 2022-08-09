---
title: 將客戶細分匯出至 Snapchat (預覽版)
description: 了解如何設定連接並匯出至 Snapchat。
ms.date: 07/25/2022
ms.reviewer: mhart
ms.subservice: audience-insights
ms.topic: conceptual
author: pkieffer
ms.author: philk
manager: shellyha
ms.openlocfilehash: 85443dcb54ebd58182997fbb56a738901f2a051f
ms.sourcegitcommit: 594081c82ca385f7143b3416378533aaf2d6d0d3
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 07/27/2022
ms.locfileid: "9195409"
---
# <a name="export-segments-to-snapchat-preview"></a>將客戶細分匯出至 Snapchat (預覽版)

將整合客戶個人資料的客戶細分匯出至 Snapchat，並用於廣告。

## <a name="prerequisites"></a>先決條件

- [Snapchat 商務帳號](https://business.snapchat.com/)、[Snapchat 廣告帳號](https://ads.snapchat.com/)以及對應的系統管理員認證。 您必須至少是組織帳戶的成員，以及指定 AD 帳戶的資料管理員。
- 在 Snapchat 對象管理者中，至少有一個類型為 SAM (Snap 對象對比) 的對象。
- [Snapchat 客戶細分/對象識別碼](https://businesshelp.snapchat.com/s/article/custom-audiences)。 在 Snapchat 觀眾管理者中選取對象之後，即可在 URL 中找到對象的識別碼。
- 在 Customer Insights 中的[已設定的客戶細分](segments.md)。
- 匯出區段的統一客戶設定檔包含代表電子郵件地址的欄位。

## <a name="known-limitations"></a>已知限制

- 多達 100 萬個客戶資料，最多可能需要 15 分鐘才能完成。
- 僅客戶細分。

## <a name="set-up-connection-to-snapchat"></a>設定與 Snapchat 的連接

[!INCLUDE [export-connection-include](includes/export-connection-admn.md)]

1. 移至 **管理** > **連接**。

1. 選取 **新增連接**，然後選擇 **Snapchat**。

1. 在 **顯示名稱** 中，給連接一個能夠辨識的名稱。 連接的名稱與類型能說明此連接。 我們建議您選取可以說明此連接用途和目標的名稱。

1. 選擇可使用此連接的人員。 根據預設，只有系統管理員。 如需詳細資訊，請參閱[允許參與者使用匯出的連接](connections.md#allow-contributors-to-use-a-connection-for-exports)。

1. 請檢查 [資料隱私權和合規性](connections.md#data-privacy-and-compliance)，並選取 **我同意**。

1. 選取 **連接** 以初始化連接。

1. 選取 **與 Snapchat 驗證**，並提供系統管理員認證給 Snapchat。

1. 選取 **將您自己新增為匯出使用者** 並提供您的 Customer Insights 認證。

1. 選取 **儲存** 來完成連接。

## <a name="configure-an-export"></a>設定匯出

[!INCLUDE [export-permission-include](includes/export-permission.md)]

1. 移至 **資料** > **匯出**。

1. 選取 **新增匯出**。

1. 在 **匯出的連結** 欄位中，在 Snapchat 區段中選擇連接。 如果沒有可用的連接，請與系統管理員聯繫。

1. 輸入匯出的名稱。

1. 輸入 **Snapchat 客戶細分/對象識別碼**。

1. 請在 **資料相符** 分段的 **電子郵件** 欄位中選取代表客戶電子郵件地址的欄位。

1. 選取您要匯出的客戶細分。

1. 選取 **儲存**。

[!INCLUDE [export-saving-include](includes/export-saving.md)]

[!INCLUDE [footer-include](includes/footer-banner.md)]
