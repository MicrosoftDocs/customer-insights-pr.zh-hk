---
title: 使用資料來源內嵌資料
description: 了解如何從不同的來源匯入資料。
ms.date: 04/12/2021
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: conceptual
author: adkuppa
ms.author: adkuppa
ms.reviewer: mhart
manager: shellyha
ms.openlocfilehash: 54dd7b629d4b4e7f640b932b0f9246e0602f46bd
ms.sourcegitcommit: d84d664e67f263bfeb741154d309088c5101b9c3
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 06/24/2021
ms.locfileid: "6304723"
---
# <a name="data-sources-overview"></a><span data-ttu-id="8b077-103">資料來源概觀</span><span class="sxs-lookup"><span data-stu-id="8b077-103">Data sources overview</span></span>

[!INCLUDE [cc-data-platform-banner](../includes/cc-data-platform-banner.md)]

<span data-ttu-id="8b077-104">Dynamics 365 Customer Insights 中的對象見解功能從一組廣泛的來源集連接到資料。</span><span class="sxs-lookup"><span data-stu-id="8b077-104">The audience insights capability in Dynamics 365 Customer Insights connects to data from a broad set of sources.</span></span> <span data-ttu-id="8b077-105">連接至資料來源通常稱為 *資料擷取* 程序。</span><span class="sxs-lookup"><span data-stu-id="8b077-105">Connecting to a data source is often referred to as the process of *data ingestion*.</span></span> <span data-ttu-id="8b077-106">擷取資料之後，您可以對資料進行[統整](data-unification.md)並採取動作。</span><span class="sxs-lookup"><span data-stu-id="8b077-106">After ingesting the data, you can [unify](data-unification.md) and take action on it.</span></span>

## <a name="add-a-data-source"></a><span data-ttu-id="8b077-107">新增資料來源</span><span class="sxs-lookup"><span data-stu-id="8b077-107">Add a data source</span></span>

<span data-ttu-id="8b077-108">根據您所選擇的選項，參考有關如何新增資料來源的詳細文章。</span><span class="sxs-lookup"><span data-stu-id="8b077-108">Refer to the detailed articles on how to add a data source, depending on which option you choose.</span></span>

<span data-ttu-id="8b077-109">有三種主要方式可以新增資料來源：</span><span class="sxs-lookup"><span data-stu-id="8b077-109">You can add a data source in three main ways:</span></span>

- [<span data-ttu-id="8b077-110">透過數十個 Power Query 連接器</span><span class="sxs-lookup"><span data-stu-id="8b077-110">Through dozens of Power Query connectors</span></span>](connect-power-query.md)
- [<span data-ttu-id="8b077-111">從 Common Data Model 資料夾</span><span class="sxs-lookup"><span data-stu-id="8b077-111">From a Common Data Model folder</span></span>](connect-common-data-model.md)
- [<span data-ttu-id="8b077-112">從您自己的 Microsoft Dataverse 資料湖</span><span class="sxs-lookup"><span data-stu-id="8b077-112">From your own Microsoft Dataverse lake</span></span>](connect-common-data-service-lake.md)

## <a name="add-data-from-on-premises-data-sources"></a><span data-ttu-id="8b077-113">從內部部署資料來源新增資料</span><span class="sxs-lookup"><span data-stu-id="8b077-113">Add data from on-premises data sources</span></span>

