---
title: 從 Customer Insights 匯出資料
description: 管理匯出到共用資料 。
ms.date: 03/25/2021
ms.reviewer: mhart
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: conceptual
author: pkieffer
ms.author: philk
manager: shellyha
ms.openlocfilehash: c1078ed0ba259a6e9cde3c7ede3570890ae48e67
ms.sourcegitcommit: 33a8e21b3bf6521bdb8346f81f79fce88091ddfd
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 05/10/2021
ms.locfileid: "6016663"
---
# <a name="exports-preview-overview"></a><span data-ttu-id="e4190-103">匯出 (預覽版) 概觀</span><span class="sxs-lookup"><span data-stu-id="e4190-103">Exports (preview) overview</span></span>

<span data-ttu-id="e4190-104">**匯出** 頁面會顯示所有已設定的匯出。</span><span class="sxs-lookup"><span data-stu-id="e4190-104">The **Exports** page shows you all configured exports.</span></span> <span data-ttu-id="e4190-105">匯出與各種應用程式共用指定資料。</span><span class="sxs-lookup"><span data-stu-id="e4190-105">Exports share specific data with various applications.</span></span> <span data-ttu-id="e4190-106">這可以包括客戶個人資料或實體、結構描述及對應詳細資料。</span><span class="sxs-lookup"><span data-stu-id="e4190-106">They can include customer profiles or entities, schemas, and mapping details.</span></span> <span data-ttu-id="e4190-107">每個匯出都需要[由系統管理員設定的連接，來管理驗證和存取權](connections.md)。</span><span class="sxs-lookup"><span data-stu-id="e4190-107">Each export requires a [connection, set up by an administrator, to manage authentication and access](connections.md).</span></span>

<span data-ttu-id="e4190-108">移至 **資料** > **匯出** 以查看匯出頁面。</span><span class="sxs-lookup"><span data-stu-id="e4190-108">Go to **Data** > **Exports** to view the exports page.</span></span> <span data-ttu-id="e4190-109">所有使用者角色都擁有存取權，可以查看設定好的匯出。</span><span class="sxs-lookup"><span data-stu-id="e4190-109">All user roles have access to view configured exports.</span></span> <span data-ttu-id="e4190-110">在命令列中使用搜尋欄位，可用名稱、連接名稱或連線類型來尋找匯出。</span><span class="sxs-lookup"><span data-stu-id="e4190-110">Use of the search field in the command bar to find exports by their name, connection name, or connection type.</span></span>

## <a name="set-up-a-new-export"></a><span data-ttu-id="e4190-111">設定新的匯出</span><span class="sxs-lookup"><span data-stu-id="e4190-111">Set up a new export</span></span>

