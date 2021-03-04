---
title: 新功能以及近期即將推出的功能
description: 關於新功能、改善和 BUG 修正的資訊。
ms.date: 02/02/2021
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: conceptual
author: m-hartmann
ms.author: mhart
ms.reviewer: midevane
manager: shellyha
ms.openlocfilehash: 9183c8af4fb9f9f08ac63d8d0cd37c6868bba310
ms.sourcegitcommit: 139548f8a2d0f24d54c4a6c404a743eeeb8ef8e0
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 02/15/2021
ms.locfileid: "5270459"
---
# <a name="whats-new-in-the-audience-insights-capability-of-dynamics-365-customer-insights"></a><span data-ttu-id="8ed3f-103">Dynamics 365 Customer Insights 的觀象見解能力有什麼新發表的功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-103">What's new in the audience insights capability of Dynamics 365 Customer Insights</span></span>

[!INCLUDE [cc-data-platform-banner](../includes/cc-data-platform-banner.md)]

<span data-ttu-id="8ed3f-104">我們很高興宣布我們最新的更新！</span><span class="sxs-lookup"><span data-stu-id="8ed3f-104">We're excited to announce our newest updates!</span></span> <span data-ttu-id="8ed3f-105">本文摘要說明公開預覽功能、正式發行增強功能以及功能更新。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-105">This article summarizes public preview features, general availability enhancements, and feature updates.</span></span> <span data-ttu-id="8ed3f-106">若要查看長期功能計劃，請參閱 [Dynamics 365 和 Power Platform 發行計劃](https://docs.microsoft.com/dynamics365/release-plans/)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-106">To see the long-term feature plans, take a look at the [Dynamics 365 and Power Platform release plans](https://docs.microsoft.com/dynamics365/release-plans/).</span></span>

<span data-ttu-id="8ed3f-107">您也可以觀看下列影片，多瞭解過去六個月已規劃的功能。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-107">You can also watch the following video to learn more about the capabilities planned for the last six months.</span></span>

