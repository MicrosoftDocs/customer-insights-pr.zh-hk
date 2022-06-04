---
title: 比對資料統整的實體
description: 比對實體以建立統整的客戶設定檔。
recommendations: false
ms.date: 05/05/2022
ms.subservice: audience-insights
ms.topic: tutorial
author: v-wendysmith
ms.author: mukeshpo
ms.reviewer: v-wendysmith
manager: shellyha
searchScope:
- ci-match
- ci-merge
- ci-map
- customerInsights
ms.openlocfilehash: bc470dd932c2c981adc5840bb52d60f8dfe0de61
ms.sourcegitcommit: 6a5f4312a2bb808c40830863f26620daf65b921d
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 05/11/2022
ms.locfileid: "8740976"
---
# <a name="match-conditions"></a>比對條件

[!INCLUDE [m3-prod-trial-note](includes/m3-prod-trial-note.md)]

整合中的這步驟，定義了實體間比對的比對順序與規則。 此步驟需要至少兩個實體。

> [!NOTE]
> 建立比對條件並選取 **下一步** 之後，就不能移除選定的實體或屬性。 如有需要，繼續之前請選取 **上一步** 以複查選定的實體和屬性。

## <a name="include-enriched-entities-preview"></a>包括已擴充的實體 (預覽版)

如果您在資料來源層級擴充實體來改善您的整合結果，請選取它們。 如需詳細資訊，請參閱[資料來源擴充](data-sources-enrichment.md)。 如果您在 **重複資料** 頁面上選取擴充實體，則不需要再次選取它們。

1. 在 **比對條件** 頁面上方，選取 **使用已擴充實體**。

1. 從使用 **已擴充的實體** 窗格中，選取一個或多個已擴充的實體。

1. 選取 **完成**。

## <a name="specify-the-match-order"></a>指定比對順序

每次比對將兩個或多個實體整合為一個合併實體。 同時，它會保留唯一的客戶記錄。 比對順序代表系統嘗試比對記錄的順序。

> [!IMPORTANT]
> 清單中的第一個實體稱為主要實體。 主要實體是整合個人資料的資料集基礎。 其他選定的實體將會新增至此實體。
>
> 重要考量：
>
> - 主要實體應選擇其中包含關於您的客戶的最完整和可靠個人資料的實體。
> - 主要實體應選擇與其他實體有幾項共用屬性 (例如：名稱、電話號碼或電子郵件地址) 的實體。

1. 在 **比對條件** 頁面上，使用 [上移]和 [下移] 箭頭，按照您想要的順序移動實體，或拖放它們。 例如，選取 **Contacts:eCommerces** 作為主要實體，而 **CustomerLoyalty:Loyalty** 作為第二實體。

1. 不管是否找到比對，若要讓實體中的每筆記錄作為唯一客戶，選取 **包含全部記錄**。 在此實體中，所有與其他任何實體記錄不相符的記錄都會包含在整合個人資料中。 沒有相符的記錄稱為單一值。
  
主要實體 *Contacts:eCommerce* 與下一個實體 *CustomerLoyalty:Loyalty* 比對。 如果您擁有超過兩個實體，則第一個比對步驟產生的資料集將與下列實體比對。

:::image type="content" source="media/m3_match.png" alt-text="選定的實體比對順序的螢幕擷取畫面。" lightbox="media/m3_match.png":::

## <a name="define-rules-for-match-pairs"></a>定義比對組的規則

比對規則指定將與特定實體配對進行比對的邏輯。 規則由一個或多個條件所組成。

實體名稱旁邊的警告表示沒有為比對組定義比對規則。

1. 為實體組選取 **新增規則**，以定義比對規則。

1. 在 **新增規則** 窗格中，設定規則的條件。

   :::image type="content" source="media/m3_add_rule.png" alt-text="新增規則窗格的螢幕擷取畫面。":::

   - **選取實體/欄位 (第一列)**：選擇相關實體和屬性，以指定可能對客戶是唯一的記錄屬性。 例如，電話號碼或電子郵寄地址。 避免以活動類型屬性進行比對。 例如，購買識別碼可能會在其他記錄類型中找不到符合項目。

   - **選取實體/欄位 (第二列)**：為第一列中指定的實體屬性，選擇相關屬性。

   - **正規化**：為選取的屬性從以下正規化選項中進行選擇。
     - **數字**：將其他數字系統 (如羅馬數字) 轉換為阿拉伯數字。 *VIII* 變成 *8*。
     - **符號**：刪除所有符號和特殊字元。 *Head&Shoulder* 變成 *HeadShoulder*。
     - **文字為小寫**：將所有字元轉換為小寫。 *ALL CAPS and Title Case* 變成 *all caps and title case*。
     - **類型 (電話、名稱、位址、組織)**：標準化名稱、職稱、電話號碼、地址、組織等。
     - **Unicode 到 ASCII**：將 Unicode 轉換為 ASCII 字元。 */u00B2* 變成 *2*。
     - **空白字元**：刪除所有空白。 *Hello   World* 變成 *HelloWorld*。

   - **精度**：設定適用此條件的精準度等級。
     - **基本**：從 *低 (30%)*、*中 (60%)*、*高 (80%)* 與 *完全相符 (100%)* 進行選擇。 選取 **全字詞**，只比對 100% 相符的記錄。
     - **自訂**：設定記錄需要相符的百分比。 系統將只比對超過此閾值的記錄。

   - **名稱**：規則的名稱。

