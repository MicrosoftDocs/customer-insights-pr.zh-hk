---
title: 使用 Microsoft Graph 富集客戶設定檔
description: 使用 Microsoft Graph 的專有資料，使用品牌和興趣親和性來擴充您的客戶資料。
ms.date: 12/10/2020
ms.reviewer: kishorem
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: how-to
author: m-hartmann
ms.author: mhart
manager: shellyha
ms.openlocfilehash: 2c95369c778f592bc1460799aca0fa8cff813d68
ms.sourcegitcommit: 139548f8a2d0f24d54c4a6c404a743eeeb8ef8e0
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 02/15/2021
ms.locfileid: "5269357"
---
# <a name="enrich-customer-profiles-with-brand-and-interest-affinities-preview"></a>使用品牌和興趣親和性來擴充客戶設定檔 (預覽)

使用 Microsoft Graph 的專有資料，使用品牌和興趣親和性來擴充您的客戶資料。 這些親和性是根據與客戶有類似人口統計資料之人員的資料所決定。 此資訊可協助您更清楚了解客戶，並根據客戶與特定品牌及興趣的親和性建立其區段。

請在對象見解中前往 **資料** > **擴充** 以便 [設定和檢視擴充](enrichment-hub.md)。

若要設定品牌親和性擴充，請移至 **探索** 索引標籤 ，並選取 **品牌** 圖標上的 **擴充我的資料**。

若要設定興趣親和性擴充，請移至 **探索** 索引標籤 ，並選取 **興趣** 圖標上的 **擴充我的資料**。

   > [!div class="mx-imgBorder"]
   > ![品牌與興趣圖標](media/BrandsInterest-tile-Hub.png "品牌與興趣圖標")

## <a name="about-microsoft-graph"></a>關於 Microsoft Graph

我們使用 Microsoft Graph 的線上搜尋資料，在各種人口統計資料區段（依年限、性別或位置定義）尋找品牌和興趣親和性。 品牌或興趣的線上搜尋量，會決定人口統計區段對該品牌或興趣有多少親和性 (與其他區段相比)。