<span data-ttu-id="e4190-112">若要設定或編輯匯出，您需要有可用的連接。</span><span class="sxs-lookup"><span data-stu-id="e4190-112">To set up or edit an export, you need to have connections available to you.</span></span> <span data-ttu-id="e4190-113">連接依據您的[使用者角色](permissions.md)而定：</span><span class="sxs-lookup"><span data-stu-id="e4190-113">Connections depend on your [user role](permissions.md):</span></span>
- <span data-ttu-id="e4190-114">系統管理員可以存取所有的連接。</span><span class="sxs-lookup"><span data-stu-id="e4190-114">Administrators have access to all connections.</span></span> <span data-ttu-id="e4190-115">在設定匯出時，他們也可以建立新的連接。</span><span class="sxs-lookup"><span data-stu-id="e4190-115">They can also create new connections when setting up an export.</span></span>
- <span data-ttu-id="e4190-116">參與者可以存取特定的連接。</span><span class="sxs-lookup"><span data-stu-id="e4190-116">Contributors can have access to specific connections.</span></span> <span data-ttu-id="e4190-117">他們依賴系統管理員來設定和共用連接。</span><span class="sxs-lookup"><span data-stu-id="e4190-117">They depend on administrators to configure and share connections.</span></span> <span data-ttu-id="e4190-118">如需詳細資訊，請參閱[允許參與者使用匯出的連接](connections.md#allow-contributors-to-use-a-connection-for-exports)。</span><span class="sxs-lookup"><span data-stu-id="e4190-118">For more information, see [Allow contributors to use a connection for exports](connections.md#allow-contributors-to-use-a-connection-for-exports).</span></span>
- <span data-ttu-id="e4190-119">檢視器只能查看現有的匯出，並不能建立。</span><span class="sxs-lookup"><span data-stu-id="e4190-119">Viewers can only view existing exports but not create them.</span></span>

1. <span data-ttu-id="e4190-120">移至 **資料** > **匯出**。</span><span class="sxs-lookup"><span data-stu-id="e4190-120">Go to **Data** > **Exports**.</span></span>

1. <span data-ttu-id="e4190-121">若要建立新的匯出目的地，請選取 **新增匯出**。</span><span class="sxs-lookup"><span data-stu-id="e4190-121">Select **Add export** to create a new export destination.</span></span>

1. <span data-ttu-id="e4190-122">在 **設定匯出** 窗格中，選取要使用的連接。</span><span class="sxs-lookup"><span data-stu-id="e4190-122">In the **Set up export** pane, select which connection to use.</span></span> <span data-ttu-id="e4190-123">[連接](connections.md)是由系統管理員所管理。</span><span class="sxs-lookup"><span data-stu-id="e4190-123">[Connections](connections.md) are managed by administrators.</span></span> 

1. <span data-ttu-id="e4190-124">提供必要的詳細資料，並選取 **儲存** 來建立匯出。</span><span class="sxs-lookup"><span data-stu-id="e4190-124">Provide the required details and select **Save** to create the export.</span></span>

### <a name="edit-an-export"></a><span data-ttu-id="e4190-125">編輯匯出</span><span class="sxs-lookup"><span data-stu-id="e4190-125">Edit an export</span></span>

1. <span data-ttu-id="e4190-126">選取想要編輯的匯出目的地其垂直省略符號。</span><span class="sxs-lookup"><span data-stu-id="e4190-126">Select the vertical ellipsis for the export destination you want to edit.</span></span>

1. <span data-ttu-id="e4190-127">從下拉式清單功能表中選取 **編輯**。</span><span class="sxs-lookup"><span data-stu-id="e4190-127">Select **Edit** from the drop-down menu.</span></span>

1. <span data-ttu-id="e4190-128">變更想要更新的值並選取 **儲存**。</span><span class="sxs-lookup"><span data-stu-id="e4190-128">Change the values you want to update and select **Save**.</span></span>

## <a name="view-exports-and-export-details"></a><span data-ttu-id="e4190-129">查看匯出和匯出詳細資料</span><span class="sxs-lookup"><span data-stu-id="e4190-129">View Exports and export details</span></span>

<span data-ttu-id="e4190-130">建立匯出目的地之後，就會在 **資料** > **匯出** 中列出。</span><span class="sxs-lookup"><span data-stu-id="e4190-130">After creating export destinations, they are listed on **Data** > **Exports**.</span></span> <span data-ttu-id="e4190-131">所有使用者都可以看到已共用的資料及其最新狀態。</span><span class="sxs-lookup"><span data-stu-id="e4190-131">All users can see which data is shared and its latest status.</span></span>

1. <span data-ttu-id="e4190-132">移至 **資料** > **匯出**。</span><span class="sxs-lookup"><span data-stu-id="e4190-132">Go to **Data** > **Exports**.</span></span>

1. <span data-ttu-id="e4190-133">沒有編輯權限的使用者選取 **查看** 而非 **編輯** 來查看匯出詳細資料。</span><span class="sxs-lookup"><span data-stu-id="e4190-133">Users without edit permissions select **View** instead of **Edit** see the export details.</span></span>

1. <span data-ttu-id="e4190-134">此側邊窗格會顯示這項匯出的設定。</span><span class="sxs-lookup"><span data-stu-id="e4190-134">This side pane shows the set up of this export.</span></span> <span data-ttu-id="e4190-135">若沒有編輯權限，就無法變更值。</span><span class="sxs-lookup"><span data-stu-id="e4190-135">Without edit permissions, you can't change values.</span></span> <span data-ttu-id="e4190-136">選取 **關閉** 來返回匯出頁面。</span><span class="sxs-lookup"><span data-stu-id="e4190-136">Select **Close** to return to the exports page.</span></span>

## <a name="run-exports-on-demand"></a><span data-ttu-id="e4190-137">視需要執行匯出</span><span class="sxs-lookup"><span data-stu-id="e4190-137">Run exports on demand</span></span>

<span data-ttu-id="e4190-138">設定匯出之後，只要有能運作的連接，每次[排程的重新整理](system.md#schedule-tab)都會執行。</span><span class="sxs-lookup"><span data-stu-id="e4190-138">After configuring an export, it will run with every [scheduled refresh](system.md#schedule-tab) as long as it has a working connection.</span></span>

<span data-ttu-id="e4190-139">若不等待排程的重新整理，要匯出資料，請移至 **資料** > **匯出**。</span><span class="sxs-lookup"><span data-stu-id="e4190-139">To export data without waiting for a scheduled refresh, go to **Data** > **Exports**.</span></span> <span data-ttu-id="e4190-140">您有兩個選擇：</span><span class="sxs-lookup"><span data-stu-id="e4190-140">You have two options:</span></span>

- <span data-ttu-id="e4190-141">若要執行所有匯出，請選取命令列中的 **全部執行**。</span><span class="sxs-lookup"><span data-stu-id="e4190-141">To run all exports, select **Run all** in the command bar.</span></span> 
- <span data-ttu-id="e4190-142">若要執行單一匯出，請選取清單項目的省略號 (...) ，然後選擇 **執行**。</span><span class="sxs-lookup"><span data-stu-id="e4190-142">To run a single export, select the ellipsis (...) on a list item and then choose **Run**.</span></span>

## <a name="remove-an-export"></a><span data-ttu-id="e4190-143">移除匯出</span><span class="sxs-lookup"><span data-stu-id="e4190-143">Remove an Export</span></span>

1. <span data-ttu-id="e4190-144">移至 **資料** > **匯出**。</span><span class="sxs-lookup"><span data-stu-id="e4190-144">Go to **Data** > **Exports**.</span></span>

1. <span data-ttu-id="e4190-145">選取要移除的匯出目的地其垂直省略符號。</span><span class="sxs-lookup"><span data-stu-id="e4190-145">Select the vertical ellipsis for the Export you want to remove.</span></span>

1. <span data-ttu-id="e4190-146">從下拉式功能表中選取 **移除**。</span><span class="sxs-lookup"><span data-stu-id="e4190-146">Select **Remove** from the dropdown menu.</span></span>

1. <span data-ttu-id="e4190-147">在確認畫面上選取 **移除** 以確認移除。</span><span class="sxs-lookup"><span data-stu-id="e4190-147">Confirm the removal by selecting **Remove** on the confirmation screen.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