1. 若只有在屬性符合多個條件時，才能比對實體，請選取 **新增** > **新增條件**，將更多條件新增至比對規則。 條件以邏輯運算子 AND 相連接，只有在滿足所有條件的情況下才會執行。

1. 或者，請考慮進階選項 ([例如例外](#add-exceptions-to-a-rule)或 [自訂比對條件](#specify-custom-match-conditions))。

1. 選取 **完成** 以完成規則。

1. 或者，[新增更多規則](#add-rules-to-a-match-pair)。

1. 按 **下一步**。

> [!div class="nextstepaction"]
> [後續步驟：整合欄位](merge-entities.md)

### <a name="add-rules-to-a-match-pair"></a>將規則新增到比對組中

比對規則代表條件組。 若要以用到多個屬性的條件來比對實體，請新增更多規則。

1. 在您想要新增規則的實體上選取 **新增規則**。

1. 遵循[對比對組訂定規則中的 ](#define-rules-for-match-pairs)步驟。

> [!NOTE]
> 規則的順序很重要。 比對演算法會嘗試根據您的第一個規則來比對指定的客戶記錄，並只在第一個規則未找出相符結果時，才繼續進行第二個規則。

## <a name="advanced-options"></a>進階選項

### <a name="add-exceptions-to-a-rule"></a>將例外新增至規則

在大多數狀況中，實體比對會以整合資料產生獨特客戶個人資料。 若要動態處理誤判和漏判的罕見案例，您可以為比對規則定義例外。 例外是在執行比對規則之後套用，且避免比對所有符合例外準則的記錄。

例如，如果比對規則結合姓氏、市/鎮及出生日期，系統會判斷居住在同一市/鎮，有著相同姓氏的雙胞胎為相同個人資料。 您可以指定例外是：如果組合實體中的名字不相同，則個人資料不相符。

1. 在 **編輯規則** 窗格中，選取 **新增** > **新增例外**。

1. 指定例外準則。

1. 選取 **完成** 以儲存規則。

### <a name="specify-custom-match-conditions"></a>指定自訂比對條件

您可以指定會覆寫預設比對邏輯的條件。 有四個可用的選項：

|選項  |Description |範例  |
|---------|---------|---------|
|永遠比對     | 定義永遠要比對的值。         |  永遠比對 *Mike* 和 *MikeR*。       |
|永不比對     | 定義永遠不比對的值。        | 永遠不比對 *John* 和 *Jonathan*。        |
|自訂略過     | 定義系統在比對階段應永遠忽略的值。 |  在比對時忽略值 *11111* 和 *Unknown*。        |
|別名對應    | 定義系統應考慮為相同值的值。         | 考慮 *Joe* 等於 *Joseph*。        |

1. 選取 **自訂**。

   :::image type="content" source="media/m3_match_custom.png" alt-text="自訂按鈕":::

1. 選擇 **自訂類型** 並選取 **下載範本**。 每個比對選項需要不同的範本。

1. 請打開下載的範本檔案，並填入詳細資料。 範本包含欄位，指定實體以及要在自訂比對中使用的實體主索引鍵值。 例如，如果您希望 *銷售* 實體的主索引鍵 *12345* 永遠與 *連絡人* 實體的主索引鍵 *34567* 相符，請寫入範本：
    - Entity1：銷售
    - Entity1Key：12345
    - Entity2：連絡人
    - Entity2Key：34567

   相同的範本檔案可以指定來自多個實體的自訂比對記錄。

   如果您想要在實體上指定重複資料刪除的自訂比對，請提供相同的實體當作 Entity1 和 Entity2 ，並設定不同主索引鍵值。

1. 新增所有覆寫之後，儲存範本檔案。

1. 前往 **資料** > **資料來源** 並將範本檔案內嵌為新實體。

1. 在上傳檔案之後，請再次選取 **自訂** 選項。 從下拉式功能表選取必要的實體，然後選取 **完成**。

   :::image type="content" source="media/custom-match-overrides.png" alt-text="螢幕擷取畫面上為選擇覆寫自訂比對案例的對話方塊。":::

1. 套用自訂比對時，會根據您要使用的比對選項而定。

   - 對於 **永遠比對** 或 **永不比對**，繼續進行下一步。
   - 對於 **略過** 或 **別名對應**，請在現有的比對規則上選取 **編輯** 或建立新規則。 在 [正規化] 下拉式功能表中，選擇 **自訂略過** 或 **別名對應** 選項，然後選取 **完成**。

1. 在 **自訂** 窗格上選取 **完成**，以套用自訂的比對設定。

> [!div class="nextstepaction"]
> [後續步驟：整合欄位](merge-entities.md)

[!INCLUDE [footer-include](includes/footer-banner.md)]