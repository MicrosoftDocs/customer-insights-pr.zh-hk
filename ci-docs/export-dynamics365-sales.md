---
title: 將客戶細分匯出至 Dynamics 365 Sales (預覽版)
description: 了解如何設定連接並匯出至 Dynamics 365 Sales。
ms.date: 07/25/2022
ms.reviewer: mhart
ms.subservice: audience-insights
ms.topic: how-to
author: pkieffer
ms.author: philk
manager: shellyha
searchScope:
- ci-export
- customerInsights
ms.openlocfilehash: c3497f4625cada49ae33c6987e58994a15536f9b
ms.sourcegitcommit: 594081c82ca385f7143b3416378533aaf2d6d0d3
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 07/27/2022
ms.locfileid: "9196008"
---
# <a name="export-segments-to-dynamics-365-sales-preview"></a>將客戶細分匯出至 Dynamics 365 Sales (預覽版)

使用您的客戶資料來建立行銷名單、追蹤工作流程，並透過 Dynamics 365 Sales 寄出促銷活動。

## <a name="prerequisites"></a>先決條件

連絡人記錄必須存在於Dynamics 365 Sales 中，才能將客戶細分從 Customer Insights 匯出至 Sales。 了解如何在 [Dynamics 365 Sales 中使用 Microsoft Dataverse](connect-dataverse-managed-lake.md) 擷取連絡人。

   > [!NOTE]
   > 將客戶細分從 Customer Insights 匯出至 Sales，並不會在 Sales 執行個體中建立新的連絡人記錄。 從 Sales 中的連絡人記錄必須擷取到 Customer Insights，並用作資料來源。 他們也必須包含整合客戶實體中，才能客戶細分匯出前，先將客戶識別碼對應至連絡人的識別碼。

## <a name="known-limitations"></a>已知限制

匯出到 Dynamics 365 Sales 的每個客戶細分限制為 100,000 個，最多可能需要 3 小時才能完成。

## <a name="set-up-connection-to-sales"></a>設定與 Sales 的連線

[!INCLUDE [export-connection-include](includes/export-connection-admn.md)]

1. 移至 **管理** > **連接**。

1. 選取 **新增連接**，然後選擇 **Dynamics 365 Sales**。

1. 在 **顯示名稱** 中，給連接一個能夠辨識的名稱。 連接的名稱與類型能說明此連接。 我們建議您選取可以說明此連接用途和目標的名稱。

1. 選擇可使用此連接的人員。 根據預設，只有系統管理員。 如需詳細資訊，請參閱[允許參與者使用匯出的連接](connections.md#allow-contributors-to-use-a-connection-for-exports)。

1. 在 **伺服器位址** 欄位中輸入組織的 Sales URL。

1. 在 **伺服器管理帳戶** 區段中，選取 **登入**，然後選擇 Dynamics 365 Sales 帳戶。

1. 將客戶識別碼欄位對應到 Dynamics 365 連絡人識別碼。

1. 請檢查 [資料隱私權和合規性](connections.md#data-privacy-and-compliance)，並選取 **我同意**。

1. 選取 **儲存** 來完成連接。

## <a name="configure-an-export"></a>設定匯出

[!INCLUDE [export-permission-include](includes/export-permission.md)]

1. 移至 **資料** > **匯出**。

1. 選取 **新增匯出**。

1. 在 **匯出的連結** 欄位中，在 Dynamics 365 Sales 區段中選擇連接。 如果沒有可用的連接，請與系統管理員聯繫。

1. 輸入匯出的名稱。

1. 在與 Dynamics 365 連絡人識別碼相符的客戶實體中選擇 [連絡人識別碼] 欄位。

1. 選取您要匯出的客戶細分。

1. 選取 **儲存**

[!INCLUDE [export-saving-include](includes/export-saving.md)]

[!INCLUDE [footer-include](includes/footer-banner.md)]
