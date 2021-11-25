---
title: 公司資料增強
description: 使用 Microsoft 模型來擴充和標準化公司資料。
ms.date: 11/05/2021
ms.reviewer: mhart
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: how-to
author: kishorem-ms
ms.author: kishorem
manager: shellyha
ms.openlocfilehash: 9bfb96d47de4ec98325e644c60752fc7cab2706c
ms.sourcegitcommit: 6efcba688d1db1a5d6343c229f292a26c48fc007
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 11/05/2021
ms.locfileid: "7770197"
---
# <a name="enrichment-of-company-profiles-with-enhanced-company-data"></a>使用增強型公司設定資料來擴充公司資料

使用 Microsoft 模型及已彙集的公司資料，來更正、補充和標準化您的公司設定資料。 我們將使用 [Common Data Model 格式 ](/common-data-model/schema/core/applicationcommon/account)，以取得更佳的準確性和見解。

## <a name="how-we-enhance-company-data"></a>我們如何增強公司資料

我們的模型經過兩步驟程序，來增強公司設定資料。 首先，它會標準化公司名稱。 例如，*Microsoft Corp* 將會被修正並標準化至 *Microsoft Corporation*。 它會嘗試在 Microsoft 已彙集的公司資料中尋找相符項目。 如果找到相符項目，我們就會使用我們所搜集的公司資料 (包括公司名稱) 來擴充公司設定資料。


### <a name="example"></a>範例

您的公司資訊可能不符合標準格式，並包含拼寫錯誤。 模型會嘗試修正這些問題，並建立一致的資訊。

```Input
Microsft
```

```Output
- AccountName: Microsoft Corporation
- MainPhoneNumber: 8006427676
- Website: https://www.microsoft.com/
- Street1: One Microsoft Way
- City: Redmond
- StateOrProvince: Washington
- County: King
- ZipOrPostalCode: 98052
- CountryOrRegion: United States
```

## <a name="limitations"></a>限制

增強型資料有一些限制。 模型不支援下列清單中的項目。

1.  確認公司的身份。 我們不會驗證輸入內容是否為現有的組織，或驗證是否有公司使用輸出內容做為其標準名稱。
2.  全面涵蓋全球公司。 Microsoft 的已彙集的公司資料可涵蓋全球範圍，但提供的涵蓋區域大部分在澳大利亞、加拿大、英國和美國。
3.  保證資料的準確性或新穎度。 隨著商務資訊經常變更，我們無法保證提供的增強型公司資料總是準確或最新的。

## <a name="configure-the-enrichment"></a>擴充設定

1. 移至 **資料** > **擴充**。

1. 在 **增強型公司資料** 圖格中，選取 **擴充我的資料**。

   :::image type="content" source="media/enhanced-company-data-tile.png" alt-text="在擴充中心的公司資料擴充圖格。":::

1. 選取 **客戶資料集**，並選擇包含要擴充地址的實體。 您可以選取 *客戶* 實體來擴充所有客戶個人資料中的位址，或者選取一個客戶細分實體來擴充只在該客戶細分中包含的客戶個人資料內的位址。

1. 選取您的公司設定資料中要用來與 Microsoft 已彙集公司資料比對的欄位類型。 這項選取將會影響在下一個步驟中可以存取的對應欄位。

1.  從您的整合客戶實體中對應公司欄位。 對應的關鍵識別碼和欄位越多，就有機會出現越高的比對率。

    :::image type="content" source="media/enhanced-company-data-mapping.png" alt-text="設定公司擴充時的資料對應步驟。":::

1. 請選取 **下一步**，完成欄位對應。

1. 提供擴充與輸出實體的名稱。

1. 檢閱選擇之後，請選取 **儲存擴充**。

## <a name="enrichment-results"></a>擴充結果

若要開始擴充程序，請從命令列中選取 **執行**。 您也可以讓系統在[排定的重新整理](system.md#schedule-tab)過程中自動執行擴充。 處理時間視客戶資料的大小而定。

擴充程序完成後，您可以在 **我的擴充內容** 底下查看新擴充的客戶設定檔資料。 此外，您還會找到上次更新時間以及已擴充的設定檔數目。

您可以選取 **檢視擴充的資料** 來存取每個已擴充設定檔的詳細檢視表。

## <a name="next-steps"></a>後續步驟

[!INCLUDE [next-steps-enrichment](../includes/next-steps-enrichment.md)]

[!INCLUDE[footer-include](../includes/footer-banner.md)]
