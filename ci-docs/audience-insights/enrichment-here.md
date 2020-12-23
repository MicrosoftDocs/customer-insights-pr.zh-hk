---
title: 藉助協力廠商 HERE Technologies 的富集作用
description: 有關 HERE Technologies 協力廠商富集作用的一般資訊。
ms.date: 10/27/2020
ms.reviewer: jodahl
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: conceptual
author: m-hartmann
ms.author: mhart
manager: shellyha
ms.openlocfilehash: 7082fcfec099c3c9436b233c193be23625f6691a
ms.sourcegitcommit: a9b2cf598f256d07a48bba8617347ee90024a1dd
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 12/03/2020
ms.locfileid: "4668705"
---
# <a name="enrichment-of-customer-profiles-with-here-technologies-preview"></a><span data-ttu-id="a7374-103">HERE Technologies 客戶設定檔的富集作用 (預覽版)</span><span class="sxs-lookup"><span data-stu-id="a7374-103">Enrichment of customer profiles with HERE Technologies (preview)</span></span>

<span data-ttu-id="a7374-104">HERE Technologies 是一間位置平台公司，提供以位置為中心的資料和服務。</span><span class="sxs-lookup"><span data-stu-id="a7374-104">HERE Technologies is a location platform company that provides location-centric data and services.</span></span> <span data-ttu-id="a7374-105">您可以使用 HERE Technologies 的資料富集服務建立對您客戶位址正規化、緯度和經度擷取等更精確的位置瞭解。</span><span class="sxs-lookup"><span data-stu-id="a7374-105">With HERE Technologies' data enrichment services, you can build a more precise location understanding of your customers with address normalization, latitude and longitude extraction, and more.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a7374-106">先決條件</span><span class="sxs-lookup"><span data-stu-id="a7374-106">Prerequisites</span></span>

<span data-ttu-id="a7374-107">若要組態 HERE Technologies 富集作用，必須符合下列先決條件：</span><span class="sxs-lookup"><span data-stu-id="a7374-107">To configure HERE Technologies enrichments, the following prerequisites must be met:</span></span>

