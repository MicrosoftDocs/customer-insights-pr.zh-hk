---
title: Customer Insights 中的實體
description: 在實體頁面上檢視資料。
ms.date: 08/04/2022
ms.reviewer: mhart
ms.subservice: audience-insights
ms.topic: conceptual
author: mukeshpo
ms.author: mukeshpo
manager: shellyha
searchScope:
- ci-entities
- customerInsight
ms.openlocfilehash: e365945b27e7c985ca5371c6b72619610b6f3af1
ms.sourcegitcommit: be341cb69329e507f527409ac4636c18742777d2
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 09/30/2022
ms.locfileid: "9610125"
---
# <a name="entities-in-customer-insights"></a>Customer Insights 中的實體

[設定資料來源](data-sources.md)之後，請移至 **實體** 頁面，評估所擷取資料的品質。 實體被視為資料集。 Dynamics 365 Customer Insights 的多重功能圍繞這些實體組建。 仔細檢閱它們可協助您驗證這些功能的輸出。

當您在 Customer Insights 中增加資料或建立客戶細分、量值及活動時，從這些動作建立的實體會顯示在 **實體** 頁面上。

## <a name="view-a-list-of-entities"></a>檢視實體清單

移至 **資料** > **實體** 以查看實體清單。 下列是每個實體都會顯示的資訊。

- **名稱**：資料實體的名稱。 如果實體名稱旁邊出現警告符號，表示無法順利載入該實體的資料。
- **來源**：擷取到實體的資料來源類型。
- **更新**：實體上次更新的時間。
- **狀態**：實體上次更新的詳細資料。

## <a name="explore-a-specific-entitys-data"></a>探索特定實體的資料

1. 請前往 **資料** > **實體**。
1. 選取實體以開啟詳細資料頁面。  
1. 探索該實體中包含的不同欄位和記錄。

- **屬性** 索引標籤會預設為選取，並顯示所選實體詳細資料，例如欄位名稱、資料類型和類型。 **類型** 欄會顯示 Common Data Model 關聯的類型，它們是由系統自動識別或由使用者[手動對應](map-entities.md)。 這些類型是語義類型，且可以與屬性的資料類型不同。 例如，下列的 *電子郵件* 欄位包含 *字串* 資料類型，但是 (語義的) Common Data Model 類型可能是 *電子郵件*、*EmailAddress* 或 *Identity.Service.Email*。

   :::image type="content" source="media/data-manager-entities-fields.png" alt-text="欄位表格。":::

   > [!NOTE]
   > 此頁面只會顯示您實體資料的範例。 若要查看完整資料集，請移至 **資料來源** 頁面，選取實體，選取 **編輯**，然後使用 Power Query 編輯器查看此實體的資料（如[資料來源](data-sources.md)中所述）。

   若要進一步了解實體中擷取的資料，**摘要** 欄提供了一些重要的資料特徵，例如 null、遺失值、唯一值、計數和分佈（視何者適用於您的資料）。 選取圖表圖示以查看資料的摘要。

   :::image type="content" source="media/data-manager-entities-summary.png" alt-text="資料摘要表格。":::

- **資料** 索引標籤會顯示有關實體中個別記錄的詳細資料。 列出的詳細資料會依實體的資料類型而定。

   :::image type="content" source="media/data-manager-entities-data.png" alt-text="選取實體。":::

- **報表** 索引標籤 (在某些實體可用) 讓您可透過建立報表來實現資料的視覺化效果，並包含這些資料行：

  - **報表名稱**：報表的名稱。
  - **建立者**：建立實體的人員名稱。
  - **建立時間**：建立實體的日期與時間。
  - **編輯者**：修改實體的人員名稱。
  - **編輯時間**：修改實體的日期與時間。

[!INCLUDE [footer-include](includes/footer-banner.md)]