[深入了解 Microsoft Graph](https://docs.microsoft.com/graph/overview)。

## <a name="affinity-level-and-score"></a>親合性等級和分數

每一個擴充的客戶設定檔，我們都提供兩個相關的值 – 親合性等級和親合性分數。 這些值可協助您判斷與其他人口統計資料段相比，該設定檔人口統計資料客戶細分、品牌或興趣的親和性強弱程度。

*親和性等級* 由四個等級所組成，而 *親和性分數* 是在對應親和性等級在 100 分範圍中的計算結果。


|親和性等級 |親和性分數  |
|---------|---------|
|非常高     | 85-100       |
|高     | 70-84        |
|中     | 35-69        |
|低     | 1-34        |

根據您要測量親和性的細微程度，您可以使用親和性等級或分數。 親和性分數提供更精確的控制。

## <a name="supported-countriesregions"></a>支援的國家/地區

我們目前支援下列國家/地區選項：澳大利亞、加拿大 (英文)、法國、德國、英國或美國 (英文)。

若要選取國家/地區，請開啟 **品牌擴充** 或 **興趣擴充**，然後選取 **國家/地區** 旁邊的 **變更**。 在 **國家/地區設定** 窗格中，選擇選項並選取 **套用**。

### <a name="implications-related-to-country-selection"></a>與國家/地區選取相關的影響

- 當[選擇您的自有品牌](#define-your-brands-or-interests)時，系統會根據選取的國家或地區提供建議。

- [選擇產業時](#define-your-brands-or-interests)，將得到與您選取的國家或地區最相關的品牌或興趣。

- 在[擴充設定檔](#refresh-enrichment)時，我們會針對選取的品牌和興趣資料用已取得的資料擴充所有客戶設定檔。 包括不在選取的國家或地區中的設定檔。 例如，當您選取德國時，如果我們在美國有適用於所選品牌及興趣的 Microsoft Graph 資料，則會擴充位於美國的設定檔。

## <a name="configure-enrichment"></a>設定擴充

### <a name="define-your-brands-or-interests"></a>定義您的品牌或興趣

選取下列其中一個選項：

- **產業**：系統會找出與您的行業相關的最上層品牌或興趣，並使用它們擴充您的客戶資料。
- **自行選擇**：從與您的組織最相關的品牌或興趣清單中，選取最多五個項目。

若要新增品牌或興趣，請在輸入區域中輸入，以依據符合的字詞取得建議。 如果我們未列出您要尋找的品牌或興趣，請使用 **建議** 連結向我們傳送意見。

### <a name="review-enrichment-preferences"></a>查看擴充喜好設定

查看預設的擴充喜好設定，並視需要加以更新。

:::image type="content" source="media/affinity-enrichment-preferences.png" alt-text="擴充喜好設定視窗的螢幕擷取畫面。":::

### <a name="select-entity-to-enrich"></a>選取要擴充的實體

選取 **擴充實體**，然後選擇要用 Microsoft Graph 中的公司資料進行擴充的資料集。 您可以選取客戶實體來擴充所有的客戶設定檔，或選取客戶細分實體僅擴充位於該客戶細分的客戶設定檔。

### <a name="map-your-fields"></a>對應欄位

對應統整客戶實體中的欄位，以定義您要讓系統用來擴充客戶資料的人口統計客戶細分。 對應國家/地區以及至少要出生日期或性別屬性。 此外，您至少必須對應一個市/鎮 (和縣/市) 或郵遞區號。 選取 **編輯** 以定義欄位對應，並在完成時選取 **套用**。 選取 **儲存** 來完成欄位對應。

支援下列格式和值，這些值不區分大小寫：

- **出生日期**：建議在資料擷取期間，將出生日期轉換為日期時間類型。 或者，也可以是使用 [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) 格式 "yyyy-MM-dd" 或 "yyyy-MM-ddTHH:mm:ssZ" 的字串。
- **性別**：男、女、未知
- **郵遞區號**：美國的五位數字郵遞區號、其他地區的標準郵遞區號
- **城市**：英文城市名稱
- **州/省**：美國和加拿大的兩字母縮寫。 澳大利亞的兩字母或三字母縮寫。 不適用於法國、德國或英國。
- **國家/地區**：

  - US：美利堅合眾國、美國、USA、US、美國、美洲
  - CA：加拿大、CA
  - GB：英國、UK、大不列顛、GB、大不列顛與北愛爾蘭聯合王國、大不列顛聯合王國
  - AU：澳大利亞、AU、澳大利亞聯邦
  - FR：法國、FR、法蘭西共和國
  - DE：德國、德文、Deutschland、Allemagne、DE、德意志聯邦共和國、德意志共和國

## <a name="refresh-enrichment"></a>重新整理擴充項目

在為人口統計設定品牌、興趣和欄位對應之後，請執行擴充。 若要開始此程序，請在品牌或興趣設定頁面上選取 **執行**。 此外，您還可以讓系統在排程的重新整理過程中自動執行擴充。
視您的客戶資料大小而定，可能需要數分鐘的時間才能完成擴充執行。

> [!TIP]
> 任務/流程目前有 [六種類型的狀態](system.md#status-types)。 此外，大部分程序都要[依賴其他下游程序](system.md#refresh-policies)。 您可以選取程序的狀態，以查看整個工作的進度詳細資料。 針對其中一項作業的工作選取 **查看詳細資料** 之後，您會找到其他資訊：處理時間、上次處理日期以及所有與工作相關的錯誤和警告。

## <a name="enrichment-results"></a>擴充結果

執行擴充程序之後，移至 **我的擴充內容** 以檢閱已擴充的客戶總數，以及擴充後客戶設定檔中的品牌或興趣明細。

:::image type="content" source="media/my-enrichments.png" alt-text="執行擴充程序之後的結果預覽":::

在圖表中選取 **查看已擴充資料**，以查看擴充後的資料。 擴充的品牌資料會移至 **BrandAffinityFromMicrosoft** 實體。 興趣資料位於 **InterestAffinityFromMicrosoft** 實體中。 您也可以 **資料** > **實體** 的 **擴充** 群組中找到這些實體。

## <a name="see-enrichment-data-on-the-customer-card"></a>查看客戶卡片上的擴充資料

您也可以在個別客戶卡片上查看品牌和興趣親和性。 移至 **客戶** 並選取客戶設定檔。 在客戶卡片中，您會發現該客戶人口統計設定檔中人員所喜好品牌或興趣的圖表。

:::image type="content" source="media/enrichment-customer-card.png" alt-text="包含擴充資料的客戶卡片":::

## <a name="next-steps"></a>後續步驟

建立在您擴充的客戶資料之上。 建立[區段](segments.md)、[量值](measures.md)，甚至[匯出資料](export-destinations.md)，以便傳送個人化體驗給您的客戶。


[!INCLUDE[footer-include](../includes/footer-banner.md)]