<span data-ttu-id="8b077-114">Microsoft Power Platform 資料流程支援在對象見解中從內部部署的資料來源內嵌資料。</span><span class="sxs-lookup"><span data-stu-id="8b077-114">Ingesting data from on-premises data sources in audience insights is supported based on Microsoft Power Platform dataflows.</span></span> <span data-ttu-id="8b077-115">設定環境時，[在 Microsoft Dataverse 提供環境 URL](manage-environments.md#create-an-environment-in-an-existing-organization)，便可以在 Customer Insights 中啟用資料流程。</span><span class="sxs-lookup"><span data-stu-id="8b077-115">Dataflows can be enabled in Customer Insights by [providing the Microsoft Dataverse environment URL](manage-environments.md#create-an-environment-in-an-existing-organization) when setting up the environment.</span></span>

<span data-ttu-id="8b077-116">將 Dataverse 環境與 Customer Insights 關聯之後，所建立的資料來源預設使用 [Power Platform 資料流程](/power-query/dataflows/overview-dataflows-across-power-platform-dynamics-365)。</span><span class="sxs-lookup"><span data-stu-id="8b077-116">Data sources that are created after associating a Dataverse environment with Customer Insights will use [Power Platform dataflows](/power-query/dataflows/overview-dataflows-across-power-platform-dynamics-365) by default.</span></span> <span data-ttu-id="8b077-117">資料流程使用資料閘道來支援內部部署連線。</span><span class="sxs-lookup"><span data-stu-id="8b077-117">Dataflows support on-premises connectivity using the data gateway.</span></span> <span data-ttu-id="8b077-118">在關聯 Dataverse 環境前就已存在的資料來源，請移除並重新建立，才能[使用內部部署資料閘道](/data-integration/gateway/service-gateway-app.md)。</span><span class="sxs-lookup"><span data-stu-id="8b077-118">Remove and recreate data sources that existed before a Dataverse environment was associated to [use the on-premises data gateways](/data-integration/gateway/service-gateway-app.md).</span></span>

<span data-ttu-id="8b077-119">來自現有 Power BI 或 Power Apps 環境的資料閘道將會顯示，並且可以在 Customer Insights 中重複使用。</span><span class="sxs-lookup"><span data-stu-id="8b077-119">Data gateways from an existing Power BI or Power Apps environment will be visible and you can reuse in Customer Insights.</span></span> <span data-ttu-id="8b077-120">資料來源頁面顯示的連結，您可移至 Microsoft Power Platform 查看和設定內部部署資料閘道的環境。</span><span class="sxs-lookup"><span data-stu-id="8b077-120">The data sources page shows links to go to the Microsoft Power Platform environment where you can view and configure on-premises data gateways.</span></span>

## <a name="review-ingested-data"></a><span data-ttu-id="8b077-121">檢閱擷取的資料</span><span class="sxs-lookup"><span data-stu-id="8b077-121">Review ingested data</span></span>

<span data-ttu-id="8b077-122">您會看到每個擷取資料來源的名稱、其狀態以及該來源上次重新整理資料的時間。</span><span class="sxs-lookup"><span data-stu-id="8b077-122">You'll see the name of each ingested data source, its status, and the last time the data was refreshed for that source.</span></span> <span data-ttu-id="8b077-123">您可以依據各欄位排序資料來源清單。</span><span class="sxs-lookup"><span data-stu-id="8b077-123">You can sort the list of data sources by every column.</span></span>

> [!div class="mx-imgBorder"]
> <span data-ttu-id="8b077-124">![新增的資料來源](media/configure-data-datasource-added.png "新增的資料來源")</span><span class="sxs-lookup"><span data-stu-id="8b077-124">![Data source added](media/configure-data-datasource-added.png "Data source added")</span></span>

|<span data-ttu-id="8b077-125">Status</span><span class="sxs-lookup"><span data-stu-id="8b077-125">Status</span></span>  |<span data-ttu-id="8b077-126">描述</span><span class="sxs-lookup"><span data-stu-id="8b077-126">Description</span></span>  |
|---------|---------|
|<span data-ttu-id="8b077-127">成功</span><span class="sxs-lookup"><span data-stu-id="8b077-127">Successful</span></span>   |<span data-ttu-id="8b077-128">如果 **重新整理的** 欄位提到時間，代表已成功內嵌資料來源。</span><span class="sxs-lookup"><span data-stu-id="8b077-128">Data source was successfully ingested if a time is mentioned in the **Refreshed** column.</span></span>
|<span data-ttu-id="8b077-129">未開始</span><span class="sxs-lookup"><span data-stu-id="8b077-129">Not started</span></span>   |<span data-ttu-id="8b077-130">資料來源尚未內嵌任何資料或仍在草稿模式中。</span><span class="sxs-lookup"><span data-stu-id="8b077-130">The data source has no data ingested yet or still in draft mode.</span></span>         |
|<span data-ttu-id="8b077-131">正在重新整理</span><span class="sxs-lookup"><span data-stu-id="8b077-131">Refreshing</span></span>    |<span data-ttu-id="8b077-132">資料擷取進行中。</span><span class="sxs-lookup"><span data-stu-id="8b077-132">Data ingestion is in progress.</span></span> <span data-ttu-id="8b077-133">您可以選取 **動作** 欄中的 **停止重新整理** 來取消此作業。</span><span class="sxs-lookup"><span data-stu-id="8b077-133">You can cancel this operation by selecting **Stop refreshing** in the **Actions** column.</span></span> <span data-ttu-id="8b077-134">停止重新整理資料來源會將它還原至上次重新整理的狀態。</span><span class="sxs-lookup"><span data-stu-id="8b077-134">Stopping the refresh of a data source will revert it to its last refresh state.</span></span>       |
|<span data-ttu-id="8b077-135">失敗</span><span class="sxs-lookup"><span data-stu-id="8b077-135">Failed</span></span>     |<span data-ttu-id="8b077-136">資料擷取執行時遇到錯誤。</span><span class="sxs-lookup"><span data-stu-id="8b077-136">Data ingestion ran into errors.</span></span>         |

<span data-ttu-id="8b077-137">在任何資料來源中選取 **狀態** 欄中的值，以查看更多詳細資料。</span><span class="sxs-lookup"><span data-stu-id="8b077-137">Select the value in the **Status** column of any data source to review more details.</span></span> <span data-ttu-id="8b077-138">在 **進度詳細資料** 窗格中，展開 **資料來源**。</span><span class="sxs-lookup"><span data-stu-id="8b077-138">In the **Progress details** pane, expand **Data sources**.</span></span> <span data-ttu-id="8b077-139">請選取 **查看詳細資料** 來查看更新狀態的更多詳細資料，包括錯誤詳細資料與下游程序更新。</span><span class="sxs-lookup"><span data-stu-id="8b077-139">Select **See details** for more information about the refresh status, including error details and downstream process updates.</span></span>

<span data-ttu-id="8b077-140">載入資料可能需要花費一些時間。</span><span class="sxs-lookup"><span data-stu-id="8b077-140">Loading data can take time.</span></span> <span data-ttu-id="8b077-141">成功重新整理之後，即可從 **實體** 頁面查看擷取的資料。</span><span class="sxs-lookup"><span data-stu-id="8b077-141">After a successful refresh, the ingested data can be reviewed from the **Entities** page.</span></span> <span data-ttu-id="8b077-142">如需詳細資訊，請參閱[實體](entities.md)。</span><span class="sxs-lookup"><span data-stu-id="8b077-142">For more information, see [Entities](entities.md).</span></span>

## <a name="refresh-a-data-source"></a><span data-ttu-id="8b077-143">重新整理資料來源</span><span class="sxs-lookup"><span data-stu-id="8b077-143">Refresh a data source</span></span>

<span data-ttu-id="8b077-144">資料來源可自動排程或依照需要情況手動重新整理。</span><span class="sxs-lookup"><span data-stu-id="8b077-144">Data sources can be refreshed on an automatic schedule or refreshed manually on demand.</span></span> 

<span data-ttu-id="8b077-145">請前往 **管理員** > **系統** > [**排程**](system.md#schedule-tab)，組態您內嵌所有資料來源的重新整理排程。</span><span class="sxs-lookup"><span data-stu-id="8b077-145">Go to **Admin** > **System** > [**Schedule**](system.md#schedule-tab) to configure scheduled refreshes of all your ingested data sources.</span></span>

<span data-ttu-id="8b077-146">若要依照需要重新整理資料來源，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="8b077-146">To refresh a data source on demand, follow these steps:</span></span>

1. <span data-ttu-id="8b077-147">在對象見解中，前往 **資料** > **資料來源**。</span><span class="sxs-lookup"><span data-stu-id="8b077-147">In audience insights, go to **Data** > **Data sources**.</span></span>

2. <span data-ttu-id="8b077-148">在您要重新整理的資料來源旁邊選取垂直省略號，然後從下拉式清單中選取 **重新整理**。</span><span class="sxs-lookup"><span data-stu-id="8b077-148">Select the vertical ellipsis next to the data source you want to refresh and select **Refresh** from the dropdown list.</span></span>

3. <span data-ttu-id="8b077-149">資料來源現在會針對手動重新整理觸發。</span><span class="sxs-lookup"><span data-stu-id="8b077-149">The data source is now triggered for a manual refresh.</span></span> <span data-ttu-id="8b077-150">重新整理資料來源將會更新資料來源中所有指定實體的實體結構描述和資料。</span><span class="sxs-lookup"><span data-stu-id="8b077-150">Refreshing a data source will update both the entity schema and data for all the entities specified in the data source.</span></span>

4. <span data-ttu-id="8b077-151">如果您要取消現有的重新整理，且資料來源將恢復成上次重新整理狀態，請選取 **停止重新整理**。</span><span class="sxs-lookup"><span data-stu-id="8b077-151">Select **Stop refreshing** if you want to cancel an existing refresh and the data source will revert to its last refresh status.</span></span>

## <a name="delete-a-data-source"></a><span data-ttu-id="8b077-152">刪除資料來源</span><span class="sxs-lookup"><span data-stu-id="8b077-152">Delete a data source</span></span>

1. <span data-ttu-id="8b077-153">在對象見解中，前往 **資料** > **資料來源**。</span><span class="sxs-lookup"><span data-stu-id="8b077-153">In audience insights, go to **Data** > **Data sources**.</span></span>

2. <span data-ttu-id="8b077-154">在您要移除的資料來源旁邊選取垂直省略號，然後從下拉式功能表中選取 **刪除**。</span><span class="sxs-lookup"><span data-stu-id="8b077-154">Select the vertical ellipsis next to the data source you want to remove and select **Delete** from the dropdown menu.</span></span>

3. <span data-ttu-id="8b077-155">確認刪除。</span><span class="sxs-lookup"><span data-stu-id="8b077-155">Confirm your deletion.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