- <span data-ttu-id="a7374-108">您已具備有效的 HERE Technologies 訂閱。</span><span class="sxs-lookup"><span data-stu-id="a7374-108">You have an active HERE Technologies subscription.</span></span> <span data-ttu-id="a7374-109">若要訂閱，您可以 [在這裡註冊](https://developer.here.com/sign-up?utm_medium=referral&utm_source=Microsoft-Dynamics-CI&create=Freemium-Basic) 或直接 [聯絡 HERE Technologies](https://developer.here.com/help?utm_medium=referral&utm_source=Microsoft-Dynamics-CI#how-can-we-help-you)。</span><span class="sxs-lookup"><span data-stu-id="a7374-109">To get a subscription, you can [sign-up here](https://developer.here.com/sign-up?utm_medium=referral&utm_source=Microsoft-Dynamics-CI&create=Freemium-Basic) or [contact HERE Technologies](https://developer.here.com/help?utm_medium=referral&utm_source=Microsoft-Dynamics-CI#how-can-we-help-you) directly.</span></span> [<span data-ttu-id="a7374-110">深入瞭解 HERE Technologies 的 Location Enrichment。</span><span class="sxs-lookup"><span data-stu-id="a7374-110">Learn more about HERE Technologies Location Enrichment.</span></span>](https://developer.here.com/location-enrichment?cid=Dev-MicrosoftDynamics-DB-0-Dev-&utm_source=MicrosoftDynamics&utm_medium=referral&utm_campaign=Online_Dev_ReferralMicrosoft)

- <span data-ttu-id="a7374-111">您擁有 HERE Technologies API 金鑰。</span><span class="sxs-lookup"><span data-stu-id="a7374-111">You have the HERE Technologies API key.</span></span>

- <span data-ttu-id="a7374-112">您擁有 [系統管理員](permissions.md#administrator) 權限。</span><span class="sxs-lookup"><span data-stu-id="a7374-112">You have [Administrator](permissions.md#administrator) permissions.</span></span>

## <a name="configuration"></a><span data-ttu-id="a7374-113">組態</span><span class="sxs-lookup"><span data-stu-id="a7374-113">Configuration</span></span>

1. <span data-ttu-id="a7374-114">移至 **資料** > **擴充**。</span><span class="sxs-lookup"><span data-stu-id="a7374-114">Go to **Data** > **Enrichment**.</span></span>

1. <span data-ttu-id="a7374-115">請在 HERE Technologies 圖格上選取 **富集我的資料**。</span><span class="sxs-lookup"><span data-stu-id="a7374-115">Select **Enrich my data** on the HERE Technologies tile.</span></span>

   > [!div class="mx-imgBorder"]
   > <span data-ttu-id="a7374-116">![HERE Technologies 圖格](media/HERE-tile.png "HERE Technologies 圖格")</span><span class="sxs-lookup"><span data-stu-id="a7374-116">![HERE Technologies tile](media/HERE-tile.png "HERE Technologies tile")</span></span>

1. <span data-ttu-id="a7374-117">輸入有效的 **HERE Technologies API 金鑰**。</span><span class="sxs-lookup"><span data-stu-id="a7374-117">Enter an active **HERE Technologies API key**.</span></span> <span data-ttu-id="a7374-118">選取 **我同意** 核取方塊，以檢閱 **資料隱私權和合規性** 並表示同意。</span><span class="sxs-lookup"><span data-stu-id="a7374-118">Review and provide your consent for **Data privacy and compliance** by selecting the **I agree** checkbox.</span></span> 

1. <span data-ttu-id="a7374-119">選取 **連接到 HERE** 確認這兩項輸入資料。</span><span class="sxs-lookup"><span data-stu-id="a7374-119">Confirm both inputs by selecting **Connect to HERE**.</span></span>

1. <span data-ttu-id="a7374-120">選取 **新增資料** 並選擇是否要將欄位對應到主要和/或次要位址。</span><span class="sxs-lookup"><span data-stu-id="a7374-120">Select **Add data** and choose if you want to map fields to the primary and/or secondary address.</span></span> <span data-ttu-id="a7374-121">您可以為兩個位址指定欄位對應 (例如住宅和公司位址)，然後分別富集兩個位址的設定檔。</span><span class="sxs-lookup"><span data-stu-id="a7374-121">You can specify a field mapping for both addresses (for example, a home and a business address) and enrich the profiles for both addresses separately.</span></span> <span data-ttu-id="a7374-122">選取 **下一步**。</span><span class="sxs-lookup"><span data-stu-id="a7374-122">Select **Next**.</span></span>

1. <span data-ttu-id="a7374-123">定義應使用您的哪些統一設定檔欄位，以尋找符合 HERE Technologies 的位置資料。</span><span class="sxs-lookup"><span data-stu-id="a7374-123">Define which fields from your unified profiles should be used to look for matching location data from HERE Technologies.</span></span> <span data-ttu-id="a7374-124">**街道 1** 和 **郵遞區號** 欄位是選取的主要和/或次要位址的必要欄位。</span><span class="sxs-lookup"><span data-stu-id="a7374-124">The **Street 1** and **Zip/Postal Code** fields are required for the selected primary and/or secondary address.</span></span> <span data-ttu-id="a7374-125">為了更高的符合準確性，可以新增更多欄位。</span><span class="sxs-lookup"><span data-stu-id="a7374-125">For a higher match accuracy, more fields can be added.</span></span>

   > [!div class="mx-imgBorder"]
   > <span data-ttu-id="a7374-126">![HERE Technologies 富集組態頁面](media/enrichment-HERE-configuration.png "HERE Technologies 富集組態頁面")</span><span class="sxs-lookup"><span data-stu-id="a7374-126">![HERE Technologies enrichment configuration page](media/enrichment-HERE-configuration.png "HERE Technologies enrichment configuration page")</span></span>

1. <span data-ttu-id="a7374-127">選取 **套用** 完成欄位對應。</span><span class="sxs-lookup"><span data-stu-id="a7374-127">Select **Apply** to complete the field mapping.</span></span>

## <a name="enrichment-results"></a><span data-ttu-id="a7374-128">擴充結果</span><span class="sxs-lookup"><span data-stu-id="a7374-128">Enrichment results</span></span>

<span data-ttu-id="a7374-129">若要開始擴充程序，請從命令列中選取 **執行**。</span><span class="sxs-lookup"><span data-stu-id="a7374-129">To start the enrichment process, select **Run** from the command bar.</span></span> <span data-ttu-id="a7374-130">您也可以讓系統在[排定的重新整理](system.md#schedule-tab)過程中自動執行擴充。</span><span class="sxs-lookup"><span data-stu-id="a7374-130">You can also let the system run the enrichment automatically as part of a [scheduled refresh](system.md#schedule-tab).</span></span> <span data-ttu-id="a7374-131">處理時間將視您的客戶資料大小和 HERE Technologies 的 API 回應時間而定。</span><span class="sxs-lookup"><span data-stu-id="a7374-131">The processing time will depend on the size of your customer data and the API response times from HERE Technologies.</span></span>

<span data-ttu-id="a7374-132">擴充程序完成後，您可以在 **我的擴充內容** 底下查看新擴充的客戶設定檔資料。</span><span class="sxs-lookup"><span data-stu-id="a7374-132">After the enrichment process completes, you can review the newly enriched customer profiles data under **My enrichments**.</span></span> <span data-ttu-id="a7374-133">此外，您還會找到上次更新時間以及已擴充的設定檔數目。</span><span class="sxs-lookup"><span data-stu-id="a7374-133">Additionally, you'll find the time of the last update and the number of enriched profiles.</span></span>

<span data-ttu-id="a7374-134">您可以選取 **檢視擴充的資料** 來存取每個已擴充設定檔的詳細檢視表。</span><span class="sxs-lookup"><span data-stu-id="a7374-134">You can access a detailed view of each enriched profile by selecting **View enriched data**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a7374-135">後續步驟</span><span class="sxs-lookup"><span data-stu-id="a7374-135">Next steps</span></span>

<span data-ttu-id="a7374-136">建立在您擴充的客戶資料之上。</span><span class="sxs-lookup"><span data-stu-id="a7374-136">Build on top of your enriched customer data.</span></span> <span data-ttu-id="a7374-137">建立[客戶細分](segments.md)、[量值](measures.md)，甚至[匯出資料](export-destinations.md)，以便傳送個人化體驗給您的客戶。</span><span class="sxs-lookup"><span data-stu-id="a7374-137">Create [segments](segments.md), [measures](measures.md), and even [export the data](export-destinations.md) to deliver personalized experiences to your customers.</span></span>

## <a name="data-privacy-and-compliance"></a><span data-ttu-id="a7374-138">資料隱私權與合規性</span><span class="sxs-lookup"><span data-stu-id="a7374-138">Data privacy and compliance</span></span>

<span data-ttu-id="a7374-139">當您啟用 Dynamics 365 Customer Insights 將資料傳輸給 HERE Technologies 時，您允許在合規性邊界之外傳輸 Dynamics 365 Customer Insights 資料，包括潛在敏感性資料如個人資料。</span><span class="sxs-lookup"><span data-stu-id="a7374-139">When you enable Dynamics 365 Customer Insights to transmit data to HERE Technologies, you allow transfer of data outside of the compliance boundary for Dynamics 365 Customer Insights, including potentially sensitive data such as Personal Data.</span></span> <span data-ttu-id="a7374-140">Microsoft 將依據您的指示傳輸此資料，但您須負責確保 HERE Technologies 符合您可能應盡的任何隱私權或資訊安全義務。</span><span class="sxs-lookup"><span data-stu-id="a7374-140">Microsoft will transfer such data at your instruction, but you are responsible for ensuring that HERE Technologies meets any privacy or security obligations you may have.</span></span> <span data-ttu-id="a7374-141">如需詳細資訊，請參閱 [Microsoft 隱私權聲明](https://go.microsoft.com/fwlink/?linkid=396732)。</span><span class="sxs-lookup"><span data-stu-id="a7374-141">For more information, see [Microsoft Privacy Statement](https://go.microsoft.com/fwlink/?linkid=396732).</span></span>
<span data-ttu-id="a7374-142">您的 Dynamics 365 Customer Insights 系統管理員可以隨時移除此富集作用，以便不再繼續使用此功能。</span><span class="sxs-lookup"><span data-stu-id="a7374-142">Your Dynamics 365 Customer Insights Administrator can remove this enrichment at any time to discontinue use of this functionality.</span></span>
