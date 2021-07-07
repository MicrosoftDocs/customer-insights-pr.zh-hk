---
title: 地址增強擴充
description: 使用 Microsoft 模型擴充和標準化客戶個人資料的地址資訊。
ms.date: 04/21/2021
ms.reviewer: mhart
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: how-to
author: kishorem-ms
ms.author: kishorem
manager: shellyha
ms.openlocfilehash: e0ca731f944da9a7eaae7c2dc2d7568b6386089f
ms.sourcegitcommit: d84d664e67f263bfeb741154d309088c5101b9c3
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 06/24/2021
ms.locfileid: "6305459"
---
# <a name="enrichment-of-customer-profiles-with-enhanced-addresses"></a><span data-ttu-id="6f4c3-103">以增強的地址擴充的客戶個人資料</span><span class="sxs-lookup"><span data-stu-id="6f4c3-103">Enrichment of customer profiles with enhanced addresses</span></span>

<span data-ttu-id="6f4c3-104">資料中的地址可能未結構化、不完整或不正確。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-104">Addresses in your data can be unstructured, incomplete, or incorrect.</span></span> <span data-ttu-id="6f4c3-105">使用 Microsoft 的模型，標準化地址並擴充成 [Common Data Model 格式](/common-data-model/schema/core/applicationcommon/address)，以取得更佳的準確性和洞察力。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-105">Use Microsoft's models to normalize and enrich your addresses into the [Common Data Model format](/common-data-model/schema/core/applicationcommon/address) for better accuracy and insights.</span></span>

## <a name="how-we-enhance-addresses"></a><span data-ttu-id="6f4c3-106">我們如何增強地址</span><span class="sxs-lookup"><span data-stu-id="6f4c3-106">How we enhance addresses</span></span>

<span data-ttu-id="6f4c3-107">我們的模型以二步驟流程來增強地址。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-107">Our model goes through a two-step process to enhance an address.</span></span> <span data-ttu-id="6f4c3-108">首先，它會解析地址找出其組成部分，並將它們設定為結構化格式。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-108">First, it parses the address to identify its components and puts them into a structured format.</span></span> <span data-ttu-id="6f4c3-109">然後，我們使用 AI 來更正、完成並標準化地址中的值。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-109">Then, we use AI to correct, complete, and standardize the values in the address.</span></span>

### <a name="example"></a><span data-ttu-id="6f4c3-110">範例</span><span class="sxs-lookup"><span data-stu-id="6f4c3-110">Example</span></span>

<span data-ttu-id="6f4c3-111">地址資訊可能以非標準格式存在，並包含拼寫錯誤。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-111">Address information might be in a nonstandard format and contain spelling errors.</span></span> <span data-ttu-id="6f4c3-112">此模型可以修正這些問題，並在整合的客戶個人資料中建立一致的地址。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-112">The model can fix these issues and create consistent addresses in unified customer profiles.</span></span>

```Input
4567 w main stret californa missouri 54321 us
```

```Output
- Street1: 4567 W Main St
- City: California
- StateOrProvince: MO
- ZipOrPostalCode: 54321
- CountryOrRegion: United States of America

- Address: 4567 W Main St, California, MO, 54321, United States of America
```

### <a name="limitations"></a><span data-ttu-id="6f4c3-113">限制</span><span class="sxs-lookup"><span data-stu-id="6f4c3-113">Limitations</span></span>

<span data-ttu-id="6f4c3-114">增強位址只能用在已擷取的地址資料中現有的值。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-114">Enhanced addresses only works with the values that already exist in your ingested address data.</span></span> <span data-ttu-id="6f4c3-115">模型不能：</span><span class="sxs-lookup"><span data-stu-id="6f4c3-115">The model doesn't:</span></span> 

1. <span data-ttu-id="6f4c3-116">確認地址是否為有效的地址。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-116">Verify if the address is a valid address.</span></span>
2. <span data-ttu-id="6f4c3-117">確認任何值 (如郵遞區號或街道名稱) 是有效的。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-117">Verify if any of the values, such as ZIP codes or street names, are valid.</span></span>
3. <span data-ttu-id="6f4c3-118">變更無法識別的值。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-118">Change values it doesn't recognize.</span></span>

<span data-ttu-id="6f4c3-119">此模型使用機器學習技術來增強地址。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-119">The model uses machine learning-based techniques to enhance addresses.</span></span> <span data-ttu-id="6f4c3-120">雖然在模型更改輸入值時，我們套用了高信賴度閾值，但與任何基於機器學習的模型一樣，無法保證 100% 的準確性。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-120">While we apply a high confidence threshold for when the model changes an input value, as with any machine learning-based model, 100 percent accuracy is not guaranteed.</span></span>

## <a name="supported-countries-or-regions"></a><span data-ttu-id="6f4c3-121">支援的國家或地區</span><span class="sxs-lookup"><span data-stu-id="6f4c3-121">Supported countries or regions</span></span>

<span data-ttu-id="6f4c3-122">目前我們在這些國家或地區支援增強地址：</span><span class="sxs-lookup"><span data-stu-id="6f4c3-122">We currently support enriching addresses in these countries or regions:</span></span> 

- <span data-ttu-id="6f4c3-123">澳洲</span><span class="sxs-lookup"><span data-stu-id="6f4c3-123">Australia</span></span>
- <span data-ttu-id="6f4c3-124">加拿大</span><span class="sxs-lookup"><span data-stu-id="6f4c3-124">Canada</span></span>
- <span data-ttu-id="6f4c3-125">英國</span><span class="sxs-lookup"><span data-stu-id="6f4c3-125">United Kingdom</span></span>
- <span data-ttu-id="6f4c3-126">美國</span><span class="sxs-lookup"><span data-stu-id="6f4c3-126">United States</span></span>

