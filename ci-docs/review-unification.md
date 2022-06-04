---
title: 審查資料整合
description: 審查資料整合步驟、建立整合客戶個人資料，以及審查結果
ms.date: 05/04/2022
ms.subservice: audience-insights
ms.topic: tutorial
author: v-wendysmith
ms.author: adkuppa
ms.reviewer: v-wendysmith
manager: shellyha
searchScope:
- ci-match
- ci-merge
- ci-relationships
- customerInsights
ms.openlocfilehash: 4c709dfb55bf079dd2fe99e41adb4c77c2bece4b
ms.sourcegitcommit: 6a5f4312a2bb808c40830863f26620daf65b921d
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 05/11/2022
ms.locfileid: "8741740"
---
# <a name="review-data-unification"></a>審查資料整合

[!INCLUDE [m3-prod-trial-note](includes/m3-prod-trial-note.md)]

整合程序的最後一個步驟會顯示程序中的步驟摘要，並在建立整合個人資料前提供變更的機會。

:::image type="content" source="media/m3_review.png" alt-text="螢幕擷取畫面：審查和建立客戶個人資料。":::

## <a name="review-the-data-unification-steps"></a>審查資料整合步驟

1. 若要查看並進行任何變更，請在任一資料整合步驟上選取 **編輯**。

1. 如果您對選取項目滿意，請選取 **建立客戶個人資料**。 建立整合客戶個人資料時，就會顯示 **整合** 頁面。 整合演算法需要一段時間才能完成，而且在完成前您無法變更設定。

   [!INCLUDE [m3-task-details-include](includes/m3-task-details.md)]

當整合程序完成時，整合客戶個人資料實體 (稱為 *customer*) 會列在 **實體** 頁面的 **個人資料** 區段。 第一次成功的整合執行會建立整合的 *Customer* 實體。 所有後續的執行都會展開該實體。

## <a name="review-the-results-of-data-unification"></a>審查資料整合結果

在整合後，**資料** > **整合** 頁面會顯示整合客戶個人資料的數量。 整合程序中的每個步驟的結果都會顯示在各個磚上。 例如，**來源欄位** 會顯示已對應屬性 (欄位) 數量以及 **重複記錄** 會顯示找到的重複記錄數量。

:::image type="content" source="media/m3_unified.png" alt-text="資料整合後，資料整合頁面的螢幕擷取畫面。":::

> [!TIP]
> 只有在選取多個實體時，才會顯示 **比對條件** 磚。

我們建議您審查結果，尤其是[比對規則](data-unification-update.md#manage-match-rules)品質，並且依需求加以修正。

如有需要，[請變更整合設定](data-unification-update.md)，然後重新執行整合個人資料。

## <a name="next-step"></a>後續步驟

設定 [活動](activities.md)、[擴充](enrichment-hub.md)、[關聯性](relationships.md)或 [量值](measures.md)，以取得更多客戶見解。

[!INCLUDE[footer-include](includes/footer-banner.md)]