> [!VIDEO https://www.youtube.com/embed/jQh-7pscH30]

<span data-ttu-id="8ed3f-108">我們會逐一在各地區推出更新。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-108">We roll out updates on a region-by-region basis.</span></span> <span data-ttu-id="8ed3f-109">因此可能會在特定地區提前看到其他地區尚未推出的功能。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-109">So certain regions might see features before others.</span></span> <span data-ttu-id="8ed3f-110">除非另有指示，您不需要採取任何動作，我們會在不停機的情況下自動更新應用程式。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-110">Unless specified differently, you don't need to take any action and we'll update the app automatically with no downtime.</span></span>

> [!TIP]
> <span data-ttu-id="8ed3f-111">若要送出和票選功能要求和產品建議，請前往 [Dynamics 365 應用程式想法入口網站](https://experience.dynamics.com/ideas/categories/?forum=79a8c474-4e35-e911-a971-000d3a4f3343&forumName=Dynamics%20365%20Customer%20Insights)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-111">To submit and vote on feature requests and product suggestions, go to the [Dynamics 365 Application Ideas portal](https://experience.dynamics.com/ideas/categories/?forum=79a8c474-4e35-e911-a971-000d3a4f3343&forumName=Dynamics%20365%20Customer%20Insights).</span></span>

## <a name="january-2021-updates"></a><span data-ttu-id="8ed3f-112">2021 年 1 月更新</span><span class="sxs-lookup"><span data-stu-id="8ed3f-112">January 2021 updates</span></span>

<span data-ttu-id="8ed3f-113">2021 年 1 月更新包含數個功能、效能升級和 BUG 修正。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-113">The updates in January 2021 include several features, performance upgrades, and bug fixes.</span></span>

#### <a name="extensibility"></a><span data-ttu-id="8ed3f-114">擴充性</span><span class="sxs-lookup"><span data-stu-id="8ed3f-114">Extensibility</span></span>

- <span data-ttu-id="8ed3f-115">**SFTP 匯出的擴充功能和增強效能** 您現在可以將 Customer Insights 的所有輸出實體匯出至 SFTP 主機。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-115">**Extended functionality and enhanced performance for SFTP export** You can now export all output entities from Customer Insights to an SFTP host.</span></span> <span data-ttu-id="8ed3f-116">先前，匯出會限制在客戶細分實體。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-116">Previously, export was limited to segment entities.</span></span> <span data-ttu-id="8ed3f-117">此外，SFTP 匯出的效能可讓您以較少的時間完成更多的資料量，視您的 SFTP 主機效能而定。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-117">Additionally, the performance of the SFTP export allows more data volume in less time, depending on the performance of your SFTP host.</span></span>    
  <span data-ttu-id="8ed3f-118">如需更多資訊，請見 [ SFTP 的連接器 (預覽版)](export-sftp.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-118">For more information, see [Connector for SFTP (preview)](export-sftp.md).</span></span>  

#### <a name="segments"></a><span data-ttu-id="8ed3f-119">客戶細分</span><span class="sxs-lookup"><span data-stu-id="8ed3f-119">Segments</span></span>

- <span data-ttu-id="8ed3f-120">**用機器學習支援建議的客戶細分以改善指標** 一種新的方式來探索並建立客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-120">**Machine learning powered suggested segments to improve metrics** There's a new way do discover and create segments.</span></span> <span data-ttu-id="8ed3f-121">系統會使用 AI 模型來建議客戶細分，這有助於改善正在追蹤的 KPI (量值)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-121">The system uses an AI model to suggest segments that can help improve a KPI (measure) you are already tracking.</span></span> <span data-ttu-id="8ed3f-122">我們會顯示您選取的屬性在量值或另一個主要屬性上的影響程度。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-122">We show the extent of influence of attributes that you select on a measure or another primary attribute.</span></span> <span data-ttu-id="8ed3f-123">此資訊可協助尋找存在商機的潛在客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-123">This information helps finding potential segments that present opportunities.</span></span>    
  <span data-ttu-id="8ed3f-124">如需更多資訊，請見[建議的客戶細分 (預覽版)](suggested-segments.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-124">For more information, see [Suggested segments (preview)](suggested-segments.md).</span></span>

#### <a name="data-unification"></a><span data-ttu-id="8ed3f-125">資料統整</span><span class="sxs-lookup"><span data-stu-id="8ed3f-125">Data unification</span></span>

- <span data-ttu-id="8ed3f-126">**增強的比對體驗** 在資料整合區域中，已更新比對體驗。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-126">**Enhanced match experience** In the data unification area, the match experience was updated.</span></span> <span data-ttu-id="8ed3f-127">它可讓您設定並查看比對規則，包括能進一步說明比對運作方式的統計詳細資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-127">It lets you configure and view the match rules, including detailed stats to further explain how matching works.</span></span> <span data-ttu-id="8ed3f-128">有一些選項可停用比對規則，所以在保留設定、拖放比對規則或更多作業時，它已不再可以使用。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-128">There are options to disable a match rule so it's no longer active while retaining the configuration, drag and drop match rules, and more.</span></span>
  <span data-ttu-id="8ed3f-129">如需詳細資訊，請參閱[比對實體](match-entities.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-129">For more information, see [Match entities](match-entities.md).</span></span>

- <span data-ttu-id="8ed3f-130">**來自比對程序中的重複資料刪除輸出可作為實體使用** 來自比對程序中的重複資料刪除輸出現在會寫入另一個實體中，提供進一步分析使用。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-130">**Deduplication output from the match process is available as an entity** Deduplication process output from the match process is now written into a separate entity for further analysis.</span></span> <span data-ttu-id="8ed3f-131">這個實體包含在重複資料刪除程序中使用的欄位，以及勝出記錄，以及與勝出記錄合併的對應替代記錄。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-131">This entity consists of the fields used in the deduplication process and the winner record and the corresponding alternate records that get merged with the winner record.</span></span>
  <span data-ttu-id="8ed3f-132">如需更多資訊，請見[重複資料刪除輸出實體](match-entities.md#deduplication-output-as-an-entity)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-132">For more information, see [Deduplication output as an entity](match-entities.md#deduplication-output-as-an-entity).</span></span>

#### <a name="system-administration"></a><span data-ttu-id="8ed3f-133">系統管理</span><span class="sxs-lookup"><span data-stu-id="8ed3f-133">System administration</span></span>

- <span data-ttu-id="8ed3f-134">**將資料無縫共用給 Microsoft Dataverse** 您現在可以使用 Microsoft Dataverse Managed Data Lake 共用 Customer Insights 輸出給 Microsoft Dataverse 應用程式。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-134">**Seamlessly share data to Microsoft Dataverse** You can now share Customer Insights output with Microsoft Dataverse applications using the Microsoft Dataverse Managed Data Lake.</span></span> <span data-ttu-id="8ed3f-135">在您將 Dataverse 環境與 Customer Insights 關聯之後，便有啟用資料共用的選項。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-135">Once you associate a Dataverse environment with Customer Insights, you get the option to enable data sharing.</span></span>
  <span data-ttu-id="8ed3f-136">如需詳細資訊，請參閱[管理環境](manage-environments.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-136">For more information, see [Manage environments](manage-environments.md).</span></span>


## <a name="december-2020-updates"></a><span data-ttu-id="8ed3f-137">2020 年 12 月更新</span><span class="sxs-lookup"><span data-stu-id="8ed3f-137">December 2020 updates</span></span>

<span data-ttu-id="8ed3f-138">2020 年 12 月的更新包括數項功能、效能升級和 BUG 修正。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-138">The updates in December 2020 include several features, performance upgrades, and bug fixes.</span></span>

### <a name="new-and-updated-features-in-december-2020"></a><span data-ttu-id="8ed3f-139">2020 年 12 月的全新和更新功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-139">New and updated features in December 2020</span></span>

#### <a name="data-enrichment"></a><span data-ttu-id="8ed3f-140">資料擴充</span><span class="sxs-lookup"><span data-stu-id="8ed3f-140">Data enrichment</span></span>

- <span data-ttu-id="8ed3f-141">**改善品牌與興趣親和度擴充**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-141">**Improved Brand and Interest affinity enrichments**</span></span>
  
  <span data-ttu-id="8ed3f-142">我們簡化了親合度分數，讓其更易於理解和使用。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-142">We simplified our affinity scores to make them easier to understand and use.</span></span> <span data-ttu-id="8ed3f-143">您現在可以來快速判斷客戶對指定品牌或興趣的親合度。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-143">You can now quickly identify customers based on how much affinity they have for a given brand or interest.</span></span>

  <span data-ttu-id="8ed3f-144">此外，我們新增了一些新的組態選項，以更好地控制您想要擴充客戶設定檔的方式。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-144">Additionally, we have added new configuration options to better control how you want your customer profiles to be enriched.</span></span> 

  <span data-ttu-id="8ed3f-145">如需詳細資訊，請參閱[使用品牌及興趣同質性擴充客戶設定檔](enrichment-microsoft-graph.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-145">For more information, see [Enrich customer profiles with brand and interest affinities](enrichment-microsoft-graph.md).</span></span>

- <span data-ttu-id="8ed3f-146">**控制要擴充的設定檔**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-146">**Control which profiles to enrich**</span></span>

  <span data-ttu-id="8ed3f-147">您現在可以只擴充客戶設定檔的一部分，而且有選項可以選取客戶細分實體而非預設客戶實體。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-147">You can now enrich only a subset of your customer profiles with the option to select a segment entity instead of the default customer entity.</span></span> <span data-ttu-id="8ed3f-148">用您想要擴充的客戶設定檔，建立一個客戶細分，並在您的客戶資料集的擴充設定中選取它。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-148">Create a segment with the customer profiles you would like to enrich and select it in the enrichment configuration for your customer data set.</span></span>
  <span data-ttu-id="8ed3f-149">此功能目前僅適用於 Experian 與 HERE Technologies 提供的擴充。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-149">This feature is currently available only for enrichments provided by Experian and HERE Technologies.</span></span> <span data-ttu-id="8ed3f-150">我們很快就會在更多擴充上推出這項功能。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-150">We will be enabling this capability to more enrichments soon.</span></span>

  <span data-ttu-id="8ed3f-151">如需詳細資訊，請參閱[使用 Experian 的人口統計來擴充客戶設定檔](enrichment-experian.md)或[用 HERE Technologies 來擴充客戶設定檔](enrichment-here.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-151">For more information, see [Enrich customer profiles with demographics from Experian](enrichment-experian.md) or [Enrichment of customer profiles with HERE Technologies](enrichment-here.md).</span></span>

#### <a name="extensibility"></a><span data-ttu-id="8ed3f-152">擴充性</span><span class="sxs-lookup"><span data-stu-id="8ed3f-152">Extensibility</span></span>

- <span data-ttu-id="8ed3f-153">**透過 Autopilot 啟動您的客戶細分**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-153">**Activate your segments through Autopilot**</span></span>

  <span data-ttu-id="8ed3f-154">將客戶細分匯出到 Autopilot 並使用在行銷目的上。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-154">Export segments to Autopilot and use them for marketing purposes.</span></span> <span data-ttu-id="8ed3f-155">如需更多資訊，請見 [Autopilot 的連接器 (預覽版)](export-autopilot.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-155">For more information, see [Connector for Autopilot (preview)](export-autopilot.md).</span></span>

- <span data-ttu-id="8ed3f-156">**透過 SendGrid 啟動您的客戶細分**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-156">**Activate your segments through SendGrid**</span></span>

  <span data-ttu-id="8ed3f-157">將客戶細分匯出到 SendGrid 並使用在行銷目的上。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-157">Export segments to SendGrid and use them for marketing purposes.</span></span> <span data-ttu-id="8ed3f-158">如需更多資訊，請見 [SendGrid 的連接器](export-sendgrid.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-158">For more information, see [Connector for SendGrid](export-sendgrid.md).</span></span>

#### <a name="system-administration"></a><span data-ttu-id="8ed3f-159">系統管理</span><span class="sxs-lookup"><span data-stu-id="8ed3f-159">System administration</span></span>

- <span data-ttu-id="8ed3f-160">**更新環境管理體驗**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-160">**Updated environment management experience**</span></span>
  
  <span data-ttu-id="8ed3f-161">您現在可以直接在環境選取器的標頭中建立、編輯、刪除及重設環境。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-161">You can now create, edit, delete, and reset environments directly from the environment picker in the app header.</span></span> 
  
  <span data-ttu-id="8ed3f-162">此外，您正在使用的環境將會釘選在環境面板的頂端，因此您不需要再搜尋它。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-162">Additionally, the environment you are using will be pinned at the top of the environment panel so you don't need to search for it anymore.</span></span>

  <span data-ttu-id="8ed3f-163">如需詳細資訊，請參閱[管理環境](manage-environments.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-163">For more information, see [Manage environments](manage-environments.md).</span></span>

## <a name="november-2020-updates"></a><span data-ttu-id="8ed3f-164">2020 年 11 月更新</span><span class="sxs-lookup"><span data-stu-id="8ed3f-164">November 2020 updates</span></span>

<span data-ttu-id="8ed3f-165">2020 年 11 月的更新包括數項功能、效能升級和 BUG 修正。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-165">The updates in November 2020 include several features, performance upgrades, and bug fixes.</span></span>

### <a name="new-and-updated-features-in-november-2020"></a><span data-ttu-id="8ed3f-166">2020 年 11 月的全新和更新功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-166">New and updated features in November 2020</span></span>

#### <a name="data-enrichment"></a><span data-ttu-id="8ed3f-167">資料擴充</span><span class="sxs-lookup"><span data-stu-id="8ed3f-167">Data enrichment</span></span>

- <span data-ttu-id="8ed3f-168">**透過安全檔案傳輸通訊協定 (SFTP) 自訂匯入您自己的富集資料**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-168">**Bring your own enrichment data via Secure File Transfer Protocol (SFTP) custom import**</span></span>
  
  <span data-ttu-id="8ed3f-169">SFTP 自訂匯入讓您無須經過資料整合程序便能匯入擴充資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-169">SFTP custom import lets you import enrichment data that doesn't have to go through the process of data unification.</span></span> <span data-ttu-id="8ed3f-170">了解更多關於 SFTP 自訂匯入。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-170">Learn more about SFTP custom import.</span></span>

  <span data-ttu-id="8ed3f-171">如需更多資訊，請見 [使用自訂資料富集客戶設定檔 (預覽版)](enrichment-SFTP-custom-import.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-171">For more information, see [Enrich customer profiles with custom data (preview)](enrichment-SFTP-custom-import.md).</span></span>
 
- <span data-ttu-id="8ed3f-172">**使用源自 HERE Technologies 的位置資料富集您的客戶資料**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-172">**Enrich your customer data with location data from HERE Technologies**</span></span>

  <span data-ttu-id="8ed3f-173">您可以使用 HERE Technologies 的資料富集服務建立對您客戶位址正規化、緯度和經度擷取等更精確的位置瞭解。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-173">With HERE Technologies' data enrichment services, you can build a more precise location understanding of your customers with address normalization, latitude and longitude extraction, and more.</span></span> <span data-ttu-id="8ed3f-174">了解更多關於使用 HERE Technologies 進行富集。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-174">Learn more about enriching with HERE Technologies.</span></span>

  <span data-ttu-id="8ed3f-175">如需更多資訊，請見 [使用 HERE Technologies 富集客戶設定檔](enrichment-here.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-175">For more information, see [Enrichment of customer profiles with HERE Technologies](enrichment-here.md).</span></span>

#### <a name="data-unification"></a><span data-ttu-id="8ed3f-176">資料統整</span><span class="sxs-lookup"><span data-stu-id="8ed3f-176">Data unification</span></span>

- <span data-ttu-id="8ed3f-177">**在選取實體上和您的儲存體帳戶欄位啟用資料剖析的彈性**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-177">**Flexibility to enable data profiling on selected entities and fields from your storage account**</span></span>

  <span data-ttu-id="8ed3f-178">您可以指出位於您的 Azure Data Lake Storage 帳戶中，您想要啟用資料內嵌流程其中一部分的資料剖析功能的 Common Data Model 資料實體和欄位。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-178">You can indicate which data entities and fields from a Common Data Model folder in your Azure Data Lake storage account you want to enable data profiling as part of the data ingestion process.</span></span>

  <span data-ttu-id="8ed3f-179">如需更多資訊，請見 [連接到 Common Data Model 資料夾](connect-common-data-model.md#connect-to-a-common-data-model-folder)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-179">For more information, see [Connect to a Common Data Model folder](connect-common-data-model.md#connect-to-a-common-data-model-folder).</span></span>

#### <a name="extensibility"></a><span data-ttu-id="8ed3f-180">擴充性</span><span class="sxs-lookup"><span data-stu-id="8ed3f-180">Extensibility</span></span>

- <span data-ttu-id="8ed3f-181">**透過 Google Ads 啟動您的區段**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-181">**Activate your segments through Google Ads**</span></span>

  <span data-ttu-id="8ed3f-182">將區段匯出到 Google Ads 對象清單並用在 Google Search、Google Display Network、YouTube 和 Gmail 上刊登廣告。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-182">Export segments from to Google Ads audience lists and use these lists to advertise on Google Search, Google Display Network, YouTube, and Gmail.</span></span> <span data-ttu-id="8ed3f-183">瞭解更多關於透過 Google Ads 啟動您的區段的資訊。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-183">Learn more about activating your segments through Google Ads.</span></span>

  <span data-ttu-id="8ed3f-184">如需更多資訊，請見 [Google Ads 連接器](export-google-ads.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-184">For more information, see [Connector for Google Ads](export-google-ads.md).</span></span>

- <span data-ttu-id="8ed3f-185">**透過 Marketo 啟動您的區段**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-185">**Activate your segments through Marketo**</span></span>

  <span data-ttu-id="8ed3f-186">將區段匯出到 Marketo 觀眾並使用這些對象進行行銷自動化。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-186">Export segments to Marketo audiences and use these audiences for marketing automation.</span></span> <span data-ttu-id="8ed3f-187">瞭解更多關於透過 Marketo 啟動您的區段的資訊。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-187">Learn more about activating your segments through Marketo.</span></span> 

  <span data-ttu-id="8ed3f-188">如需更多資訊，請見 [Marketo 連接器](export-marketo.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-188">For more information, see [Connector for Marketo](export-marketo.md).</span></span>

- <span data-ttu-id="8ed3f-189">**透過 DotDigital 啟動您的區段**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-189">**Activate your segments through DotDigital**</span></span>

  <span data-ttu-id="8ed3f-190">將區段匯出到 DotDigital 並用於行銷目的。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-190">Export segments to DotDigital and use them for marketing purposes.</span></span> <span data-ttu-id="8ed3f-191">瞭解更多關於透過 DotDigital 啟動您的區段的資訊。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-191">Learn more about activating your segments through DotDigital.</span></span> 

  <span data-ttu-id="8ed3f-192">如需更多資訊，請見 [DotDigital 連接器](export-dotdigital.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-192">For more information, see [Connector for DotDigital](export-dotdigital.md).</span></span>

#### <a name="predictions"></a><span data-ttu-id="8ed3f-193">預測</span><span class="sxs-lookup"><span data-stu-id="8ed3f-193">Predictions</span></span>

- <span data-ttu-id="8ed3f-194">**預測交易性流失**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-194">**Predict transactional churn**</span></span>

  <span data-ttu-id="8ed3f-195">交易流失預測功能讓您不需要資料科學家就能預測客戶停止購買產品或服務的可能性。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-195">The transaction churn prediction feature enables you, without the help of a data scientist, to predict the likelihood of a customer to stop purchasing products or services.</span></span>  <span data-ttu-id="8ed3f-196">您可以使用預測分數結合有關客戶的其他資訊，像是客戶價值，建立高流失風險或高價值客戶的區段。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-196">Using the prediction score, you can combine other information about your customers, like customer value, to create segments of high churn risk or high value customers.</span></span> <span data-ttu-id="8ed3f-197">使用此區段直接透過行銷活動、客戶支援及其他案例鎖定客戶的目標以降低流失風險。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-197">Use this segment to directly target customers through marketing activities, customer support, and other scenarios to reduce churn risk.</span></span>
 
  <span data-ttu-id="8ed3f-198">將流失的定義組態為您業務專屬的時間型視窗，定義客戶視同為已流失的時間點。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-198">Configure the definition of churn as a time-based window specific to your business and define when customers are considered churned.</span></span> <span data-ttu-id="8ed3f-199">例如假使雜貨店裡的顧客未能在過去 30 天內購買任何產品，雜貨店可能想認定已流失客戶。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-199">For example, a grocery store may want to consider a customer churned if they have not purchased anything in the past 30 days.</span></span>
 
  <span data-ttu-id="8ed3f-200">由於您繼續建立預測，因此我們將引導您掌握需要的資料，並讓您將有關業務的資料對應到需預測您客戶流失的欄位。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-200">As you continue creating the prediction, we'll guide you what data is needed, and enable you to map data about your business to fields required to predict churn for your customers.</span></span> <span data-ttu-id="8ed3f-201">您也可以根據系統中的新資訊設定排程重新培養模型，以適應不斷變動的業務環境。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-201">You can also set a schedule to retrain the model based on new information in your system to adapt to changing business circumstances.</span></span>
 
  <span data-ttu-id="8ed3f-202">如需更多資訊，請見 [交易性流失預測 (預覽版)](predict-transactional-churn.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-202">For more information, see [Transactional churn prediction (preview)](predict-transactional-churn.md).</span></span>

#### <a name="system-administration"></a><span data-ttu-id="8ed3f-203">系統管理</span><span class="sxs-lookup"><span data-stu-id="8ed3f-203">System administration</span></span>

- <span data-ttu-id="8ed3f-204">**重設環境**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-204">**Reset environment**</span></span>

  <span data-ttu-id="8ed3f-205">將選取執行個體環境中的一切重新設定為開始重新整理。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-205">Reset everything in an environment of a selected instance to start fresh.</span></span>

  <span data-ttu-id="8ed3f-206">如需更多資訊，請見 [重新設定現有環境](manage-environments.md#reset-an-existing-environment)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-206">For more information, see [Reset an existing environment](manage-environments.md#reset-an-existing-environment).</span></span>


- <span data-ttu-id="8ed3f-207">**使用服務主體連接到您的 Azure Data Lake Storage 帳戶**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-207">**Connect to your Azure Data Lake storage account using a service principal**</span></span>

  <span data-ttu-id="8ed3f-208">使用 Azure 服務主體將資料輸出寫入您的儲存體帳戶並讀取資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-208">Write data output to and read data from your storage account using an Azure service principal.</span></span> <span data-ttu-id="8ed3f-209">現有儲存體帳戶連接可繼續使用帳戶金鑰。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-209">Existing storage account connections can continue to use the account key.</span></span> <span data-ttu-id="8ed3f-210">它們也會提供升級選項，以便繼續使用服務主體。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-210">They also offer an upgrade option to use the service principal moving forward.</span></span> <span data-ttu-id="8ed3f-211">新連接將根據您的儲存體帳戶服務主體驗證方法進行。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-211">New connections will be based on the service principal authentication method for your storage account.</span></span>

  <span data-ttu-id="8ed3f-212">更多資訊請見 [使用 Azure 服務主體對象見解連接到 Azure Data Lake Storage Gen2 帳戶](connect-service-principal.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-212">For more information, see [Connect to an Azure Data Lake Storage Gen2 account with an Azure service principal for audience insights](connect-service-principal.md).</span></span>

## <a name="october-2020-updates"></a><span data-ttu-id="8ed3f-213">2020 年 10 月更新</span><span class="sxs-lookup"><span data-stu-id="8ed3f-213">October 2020 updates</span></span>

<span data-ttu-id="8ed3f-214">2020 年 10 月的更新包括數項功能、效能升級和 BUG 修正。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-214">The updates in October 2020 include several features, performance upgrades, and bug fixes.</span></span>

### <a name="new-and-updated-features-in-october-2020"></a><span data-ttu-id="8ed3f-215">2020 年 10 月的全新和更新功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-215">New and updated features in October 2020</span></span>

#### <a name="extensibility"></a><span data-ttu-id="8ed3f-216">擴充性</span><span class="sxs-lookup"><span data-stu-id="8ed3f-216">Extensibility</span></span>

- <span data-ttu-id="8ed3f-217">**匯出到 Mailchimp**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-217">**Export to Mailchimp**</span></span>

<span data-ttu-id="8ed3f-218">將區段匯出到 Mailchimp 中的現有對象清單，以便為您的客戶提供個人化的電子郵件體驗。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-218">Export segments to existing audience lists in Mailchimp to provide a personalized email experience for your customers.</span></span>

<span data-ttu-id="8ed3f-219">如需更多資訊，請見 [Mailchimp 連接器](export-mailchimp.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-219">For more information, see [Connector for Mailchimp](export-mailchimp.md).</span></span>

#### <a name="data-enrichment"></a><span data-ttu-id="8ed3f-220">資料擴充</span><span class="sxs-lookup"><span data-stu-id="8ed3f-220">Data enrichment</span></span>

- <span data-ttu-id="8ed3f-221">**重複資料刪除比對實體中的來源記錄**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-221">**Deduplicate the source records in a Match entity**</span></span>

<span data-ttu-id="8ed3f-222">針對比對流程使用的實體指定重複資料刪除規則，以便找出重複記錄。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-222">Specify deduplication rules on entities used in the match process to identify duplicate records.</span></span> <span data-ttu-id="8ed3f-223">將它們合併為一筆記錄並將所有來源記錄連結到此合併記錄。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-223">Merge them into one record and link all the source records to this merged record.</span></span> <span data-ttu-id="8ed3f-224">接著這筆重複遭刪除的記錄將用在跨實體比對流程。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-224">This deduplicated record will then be used in the cross-entity matching process.</span></span>

<span data-ttu-id="8ed3f-225">如需更多資訊，請見 [定義比對實體的重複資料刪除](match-entities.md#define-deduplication-on-a-match-entity)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-225">For more information, see [Define deduplication on a match entity](match-entities.md#define-deduplication-on-a-match-entity).</span></span>

#### <a name="system-administration"></a><span data-ttu-id="8ed3f-226">系統管理</span><span class="sxs-lookup"><span data-stu-id="8ed3f-226">System administration</span></span>

- <span data-ttu-id="8ed3f-227">**協調流程：Merge 中的新重新整理選項**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-227">**Orchestration: New refresh option in Merge**</span></span>

<span data-ttu-id="8ed3f-228">截至今天為止，當您執行合併流程時，系統已執行過所有以合併及後續流程為主的下游流程。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-228">Until today, when you run the merge process, the system ran all the downstream processes that depend on merge and subsequent processes.</span></span> <span data-ttu-id="8ed3f-229">您現在可以審核合併流程 (統整的客戶實體) 的輸出，再將它用在下游處理像是區段或量值。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-229">You can now verify the output of the merge process (the unified customer entity) before using it in downstream processing like segments or measures.</span></span>
<span data-ttu-id="8ed3f-230">您現在可以在合併頁面上選擇只執行合併步驟及此道流程。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-230">On the merge page, you can now choose to run only the merge step and run only this process.</span></span> <span data-ttu-id="8ed3f-231">若是也要重新整理所有下游流程，您可以選擇執行合併和下游流程。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-231">To refresh all the downstream processes too, you can choose run merge and downstream processes.</span></span> 

## <a name="september-2020-updates"></a><span data-ttu-id="8ed3f-232">2020 年 9 月更新</span><span class="sxs-lookup"><span data-stu-id="8ed3f-232">September 2020 updates</span></span>

<span data-ttu-id="8ed3f-233">2020 年 9 月更新包含數項功能、效能升級和 BUG 修正。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-233">The updates in September 2020 include several features, performance upgrades, and bug fixes.</span></span>

### <a name="new-and-updated-features-in-september-2020"></a><span data-ttu-id="8ed3f-234">2020 年 9 月的新增及更新功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-234">New and updated features in September 2020</span></span>

#### <a name="activities"></a><span data-ttu-id="8ed3f-235">活動</span><span class="sxs-lookup"><span data-stu-id="8ed3f-235">Activities</span></span>

- <span data-ttu-id="8ed3f-236">**屬性語意智慧預測**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-236">**Intelligent prediction of attribute semantics**</span></span>

<span data-ttu-id="8ed3f-237">這項新功能可預測傳遞給資料統合程序的輸入屬性語意類型。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-237">This new feature predicts the semantic types of input attributes that are passed on to the data unification process.</span></span> <span data-ttu-id="8ed3f-238">採用可改善準確性和節省時間的機器學習模型。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-238">It uses machine learning models that improve accuracy and save time.</span></span>

#### <a name="enrichments"></a><span data-ttu-id="8ed3f-239">擴充</span><span class="sxs-lookup"><span data-stu-id="8ed3f-239">Enrichments</span></span>

- <span data-ttu-id="8ed3f-240">**Experian 的人口統計擴充內容**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-240">**Demographics enrichment from Experian**</span></span>

<span data-ttu-id="8ed3f-241">Experian 的人口統計擴充內容現已開放預覽。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-241">The demographics enrichment from Experian is now available in preview.</span></span> <span data-ttu-id="8ed3f-242">Experian 是消費者與企業信用報告以及行銷服務的全球領導者。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-242">Experian is a global leader in consumer and business credit reporting and marketing services.</span></span> <span data-ttu-id="8ed3f-243">有了 [Experian 的資料擴充服務](https://www.experian.com/marketing-services/microsoft?cmpid=ems_web_mci_cdppage)，您就可以透過人口統計資料 (例如家庭人數、收入及其他) 擴充您的客戶設定檔，加深對客戶的了解。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-243">With [Experian’s data enrichment services](https://www.experian.com/marketing-services/microsoft?cmpid=ems_web_mci_cdppage), you can build a deeper understanding of your customers by enriching your customer profiles with demographic data such as household size, income, and more.</span></span>

<span data-ttu-id="8ed3f-244">若要使用此功能，您必須已加入有效的 Experian 訂閱。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-244">To use this feature, you must have an active Experian subscription.</span></span>

<span data-ttu-id="8ed3f-245">如需詳細資訊，請參閱[使用 Experian 提供的人口統計資料擴充客戶設定檔](enrichment-experian.md)</span><span class="sxs-lookup"><span data-stu-id="8ed3f-245">For more information, see [Enrich customer profiles with demographics from Experian](enrichment-experian.md)</span></span>


#### <a name="system-administration"></a><span data-ttu-id="8ed3f-246">系統管理</span><span class="sxs-lookup"><span data-stu-id="8ed3f-246">System administration</span></span>

- <span data-ttu-id="8ed3f-247">**工作詳細資料窗格**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-247">**Task details pane**</span></span>

<span data-ttu-id="8ed3f-248">工作詳細資料窗格可讓您查看有關系統所執行工作的詳細資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-248">The task details pane enables you to see details about tasks that the system runs.</span></span> <span data-ttu-id="8ed3f-249">這是識別問題和尋找解決方案的便捷方式。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-249">It's a handy way to identify issues with the configuration and find solutions.</span></span>
<span data-ttu-id="8ed3f-250">檢閱錯誤訊息，以了解如何處理潛在問題。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-250">Review the error messages see how you address potential issues.</span></span>
 
- <span data-ttu-id="8ed3f-251">**將處理中的資訊新增至更多頁面**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-251">**Processing information added to more pages**</span></span>

<span data-ttu-id="8ed3f-252">這項改善會在 **實體** 和 **客戶** 頁面上新增有關實體狀態的資訊。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-252">This improvement adds information about the status of your entities on the **Entities** and **Customers** page.</span></span>
 
<span data-ttu-id="8ed3f-253">此外，您還可以在這兩個頁面上找到有關處理進度的詳細資訊，以及工作詳細資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-253">Additionally, you can find details about the progress of processes, along with the task details, on both of these pages.</span></span>

- <span data-ttu-id="8ed3f-254">**系統狀態頁面的改善**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-254">**Improvements to system status page**</span></span>

<span data-ttu-id="8ed3f-255">我們已改進 **系統** > **狀態** 上的狀態詳細資料表格在檢閱資料匯出時的結構。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-255">We improved the structure of the status details table on **System** > **Status** when reviewing data exports.</span></span>
 
<span data-ttu-id="8ed3f-256">此外，**詳細資料** 欄中的錯誤現在更加詳細且可操作。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-256">Additionally, errors in the **Details** column are now more detailed and actionable.</span></span> 
 
- <span data-ttu-id="8ed3f-257">**取消將工作還原為先前狀態**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-257">**Cancel reverts job back to previous state**</span></span>

<span data-ttu-id="8ed3f-258">取消工作時 (例如，在比對程序中)，工作會還原為其最近一次的狀態。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-258">When you cancel a task, for example, in the match process, it will revert back to its latest state.</span></span> <span data-ttu-id="8ed3f-259">例如，如果比對程序在昨天完成，而您今天將其取消，則此工作會還原為昨天的成功狀態。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-259">For example, if the Match process completed yesterday and you cancel it today, it will revert to yesterday's successful state.</span></span>


## <a name="august-2020-updates"></a><span data-ttu-id="8ed3f-260">2020 年 8 月更新</span><span class="sxs-lookup"><span data-stu-id="8ed3f-260">August 2020 updates</span></span>

<span data-ttu-id="8ed3f-261">2020 年 8 月更新包含數項功能、效能升級和 BUG 修正。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-261">The updates in August 2020 include several features, performance upgrades, and bug fixes.</span></span>

### <a name="new-and-updated-features-in-august-2020"></a><span data-ttu-id="8ed3f-262">2020 年 8 月的新增及更新功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-262">New and updated features in August 2020</span></span>

#### <a name="data-unification"></a><span data-ttu-id="8ed3f-263">資料統整</span><span class="sxs-lookup"><span data-stu-id="8ed3f-263">Data unification</span></span>

- <span data-ttu-id="8ed3f-264">**改善資料統合期間對應階段的體驗**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-264">**Improved experience for the map stage during data unification**</span></span>

  <span data-ttu-id="8ed3f-265">資料統合程序中對應階段的體驗可讓您選取實體、屬性，並以更加流暢的方式來定義語意。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-265">The experience to the map stage in the data unification process lets you select entities, attributes, and define semantics in a more seamless way.</span></span>

  <span data-ttu-id="8ed3f-266">這些變更包括：</span><span class="sxs-lookup"><span data-stu-id="8ed3f-266">The changes include:</span></span>
  
  - <span data-ttu-id="8ed3f-267">新增實體與欄位所需的互動較少</span><span class="sxs-lookup"><span data-stu-id="8ed3f-267">fewer interactions required to add entities and fields</span></span>
  - <span data-ttu-id="8ed3f-268">改善對應頁面上的搜尋功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-268">improved search capabilities on the map page</span></span>
  - <span data-ttu-id="8ed3f-269">直觀且易於識別建議的欄位類型</span><span class="sxs-lookup"><span data-stu-id="8ed3f-269">visual and easy identification of the suggested field type</span></span>

#### <a name="enrichment"></a><span data-ttu-id="8ed3f-270">擴充</span><span class="sxs-lookup"><span data-stu-id="8ed3f-270">Enrichment</span></span>

- <span data-ttu-id="8ed3f-271">**興趣親合度擴充在更多市場提供**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-271">**Interest affinities enrichment available in more markets**</span></span>

  <span data-ttu-id="8ed3f-272">在美國之外，我們增加了其他五個市場到興趣親合度擴充的使用範圍：加拿大、澳大利亞、英國、法國和德國。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-272">We're extending the availability of the interest affinities enrichment beyond the United States to five other markets: Canada, Australia, United Kingdom, France, and Germany.</span></span> <span data-ttu-id="8ed3f-273">使用此項新增，您可以用更多適用於這些市場的興趣擴充您的客戶資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-273">With this extension, you can enrich your customer data with more interests applicable to these markets.</span></span> <span data-ttu-id="8ed3f-274">我們也會使用 Microsoft Graph 的當地專有資料專，擴充您位於這些市場的客戶設定檔。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-274">We'll also enrich your customer profiles that are located in these markets by using local proprietary data from Microsoft Graph.</span></span>
  <span data-ttu-id="8ed3f-275">如需詳細資訊，請參閱[使用品牌及興趣同質性擴充客戶設定檔](enrichment-microsoft-graph.md)</span><span class="sxs-lookup"><span data-stu-id="8ed3f-275">For more information, see [Enrich customer profiles with brand and interest affinities](enrichment-microsoft-graph.md)</span></span>


## <a name="july-2020-updates"></a><span data-ttu-id="8ed3f-276">2020 年 7 月更新</span><span class="sxs-lookup"><span data-stu-id="8ed3f-276">July 2020 updates</span></span>

<span data-ttu-id="8ed3f-277">2020 年 7 月更新包含數項功能、效能升級和 BUG 修正。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-277">The updates in July 2020 include several features, performance upgrades, and bug fixes.</span></span>

### <a name="new-and-updated-features-in-july-2020"></a><span data-ttu-id="8ed3f-278">2020 年 7 月的新增及更新功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-278">New and updated features in July 2020</span></span>

#### <a name="extensibility"></a><span data-ttu-id="8ed3f-279">擴充性</span><span class="sxs-lookup"><span data-stu-id="8ed3f-279">Extensibility</span></span>

- <span data-ttu-id="8ed3f-280">**已完成的統整程序的 Power Automate 觸發程序**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-280">**Power Automate trigger for completed unification process**</span></span>

  <span data-ttu-id="8ed3f-281">我們已擴充 Power Automate 的觸發程序，並且允許您在統整程序 (對應、比對、合併) 重新整理完成時，建立通知或動作。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-281">We have extended our triggers for Power Automate and let you create a notification or action when a refresh of the unification process (map, match, merge) is completed.</span></span>    
  <span data-ttu-id="8ed3f-282">如需詳細資訊，請參閱[Power Automate 連接器](export-power-automate.md)</span><span class="sxs-lookup"><span data-stu-id="8ed3f-282">For more information, see [Power Automate connector](export-power-automate.md)</span></span>

#### <a name="enrichment"></a><span data-ttu-id="8ed3f-283">擴充</span><span class="sxs-lookup"><span data-stu-id="8ed3f-283">Enrichment</span></span>

- <span data-ttu-id="8ed3f-284">**品牌親合度擴充在更多市場提供**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-284">**Brand affinities enrichment available in more markets**</span></span>

  <span data-ttu-id="8ed3f-285">在美國之外，我們增加了其他五個市場到品牌親合度擴充的使用範圍：加拿大、澳大利亞、英國、法國和德國。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-285">We're extending the availability of the brand affinities enrichment beyond the United States to five other markets: Canada, Australia, United Kingdom, France, and Germany.</span></span> <span data-ttu-id="8ed3f-286">隨著此次延伸，您可以使用這些市場中的當地品牌來擴充客戶資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-286">With this extension, you can enrich your customer data with local brands in these markets.</span></span> <span data-ttu-id="8ed3f-287">我們也會使用 Microsoft Graph 的當地專有資料專，擴充您位於這些市場的客戶設定檔。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-287">We'll also enrich your customer profiles that are located in these markets by using local proprietary data from Microsoft Graph.</span></span>
  <span data-ttu-id="8ed3f-288">如需詳細資訊，請參閱[使用品牌及興趣同質性擴充客戶設定檔](enrichment-microsoft-graph.md)</span><span class="sxs-lookup"><span data-stu-id="8ed3f-288">For more information, see [Enrich customer profiles with brand and interest affinities](enrichment-microsoft-graph.md)</span></span>

## <a name="june-2020-updates"></a><span data-ttu-id="8ed3f-289">2020 年 6 月更新</span><span class="sxs-lookup"><span data-stu-id="8ed3f-289">June 2020 updates</span></span>

<span data-ttu-id="8ed3f-290">2020 年 6 月更新包含數項功能、效能升級和 BUG 修正。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-290">The updates in June 2020 include several features, performance upgrades, and bug fixes.</span></span>

### <a name="new-and-updated-features-in-june-2020"></a><span data-ttu-id="8ed3f-291">2020 年 6 月的新增及更新功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-291">New and updated features in June 2020</span></span>

#### <a name="enrichment"></a><span data-ttu-id="8ed3f-292">擴充</span><span class="sxs-lookup"><span data-stu-id="8ed3f-292">Enrichment</span></span>

- <span data-ttu-id="8ed3f-293">**Leadspace 提供的公司資料擴充**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-293">**Enrichment with company data from Leadspace**</span></span>
  
  <span data-ttu-id="8ed3f-294">定義統整客戶設定檔中的欄位，這些欄位可用來向 Leadspace 查詢相關的公司資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-294">Define fields in unified customer profiles that are used to look up related company data from Leadspace.</span></span> <span data-ttu-id="8ed3f-295">執行擴充程序之後，B2B 設定檔會擴充更多屬性，包括公司大小、地點、產業等等。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-295">After running the enrichment process, B2B profiles are enriched with more attributes including company size, location, industry, and more.</span></span>    
  <span data-ttu-id="8ed3f-296">此共同作業可讓您利用協力廠商服務提供的資訊來改善資料品質。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-296">This collaboration allows you to improve the quality of your data with input from third-party services.</span></span> <span data-ttu-id="8ed3f-297">若要使用此擴充內容，您需要 Leadspace 的授權，才能存取其 B2B 公司資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-297">To use this enrichment, you'll need a license from Leadspace to access its B2B company data.</span></span> <span data-ttu-id="8ed3f-298">系統將使用該授權保持您的資料不斷富集。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-298">The system will use that license to keep your data enriched continuously.</span></span>    
  <span data-ttu-id="8ed3f-299">如需詳細資訊，請參閱 [使用 Leadspace 的公司設定檔擴充](enrichment-leadspace.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-299">For more information, see [Enrichment of company profiles with Leadspace](enrichment-leadspace.md).</span></span>

- <span data-ttu-id="8ed3f-300">**擴充中心頁面**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-300">**Enrichment hub page**</span></span>

  <span data-ttu-id="8ed3f-301">第一方和第三方擴充內容提供者的所有可用資料擴充都是在同一個位置進行設定。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-301">All available data enrichment from first- and third-party enrichment providers gets configured in the same place.</span></span> <span data-ttu-id="8ed3f-302">設定資料擴充是從共同位置管理的順暢體驗。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-302">Configuring data enrichment is a seamless experience that is managed from a common place.</span></span>    
  <span data-ttu-id="8ed3f-303">如需詳細資訊，請參閱[客戶設定檔的擴充](enrichment-hub.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-303">For more information, see [Enrichment for customer profiles](enrichment-hub.md).</span></span>

- <span data-ttu-id="8ed3f-304">**個別品牌及興趣同質性擴充**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-304">**Separate brand and interest affinity enrichment**</span></span>

  <span data-ttu-id="8ed3f-305">品牌及興趣同質性現在可當做兩個獨立的擴充內容來使用。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-305">The brands and interests affinities are now available as two independent enrichments.</span></span> <span data-ttu-id="8ed3f-306">分開的擴充內容可讓您靈活地根據業務需求或需要個別加以設定和管理。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-306">Separated enrichments give you the flexibility to configure and manage them individually, depending on your business requirements or needs.</span></span>    
  <span data-ttu-id="8ed3f-307">如需詳細資訊，請參閱[使用品牌及興趣同質性擴充客戶設定檔](enrichment-microsoft-graph.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-307">For more information, see [Enrich customer profiles with brand and interest affinities](enrichment-microsoft-graph.md).</span></span>

#### <a name="extensibility"></a><span data-ttu-id="8ed3f-308">擴充性</span><span class="sxs-lookup"><span data-stu-id="8ed3f-308">Extensibility</span></span>

- <span data-ttu-id="8ed3f-309">**Dynamics 365 Customer 卡片增益集上的統整活動的可點選 URL**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-309">**Clickable URLs for unified activities on the Dynamics 365 Customer Card Add-in**</span></span>

  <span data-ttu-id="8ed3f-310">如果活動組態期間已定義此類 URL，則客戶卡增益集中的統整活動現在就會顯示可點按的 URL。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-310">The unified activities in the Customer Card Add-in are now showing clickable URLs if such URLs have been defined during the configuration of activities.</span></span>    
  <span data-ttu-id="8ed3f-311">如需詳細資訊，請參閱[客戶卡片增益集](customer-card-add-in.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-311">For more information, see [Customer Card Add-in](customer-card-add-in.md).</span></span>

- <span data-ttu-id="8ed3f-312">**Dynamics 365 客戶卡片增益集中可用的品牌及興趣同質性**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-312">**Brand and interest affinities available on the Dynamics 365 Customer Card Add-in**</span></span>

  <span data-ttu-id="8ed3f-313">Dynamics 365 客戶卡片增益集的新控制項可讓您在 Dynamics 365 的客戶參與應用程式中顯示有關連絡人的品牌及興趣擴充內容。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-313">A new control on the Dynamics 365 Customer Card Add-in lets you show brand and interest enrichments on your contacts in customer engagement apps in Dynamics 365.</span></span>    
  <span data-ttu-id="8ed3f-314">如需詳細資訊，請參閱[客戶卡片增益集](customer-card-add-in.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-314">For more information, see [Customer Card Add-in](customer-card-add-in.md).</span></span>

- <span data-ttu-id="8ed3f-315">**更多 Power Automate 觸發程序**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-315">**More Power Automate triggers**</span></span>

  <span data-ttu-id="8ed3f-316">我們已擴充 Power Automate 的觸發程序，並新增下列觸發程序：</span><span class="sxs-lookup"><span data-stu-id="8ed3f-316">We have extended our triggers for Power Automate and added the following triggers:</span></span>
  - <span data-ttu-id="8ed3f-317">在自動化完整重新整理 (資料來源、統整、客戶細分、量值、匯出) 完成時，取得通知或執行動作</span><span class="sxs-lookup"><span data-stu-id="8ed3f-317">Get a notification or perform an action when an automated full refresh (data sources, unification, segments, measures, exports) completes</span></span>
  - <span data-ttu-id="8ed3f-318">定義業務量值的閾值。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-318">Define a threshold for a business measure.</span></span> <span data-ttu-id="8ed3f-319">例如，您可以建立會在越過定義的閾值時傳送的通知。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-319">For example, you can create a notification that gets sent when the defined threshold is passed.</span></span> <span data-ttu-id="8ed3f-320">此外，觸發程序還會提供可讓您在 Power Automate 中建置更複雜工作流程的資訊 。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-320">Additionally, the trigger brings information that allows you to build more complex workflows in Power Automate.</span></span>    
  <span data-ttu-id="8ed3f-321">如需詳細資訊，請參閱[Power Automate 連接器](export-power-automate.md)</span><span class="sxs-lookup"><span data-stu-id="8ed3f-321">For more information, see [Power Automate connector](export-power-automate.md)</span></span>

- <span data-ttu-id="8ed3f-322">**匯出至 Facebook 廣告管理員**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-322">**Export to Facebook Ads Manager**</span></span>
  
  <span data-ttu-id="8ed3f-323">此功能讓您將區段匯出到 Facebook Ads 管理員。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-323">This capability lets you export segments to Facebook Ads Manager.</span></span> <span data-ttu-id="8ed3f-324">區段匯出為自訂對象，在 Facebook 行銷廣告活動和廣告中使用統整的客戶設定檔。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-324">Segments are exported as custom audiences to use unified customer profiles in Facebook marketing campaigns and ads.</span></span> <span data-ttu-id="8ed3f-325">自訂對象也適用在 Instagram 中透過 Facebook 廣告管理員建立行銷活動。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-325">The custom audiences are also usable to create campaigns on Instagram through Facebook Ads Manager.</span></span>    
  <span data-ttu-id="8ed3f-326">如需詳細資訊，請參閱 [Facebook 廣告管理員的連接器](export-facebook.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-326">For more information, see [Connector for Facebook Ads Manager](export-facebook.md).</span></span>

#### <a name="predictions"></a><span data-ttu-id="8ed3f-327">預測</span><span class="sxs-lookup"><span data-stu-id="8ed3f-327">Predictions</span></span>

- <span data-ttu-id="8ed3f-328">**訂閱流失預測**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-328">**Subscription churn prediction**</span></span>

  <span data-ttu-id="8ed3f-329">遵循引導式體驗，在雲端服務、客戶成員資格和其他部門等訂閱區域中建立流失預測。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-329">Follow a guided experience to create churn prediction in subscription areas like cloud services, customer membership, and other sectors.</span></span> 

  <span data-ttu-id="8ed3f-330">訂閱流失預測功能，讓您不聘用資料科學家，也能預測客戶停止使用訂閱型產品或服務的可能性。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-330">The subscription churn prediction feature enables you to predict the likelihood of a customer stopping the use of subscription-based products or services without engaging a data scientist.</span></span> <span data-ttu-id="8ed3f-331">您可以使用預測分數，結合客戶的其他相關資訊來建立高流失風險的客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-331">Using the prediction score, you can combine other information about your customers to create segments of high churn risk.</span></span> <span data-ttu-id="8ed3f-332">藉助此區段，您可以直接鎖定行銷客戶、客戶支援及其他案例，減少特定客戶改善營收和降低成本產生的流失風險。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-332">With the help of this segment, you can directly target customers in marketing, customer support, and other scenarios to reduce the risk of churn for specific customers to improve revenue and reduce cost.</span></span>

  <span data-ttu-id="8ed3f-333">在此體驗中，您可以將流失的定義設定為適合特定業務的時間範圍。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-333">Within the experience, you can configure the definition of churn as a time-based window specific to your business.</span></span> <span data-ttu-id="8ed3f-334">例如，具有每月訂閱程序的視訊串流業務可能需要在客戶訂閱到期後 15 天過後，將該客戶視為已流失。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-334">For example, a video streaming business that has a monthly subscription process might want to consider a customer to have churned after 15 days after the expiration of their subscription.</span></span>

  <span data-ttu-id="8ed3f-335">當您繼續進行預測時，我們將引導您瀏覽所需的資料，並讓您可以將業務相關資料對應至需要預測客戶流失的欄位。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-335">As you continue through the prediction, we'll guide you through what data is needed, and enable you to map data about your business to fields required to predict churn for your customers.</span></span> <span data-ttu-id="8ed3f-336">業務資訊變更時，您也可以設定排程，根據系統中的新資訊重新定型，以適應不斷變化的業務環境。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-336">As business information changes, you can also set a schedule to retrain on new information in your system to adapt to changing business circumstances.</span></span>    
  <span data-ttu-id="8ed3f-337">如需詳細資訊，請參閱[訂閱流失預測 (預覽)](predict-subscription-churn.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-337">For more information, see [Subscription churn prediction (preview)](predict-subscription-churn.md).</span></span>

#### <a name="segments"></a><span data-ttu-id="8ed3f-338">客戶細分</span><span class="sxs-lookup"><span data-stu-id="8ed3f-338">Segments</span></span>

- <span data-ttu-id="8ed3f-339">**尋找類似的客戶**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-339">**Find similar customers**</span></span>
  
  <span data-ttu-id="8ed3f-340">使用人工智慧，在您的客戶群中尋找類似的客戶。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-340">Find similar customers in your customer base using artificial intelligence.</span></span> <span data-ttu-id="8ed3f-341">二元分類機器學習模型會將相似性分數指派給展開的客戶細分中的客戶。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-341">A binary classification machine learning model assigns a similarity score to customers in the expanded segment.</span></span> <span data-ttu-id="8ed3f-342">分數是根據與來源客戶細分中客戶的相似性所建立。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-342">The score is based on the similarity to customers in the source segment.</span></span> <span data-ttu-id="8ed3f-343">客戶設定檔會根據相似性分數新增至新建立的客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-343">Depending on the similarity score, customer profiles are added to a newly created segment.</span></span>

  <span data-ttu-id="8ed3f-344">有時在數位行銷中稱為相似模型，它使用 AI 模型來協助加入更多屬性尋找與其他客戶細分相似的客戶。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-344">Sometimes referred to as lookalike modeling in digital marketing, it uses an AI model to help find customers who are similar to another segment of your customers by factoring in more attributes.</span></span> <span data-ttu-id="8ed3f-345">不僅可讓您選擇屬性，也允許您指定這個新的客戶細分中應有的客戶數目上限。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-345">It not only allows you to pick the attributes but also allows you to specify the maximum number of customers who should be in this new segment.</span></span> <span data-ttu-id="8ed3f-346">AI 模型接著根據您選取的屬性計算每個客戶的相似性分數，並尋找相似性分數高於平均值的客戶。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-346">The AI model will then compute similarity scores for each customer based on your selected attributes and find customers with the higher average similarity score.</span></span> <span data-ttu-id="8ed3f-347">產生的客戶細分將會包含看起來與原始客戶細分中客戶相似的客戶。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-347">The resulting segment will include customers who look similar to the customer in your original segment.</span></span>    
  <span data-ttu-id="8ed3f-348">如需詳細資訊，請參閱[類似客戶](find-similar-customer-segments.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-348">For more information, see [Similar Customers](find-similar-customer-segments.md).</span></span>

- <span data-ttu-id="8ed3f-349">**客戶細分重疊和區別因素**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-349">**Segment overlap and differentiators**</span></span>

  <span data-ttu-id="8ed3f-350">客戶細分重疊可讓您了解兩個或多個客戶細分有多少共同的客戶，以及有哪些共同客戶。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-350">Segment overlap lets you see how many and which customers are common to two or more segments.</span></span> <span data-ttu-id="8ed3f-351">例如，高消費者客戶細分與高滿意度客戶細分的重疊情形，或是客戶流失客戶細分與低滿意度客戶細分的重疊情形。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-351">For example, how a high-spenders segment overlaps with a high-satisfaction customers segment or how a churning customer segment overlaps with a low-satisfaction customers segment.</span></span> <span data-ttu-id="8ed3f-352">此外，您也可以根據選擇的額外屬性，分析重疊如何變化。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-352">Additionally, you can analyze how the overlap changes based on an extra attribute of your choice.</span></span>

  <span data-ttu-id="8ed3f-353">客戶細分區別因素揭示一個客戶細分與其餘客戶或其他客戶細分有什麼區別。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-353">Segment differentiators reveal what differentiates one segment from the rest of your customers or from another segment.</span></span> <span data-ttu-id="8ed3f-354">您所要做的只是識別客戶細分，系統就會找出區分客戶細分的設定檔屬性及量值，其形式為區別因素的排名清單，從最強至最弱列出這些區別因素。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-354">All you need to do is identify a segment and the system will identify profile attributes and measures that distinguish the segment in the form of a ranked list of differentiators—from the strongest differentiator to the weakest.</span></span>    
  <span data-ttu-id="8ed3f-355">如需詳細資訊，請參閱[客戶細分見解 (預覽)](segment-insights.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-355">For more information, see [Segment insights (preview)](segment-insights.md).</span></span>

- <span data-ttu-id="8ed3f-356">**客戶細分存留期**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-356">**Segment lifetime**</span></span>
  
  <span data-ttu-id="8ed3f-357">定義排程，以啟用或停用客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-357">Define a schedule to activate or deactivate a segment.</span></span>    
  <span data-ttu-id="8ed3f-358">如需詳細資訊，請參閱[管理現有的客戶細分](segments.md#manage-existing-segments)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-358">For more information, see [Manage existing segments](segments.md#manage-existing-segments).</span></span>

## <a name="may-2020-updates"></a><span data-ttu-id="8ed3f-359">2020 年 5 月更新</span><span class="sxs-lookup"><span data-stu-id="8ed3f-359">May 2020 updates</span></span>

<span data-ttu-id="8ed3f-360">2020 年 5 月更新包含數項功能的的、效能升級和 BUG 修正。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-360">The updates in May 2020 includes several features, performance upgrades, and bug fixes.</span></span>

### <a name="new-and-updated-features-in-may-2020"></a><span data-ttu-id="8ed3f-361">2020 年 5 月的新增及更新功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-361">New and updated features in May 2020</span></span>

#### <a name="data-ingestion"></a><span data-ttu-id="8ed3f-362">資料擷取</span><span class="sxs-lookup"><span data-stu-id="8ed3f-362">Data ingestion</span></span>

- <span data-ttu-id="8ed3f-363">**即時資料擷取：歷程記錄檢視**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-363">**Real-time data ingestion: history views**</span></span>

  <span data-ttu-id="8ed3f-364">使用我們的 API 來擷取即時更新時，您可以查看這些更新最多 30 天的彙總歷程記錄。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-364">When using our API to ingest real-time updates, you can see up to 30 days of aggregated history for these updates.</span></span> <span data-ttu-id="8ed3f-365">您可以存取所有成功或失敗 API 呼叫的彙總，包括其結果、來源系統以及其他有用的中繼資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-365">You have access to aggregates of all successful or failed API calls including their outcome, source system, and other useful metadata.</span></span>    
  <span data-ttu-id="8ed3f-366">如需詳細資訊，請參閱[即時資料擷取](real-time-data-ingestion.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-366">For more information, see [Real-time data ingestion](real-time-data-ingestion.md).</span></span>

- <span data-ttu-id="8ed3f-367">**即時資料擷取：設定檔更新**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-367">**Real-time data ingestion: profile updates**</span></span>

  <span data-ttu-id="8ed3f-368">這項即時資料擷取的擴充功能讓您在數秒內就能了解特定使用者設定檔欄位的變更。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-368">This extension of the real-time data ingestion lets you see, within seconds, changes to specific user profile fields.</span></span>    
  <span data-ttu-id="8ed3f-369">除了即時活動功能以外，系統也支援對設定檔欄位低延隔的更新動作。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-369">In addition to the real-time functionality for activities, the system supports low latency updates to profile fields.</span></span> <span data-ttu-id="8ed3f-370">設定檔欄位的即時更新有到期時間，因此不會取代已排定的重新整理。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-370">Real-time updates for profile fields have an expiration time and are therefore not a replacement for scheduled refreshes.</span></span>    
  <span data-ttu-id="8ed3f-371">如需詳細資訊，請參閱[即時資料擷取](real-time-data-ingestion.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-371">For more information, see [Real-time data ingestion](real-time-data-ingestion.md).</span></span>

#### <a name="extensibility"></a><span data-ttu-id="8ed3f-372">擴充性</span><span class="sxs-lookup"><span data-stu-id="8ed3f-372">Extensibility</span></span>

- <span data-ttu-id="8ed3f-373">**客戶卡片增益集上已更新的時間表和分頁**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-373">**Updated timeline and pagination on the Customer Card Add-in**</span></span>

  <span data-ttu-id="8ed3f-374">客戶卡增益集解決方案的時間表符合活動時間表。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-374">The timeline of the Customer Card Add-in solution matches the activity timeline.</span></span> <span data-ttu-id="8ed3f-375">時間表的分頁已改善，最多可一次顯示 50 項活動。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-375">The pagination of the timeline improved, showing up to 50 activities at once.</span></span> <span data-ttu-id="8ed3f-376">它也可讓您在時間表中載入更多活動。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-376">It also allows loading more activities in the timeline.</span></span>    
  <span data-ttu-id="8ed3f-377">如需詳細資訊，請參閱[客戶卡片增益集](customer-card-add-in.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-377">For more information, see [Customer Card Add-in](customer-card-add-in.md).</span></span>

- <span data-ttu-id="8ed3f-378">**客戶細分變更的 Power Automate 觸發程序**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-378">**Power Automate trigger for segment changes**</span></span>

  <span data-ttu-id="8ed3f-379">Power Automate 的觸發程序定義您可從中建置流程的內容。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-379">Triggers for Power Automate define what you can build a flow from.</span></span> <span data-ttu-id="8ed3f-380">新加入的觸發程序可讓您定義客戶細分的閾值。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-380">The newly added trigger lets you define a threshold for a segment.</span></span> <span data-ttu-id="8ed3f-381">例如，您可以建立會在越過定義的閾值時傳送的通知。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-381">For example, you can create a notification that gets sent when the defined threshold is passed.</span></span>    
  <span data-ttu-id="8ed3f-382">如需詳細資訊，請參閱 [Power Automate 連接器](export-power-automate.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-382">For more information, see [Power Automate connector](export-power-automate.md).</span></span>

- <span data-ttu-id="8ed3f-383">**自訂模型的多組織用戶共享支援**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-383">**Multitenant support for custom models**</span></span>

  <span data-ttu-id="8ed3f-384">透過不同 Azure Machine Learning 租用戶的 Web 服務，設定自訂模型的工作流程。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-384">Configure workflows for custom models with a web service of a different Azure Machine Learning tenant.</span></span> <span data-ttu-id="8ed3f-385">當您建立自訂模型的新工作流程時，您可以登入 Azure Machine Learning 租用戶。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-385">You can sign in to the Azure Machine Learning tenant when creating a new workflow for custom models.</span></span> <span data-ttu-id="8ed3f-386">這項功能是附加在整合於您自己自訂 Azure Machine Learning Web 服務之現有功能的項目。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-386">This capability is an addition to the existing capability of integrating with your own custom Azure Machine Learning web service.</span></span>    
  <span data-ttu-id="8ed3f-387">如需詳細資訊，請參閱[自訂機器學習模型](custom-models.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-387">For more information, see [Custom machine learning models](custom-models.md).</span></span>

#### <a name="segments"></a><span data-ttu-id="8ed3f-388">客戶細分</span><span class="sxs-lookup"><span data-stu-id="8ed3f-388">Segments</span></span>

- <span data-ttu-id="8ed3f-389">**實體路徑自動化**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-389">**Entity path automation**</span></span>

  <span data-ttu-id="8ed3f-390">當建立區段時，使用者必須定義實體路徑。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-390">When creating a segment, users need to define the entity path.</span></span> <span data-ttu-id="8ed3f-391">此功能會在自動化實體路徑定義時採取第一個步驟，這樣您就可以將專注於建立您所構想的客戶區隔準則。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-391">This capability takes a first step at automating the entity path definition so you can focus on the segmentation criteria that you have in mind.</span></span>    
  <span data-ttu-id="8ed3f-392">如果您要據以細分客戶的實體與統一客戶實體直接相關，就不需要再定義實體路徑。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-392">If the entity by which you want to segment your customers is directly related to the unified customer entity, you won't need to define the entity path anymore.</span></span> <span data-ttu-id="8ed3f-393">不過，如果有多個可能的實體路徑，您還是必須手動加以定義。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-393">However, if there is more than one possible entity path, you still need to define it manually.</span></span>

- <span data-ttu-id="8ed3f-394">**對多個客戶細分的動作**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-394">**Actions on multiple segments**</span></span>
  
  <span data-ttu-id="8ed3f-395">使用者只需按一下即可選取多個客戶細分並對其執行動作 (例如重新整理客戶細分)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-395">Users can select multiple segments and take actions on them, like refreshing the segments, with a single click.</span></span>    

- <span data-ttu-id="8ed3f-396">**重新整理客戶細分**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-396">**Refresh segments**</span></span>

  <span data-ttu-id="8ed3f-397">使用者可以重新整理單一客戶細分，或是只選取要重新整理的客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-397">Users can refresh a single segment or select only the segments they want to refresh.</span></span>    

  
- <span data-ttu-id="8ed3f-398">**對複合客戶細分的改善**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-398">**Improvements to compounded segments**</span></span>

  <span data-ttu-id="8ed3f-399">使用者可以建立、編輯和刪除在其他客戶細分基礎上建立的客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-399">Users can create, edit, and delete segments that are based on other segments.</span></span> <span data-ttu-id="8ed3f-400">例如，在其他建構於第三個客戶細分的客戶細分上所建構的客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-400">For example, a segment constructed on another segment that was constructed on a third segment.</span></span>    

- <span data-ttu-id="8ed3f-401">**客戶細分清單頁面**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-401">**Segment list page**</span></span>

  <span data-ttu-id="8ed3f-402">客戶細分頁面的新設計採用可讓您一次查看更多客戶細分的清單格式。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-402">The new design of the segments page uses a list format that lets you see more segments at once.</span></span> <span data-ttu-id="8ed3f-403">已新增搜尋欄位，以便快速尋找客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-403">A search field is added to find segments quickly.</span></span> <span data-ttu-id="8ed3f-404">使用者現在可同時在多個客戶細分上套用動作，例如下載或刪除。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-404">Users can now apply actions like downloading or deleting on multiple segments at once.</span></span> <span data-ttu-id="8ed3f-405">引進新的趨勢體驗，可快速識別客戶細分上的重大變更。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-405">A new trend experience is introduced to quickly identify significant changes on segments.</span></span>    
  <span data-ttu-id="8ed3f-406">如需詳細資訊，請參閱[建立和管理客戶細分](segments.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-406">For more information, see [Create and manage segments](segments.md).</span></span>

#### <a name="system-administration"></a><span data-ttu-id="8ed3f-407">系統管理</span><span class="sxs-lookup"><span data-stu-id="8ed3f-407">System administration</span></span>

- <span data-ttu-id="8ed3f-408">**可在 Microsoft Dynamics 365 Online Government 中使用 Customer Insights**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-408">**Customer Insights available in Microsoft Dynamics 365 Online Government**</span></span>

  <span data-ttu-id="8ed3f-409">隨著越來越多的管道可供互動之用，公民資料已散佈在無數的系統中，形成孤立資料，並導致對公民互動相關資訊的觀點也變得支離破碎。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-409">With more and more channels for interactions, citizen data is scattered across myriad systems, leading to siloed data, and a fragmented view of information about citizen interactions.</span></span> <span data-ttu-id="8ed3f-410">如果對不同管道上個別公民的互動情形沒有完整的觀點，政府就無法大規模推行現代化。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-410">Without a complete view of each citizen's interactions across channels, it's impossible for governments to modernize at scale.</span></span> <span data-ttu-id="8ed3f-411">Microsoft 致力於支援政府的技術需求，以維持民眾對一致且回應迅速體驗的期望。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-411">Microsoft is committed to supporting the technology needs of government to keep up with citizen expectations for consistent and responsive experiences.</span></span>    
  <span data-ttu-id="8ed3f-412">隨著 2020 年第 1 段發行浪潮到來，Dynamics 365 Customer Insights 將可用於政府社群雲端 (GCC) 這個旨在符合美國政府機關更高合規性需求的環境。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-412">With 2020 release wave 1, Dynamics 365 Customer Insights will be available for the Government Community Cloud (GCC), an environment built to meet the higher compliance needs of United States government agencies.</span></span> <span data-ttu-id="8ed3f-413">這些政府機關會獲得對民眾的統一觀點，並使用預建 AI 來產生改善互動情形、增強員工權能強和推動社群轉型的見解，同時降低 IT 複雜性，以及符合美國的合規性與安全性標準。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-413">Agencies gain a unified view of citizens and use prebuilt AI to derive insights that improve interactions, empower employees, and transform communities, while reducing IT complexity and meeting United States compliance and security standards.</span></span> <span data-ttu-id="8ed3f-414">Dynamics 365 Government 符合美國聯邦風險與授權管理計畫 (Federal Risk and Authorization Management Program，FedRAMP) 的嚴苛需求，使美國聯邦機構因 Microsoft 雲端的成本節約與嚴格安全性而獲益匪淺。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-414">Dynamics 365 Government meets the demanding requirements of the US Federal Risk and Authorization Management Program (FedRAMP), enabling United States federal agencies to benefit from the cost savings and rigorous security of the Microsoft Cloud.</span></span>

## <a name="april-2020-updates"></a><span data-ttu-id="8ed3f-415">2020 年 4 月更新</span><span class="sxs-lookup"><span data-stu-id="8ed3f-415">April 2020 updates</span></span>

<span data-ttu-id="8ed3f-416">2020 年 4 月更新包含數項功能的的、效能升級和 BUG 修正。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-416">The updates in April 2020 includes several features, performance upgrades, and bug fixes.</span></span>

### <a name="new-and-updated-features-in-april-2020"></a><span data-ttu-id="8ed3f-417">2020 年 4 月的新增及更新功能</span><span class="sxs-lookup"><span data-stu-id="8ed3f-417">New and updated features in April 2020</span></span>

#### <a name="activities"></a><span data-ttu-id="8ed3f-418">活動</span><span class="sxs-lookup"><span data-stu-id="8ed3f-418">Activities</span></span>

- <span data-ttu-id="8ed3f-419">**將活動實體對應至標準活動類型**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-419">**Map activity entity to standard activity type**</span></span>
  
  <span data-ttu-id="8ed3f-420">活動設定和儲存空間目前以靜態設計為基礎，您可在時間表中進行檢視。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-420">Activity configuration and storage are currently based on a static design to view them in a timeline.</span></span> <span data-ttu-id="8ed3f-421">目前並未完全使用活動的語意含義，這些活動在 AI 模型中可能會有多種使用案例。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-421">The semantic meaning of activities, which has potential for multiple use-cases in AI models, isn't fully used at the moment.</span></span> <span data-ttu-id="8ed3f-422">我們規劃要根據活動類型以及更好的活動語意理解，讓活動時間表變得更具動態。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-422">We plan to make the activity timeline more dynamic, based on the activity type and better semantic understanding of the activities.</span></span> <span data-ttu-id="8ed3f-423">此功能旨在識別 Common Data Model 中針對任何已擷取活動所定義的活動類型。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-423">This feature aims to identify the activity type as defined in Common Data Model for any ingested activity.</span></span>
  <span data-ttu-id="8ed3f-424">如需詳細資訊，請參閱[客戶活動](activities.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-424">For more information, see [Customer activities](activities.md).</span></span>

#### <a name="data-ingestion"></a><span data-ttu-id="8ed3f-425">資料擷取</span><span class="sxs-lookup"><span data-stu-id="8ed3f-425">Data ingestion</span></span>

- <span data-ttu-id="8ed3f-426">**即時資料擷取：活動**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-426">**Real-time data ingestion: activities**</span></span>
  
  <span data-ttu-id="8ed3f-427">即時資料內嵌功能立即提供資料方便使用，直到後續排程的重新整理作業將此資料從資料來源拉出為止。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-427">Real-time data ingestion provides data immediately for consumption, until the subsequent scheduled refresh pulls this data from the data source.</span></span>    
  <span data-ttu-id="8ed3f-428">如需詳細資訊，請參閱[即時資料擷取](real-time-data-ingestion.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-428">For more information, see [Real-time data ingestion](real-time-data-ingestion.md).</span></span>

- <span data-ttu-id="8ed3f-429">**對資料準備的改善**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-429">**Improvements to data preparation**</span></span>
  
  <span data-ttu-id="8ed3f-430">進一步了解實體中擷取的資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-430">Learn more about the data ingested in an entity.</span></span> <span data-ttu-id="8ed3f-431">您可以透過資料摘要了解可協助採取適當動作的資料品質特性。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-431">With the data summary, you can understand the data quality characteristics that can help to take appropriate action.</span></span>    
  <span data-ttu-id="8ed3f-432">如需詳細資訊，請參閱[探索實體資料](entities.md#exploring-a-specific-entitys-data)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-432">For more information, see [Explore entity data](entities.md#exploring-a-specific-entitys-data).</span></span>

- <span data-ttu-id="8ed3f-433">**透過 Common Data Service 從 Dynamics 365 擷取分析資料**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-433">**Ingest analytical data from Dynamics 365 with Common Data Service**</span></span>
  
  <span data-ttu-id="8ed3f-434">Common Data Service 可做為建立資料來源的方式。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-434">Common Data Service is available as a way to create data sources.</span></span> <span data-ttu-id="8ed3f-435">現有的 Dynamics 365 客戶可以將 Common Data Service 中的分析實體擷取到 Customer Insights。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-435">Existing Dynamics 365 customers can ingest analytical entities from Common Data Service to Customer Insights.</span></span> <span data-ttu-id="8ed3f-436">單一資料來源可同時在 Customer Insights 環境中使用同一個 Common Data Service 管理的湖。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-436">A single data source can simultaneously use the same Common Data Service-managed lake in a Customer Insights environment.</span></span>    
  <span data-ttu-id="8ed3f-437">如需詳細資訊，請參閱[連接至 Common Data Service 受管理資料湖中的資料](connect-common-data-service-lake.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-437">For more information, see [Connect to data in a Common Data Service managed data lake](connect-common-data-service-lake.md).</span></span>

#### <a name="extensibility"></a><span data-ttu-id="8ed3f-438">擴充性</span><span class="sxs-lookup"><span data-stu-id="8ed3f-438">Extensibility</span></span>

- <span data-ttu-id="8ed3f-439">**匯出至 LiveRamp**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-439">**Export to LiveRamp**</span></span>

  <span data-ttu-id="8ed3f-440">在 LiveRamp® 中啟用您的資料，與遍佈數位、社交和電視生態系統的 500 多個平台進行連接。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-440">Activate your data in LiveRamp® to connect with over 500 platforms across digital, social, and TV ecosystems.</span></span> <span data-ttu-id="8ed3f-441">在 LiveRamp 中使用您的資料來設定目標、排除和個人化廣告行銷活動。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-441">Use your data in LiveRamp for targeting, suppressing, and personalizing ad campaigns.</span></span>    
  <span data-ttu-id="8ed3f-442">如需詳細資訊，請參閱[LiveRamp&reg; 連接器](export-liveramp.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-442">For more information, see [LiveRamp&reg; connector](export-liveramp.md).</span></span>

- <span data-ttu-id="8ed3f-443">**Customer Insights Teams 增益集**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-443">**Customer Insights Teams Add-in**</span></span>
  
  <span data-ttu-id="8ed3f-444">機器人提供對統一客戶設定檔的查詢功能。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-444">The bot provides lookup capabilities for unified customer profiles.</span></span> <span data-ttu-id="8ed3f-445">其中會顯示包含最多 15 個來自所產生客戶設定檔中欄位的卡片。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-445">It will show a card with up to 15 fields from the resulting customer profile.</span></span> <span data-ttu-id="8ed3f-446">有多個相符項目時，會傳回可讓您選取設定檔的結果清單。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-446">Multiple matches return a list of results where you can select a profile.</span></span>    
  <span data-ttu-id="8ed3f-447">如需詳細資訊，請參閱 [Customer Insights 的 Teams 機器人](export-teams-bot.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-447">For more information, see [Teams bot for Customer Insights](export-teams-bot.md).</span></span>

#### <a name="measures"></a><span data-ttu-id="8ed3f-448">量值</span><span class="sxs-lookup"><span data-stu-id="8ed3f-448">Measures</span></span>

- <span data-ttu-id="8ed3f-449">**量值清單頁面**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-449">**Measure list page**</span></span>
  
  <span data-ttu-id="8ed3f-450">對量值頁面的改善包括支援對單一量值以及同時對多個量值採取的動作。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-450">Improvements to the measures page include support for actions on a single measure and on multiple measures at once.</span></span> <span data-ttu-id="8ed3f-451">此外，您還會發現有搜尋欄位可快速尋找和追蹤量值。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-451">Additionally, you'll find a search field to find and track measures quickly.</span></span>    
  <span data-ttu-id="8ed3f-452">如需詳細資訊，請參閱[建立和管理客戶細分](segments.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-452">For more information, see [Create and manage segments](segments.md).</span></span>

- <span data-ttu-id="8ed3f-453">**對複合量值的改善**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-453">**Improvements to compounded measures**</span></span>
  
  <span data-ttu-id="8ed3f-454">使用者可以建立、編輯和刪除在其他量值基礎上建立的量值。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-454">Users can create, edit, and delete measures that are based on other measures.</span></span> <span data-ttu-id="8ed3f-455">例如，在其他建構於第三個量值的量值上所建構的量值。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-455">For example, a measure constructed on another measure that was constructed on a third measure.</span></span>

#### <a name="segments"></a><span data-ttu-id="8ed3f-456">客戶細分</span><span class="sxs-lookup"><span data-stu-id="8ed3f-456">Segments</span></span>

- <span data-ttu-id="8ed3f-457">**另一個運算子**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-457">**Another operator**</span></span>
  
  <span data-ttu-id="8ed3f-458">IN 集運算子允許依數個可能的字串值進行客戶區隔。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-458">The In-set operator allows segmentation for customers by several possible string values.</span></span> <span data-ttu-id="8ed3f-459">將此運算子加入之前，您必須使用多個「或」條件來建構這類客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-459">Before this operator was added, you had to construct such segments with multiple OR conditions.</span></span> <span data-ttu-id="8ed3f-460">IN 集運算子可讓您使用單一條件來執行此動作。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-460">The In-set operator lets you do that with a single condition.</span></span>    
  <span data-ttu-id="8ed3f-461">如需詳細資訊，請參閱[建立和管理客戶細分](segments.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-461">For more information, see [Create and manage segments](segments.md).</span></span>

#### <a name="system-administration"></a><span data-ttu-id="8ed3f-462">系統管理</span><span class="sxs-lookup"><span data-stu-id="8ed3f-462">System administration</span></span>

- <span data-ttu-id="8ed3f-463">**將組態設定複製到新環境**</span><span class="sxs-lookup"><span data-stu-id="8ed3f-463">**Copy configuration settings to a new environment**</span></span>
  
  <span data-ttu-id="8ed3f-464">將您的組態從一個環境複製到另一個環境。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-464">Copy your configuration from one environment to another.</span></span> <span data-ttu-id="8ed3f-465">建立新環時，您可以選取要從中複製設定的現有環境。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-465">While creating a new environment, you can select an existing environment you want to copy the configuration from.</span></span> <span data-ttu-id="8ed3f-466">我們目前支援複製資料來源、資料統整、關聯、量值和客戶細分。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-466">We currently support data sources, data unification, relationships, measures, and segments to be copied.</span></span> <span data-ttu-id="8ed3f-467">不會複製資料來源認證和實際資料。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-467">Data source credentials and actual data aren't copied.</span></span>    
  <span data-ttu-id="8ed3f-468">如需詳細資訊，請參閱[管理環境](manage-environments.md)。</span><span class="sxs-lookup"><span data-stu-id="8ed3f-468">For more information, see [Manage environments](manage-environments.md).</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]