<span data-ttu-id="6f4c3-127">地址必須包含國家/地區值。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-127">Addresses must contain a country/region value.</span></span> <span data-ttu-id="6f4c3-128">不支援的國家或地區的地址以及沒有提供國家或地區的地址，無法處理。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-128">We don't process addresses for countries or regions that aren't supported and addresses that have no country or region provided.</span></span>

## <a name="configure-the-enrichment"></a><span data-ttu-id="6f4c3-129">擴充設定</span><span class="sxs-lookup"><span data-stu-id="6f4c3-129">Configure the enrichment</span></span>

1. <span data-ttu-id="6f4c3-130">移至 **資料** > **擴充**。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-130">Go to **Data** > **Enrichment**.</span></span>

1. <span data-ttu-id="6f4c3-131">在 **增強地址** 圖格中，選取 **擴充資料**。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-131">Select **Enrich my data** on the **Enhanced addresses** tile.</span></span>

   :::image type="content" source="media/enhanced-addresses-tile.png" alt-text="增強地址圖格的螢幕擷取畫面。":::

1. <span data-ttu-id="6f4c3-133">選取 **客戶資料集**，並選擇包含要擴充地址的實體。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-133">Select the **Customer data set** and choose the entity containing the addresses you want to enrich.</span></span> <span data-ttu-id="6f4c3-134">您可以選取 *客戶* 實體來擴充所有客戶個人資料中的位址，或者選取一個客戶細分實體來擴充只在該客戶細分中包含的客戶個人資料內的位址。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-134">You can select the *Customer* entity to enrich addresses in all your customer profiles or select a segment entity to enrich addresses only in customer profiles contained in that segment.</span></span>

1. <span data-ttu-id="6f4c3-135">選取在資料集中格式化地址的方式。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-135">Select how addresses are formatted in your data set.</span></span> <span data-ttu-id="6f4c3-136">若資料中的地址使用單一欄位，請選擇 **單一屬性位址**。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-136">Choose **Single-attribute address** if addresses in your data use a single field.</span></span> <span data-ttu-id="6f4c3-137">若資料中的地址使用超過一個資料欄位，請選擇 **複數屬性地址**。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-137">Choose **Multiple-attribute address** if addresses in your data use more than one data field.</span></span>

   > [!NOTE]
   > <span data-ttu-id="6f4c3-138">單屬性和多屬性位址都必須有國家/地區。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-138">Country/Region is mandatory in both single-attribute and multiple-attribute addresses.</span></span> <span data-ttu-id="6f4c3-139">缺乏有效或受支援的國家/地區值的地址將不會被擴充。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-139">Addresses that don't contain valid or supported country/region values won't be enriched.</span></span>

1.  <span data-ttu-id="6f4c3-140">請從整合客戶實體對應至地址欄位。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-140">Map the address fields from your unified customer entity.</span></span>

    :::image type="content" source="media/enhanced-address-mapping.png" alt-text="增強地址的欄位對應頁面。":::

1. <span data-ttu-id="6f4c3-142">請選取 **下一步**，完成欄位對應。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-142">Select **Next** to complete the field mapping.</span></span>

1. <span data-ttu-id="6f4c3-143">提供擴充與輸出實體的名稱。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-143">Provide a name for the enrichment and the output entity.</span></span>

1. <span data-ttu-id="6f4c3-144">檢閱選擇之後，請選取 **儲存擴充**。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-144">Select **Save enrichment** after reviewing your choices.</span></span>

## <a name="enrichment-results"></a><span data-ttu-id="6f4c3-145">擴充結果</span><span class="sxs-lookup"><span data-stu-id="6f4c3-145">Enrichment results</span></span>

<span data-ttu-id="6f4c3-146">若要開始擴充程序，請從命令列中選取 **執行**。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-146">To start the enrichment process, select **Run** from the command bar.</span></span> <span data-ttu-id="6f4c3-147">您也可以讓系統在[排定的重新整理](system.md#schedule-tab)過程中自動執行擴充。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-147">You can also let the system run the enrichment automatically as part of a [scheduled refresh](system.md#schedule-tab).</span></span> <span data-ttu-id="6f4c3-148">處理時間視客戶資料的大小而定。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-148">The processing time depends on the size of your customer data.</span></span>

<span data-ttu-id="6f4c3-149">擴充程序完成後，您可以在 **我的擴充內容** 底下查看新擴充的客戶設定檔資料。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-149">After the enrichment process completes, you can review the newly enriched customer profiles data under **My enrichments**.</span></span> <span data-ttu-id="6f4c3-150">此外，您還會找到上次更新時間以及已擴充的設定檔數目。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-150">Additionally, you'll find the time of the last update and the number of enriched profiles.</span></span>

<span data-ttu-id="6f4c3-151">您可以選取 **檢視擴充的資料** 來存取每個已擴充設定檔的詳細檢視表。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-151">You can access a detailed view of each enriched profile by selecting **View enriched data**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6f4c3-152">後續步驟</span><span class="sxs-lookup"><span data-stu-id="6f4c3-152">Next steps</span></span>

<span data-ttu-id="6f4c3-153">建立在您擴充的客戶資料之上。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-153">Build on top of your enriched customer data.</span></span> <span data-ttu-id="6f4c3-154">建立[客戶細分](segments.md)和 [量值 ](measures.md)，甚至 [匯出資料](export-destinations.md)，為您的客戶提供個人化的體驗。</span><span class="sxs-lookup"><span data-stu-id="6f4c3-154">Create [segments](segments.md) and [measures](measures.md), and even [export the data](export-destinations.md) to deliver personalized experiences to your customers.</span></span>

[!INCLUDE[footer-include](../includes/footer-banner.md)]
