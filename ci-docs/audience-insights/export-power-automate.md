---
title: Power Automate 連接器 | Microsoft Docs
description: 在 Dynamics 365 Customer Insights 中建立 Microsoft Power Automate 的流程。
ms.date: 01/20/2021
ms.reviewer: mhart
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: how-to
author: pkieffer
ms.author: philk
manager: shellyha
ms.openlocfilehash: ce2477d957a1792e0436a0dfc15a33621b1c89a9
ms.sourcegitcommit: e8e03309ba2515374a70c132d0758f3e1e1851d0
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 05/04/2021
ms.locfileid: "5976115"
---
# <a name="power-automate-connector-preview"></a><span data-ttu-id="88179-103">Power Automate 連接器 (預覽)</span><span class="sxs-lookup"><span data-stu-id="88179-103">Power Automate connector (preview)</span></span>

<span data-ttu-id="88179-104">資料變更時觸發自動發生的特定事件，或直接在 [Power Automate](https://flow.microsoft.com/) 中管理更複雜的流程。</span><span class="sxs-lookup"><span data-stu-id="88179-104">Trigger specific events to occur automatically when your data changes and manage more complex flows directly in [Power Automate](https://flow.microsoft.com/).</span></span>

## <a name="power-automate-triggers"></a><span data-ttu-id="88179-105">Power Automate 觸發程序</span><span class="sxs-lookup"><span data-stu-id="88179-105">Power Automate triggers</span></span>

<span data-ttu-id="88179-106">使用觸發程序來建立雲端流程並自動化重複工作，例如通知或更多進階動作。</span><span class="sxs-lookup"><span data-stu-id="88179-106">Use triggers to create cloud flows and automate repetitive tasks, such as notifications or more advanced actions.</span></span> 

- <span data-ttu-id="88179-107">當資料來源重新整理失敗時觸發。</span><span class="sxs-lookup"><span data-stu-id="88179-107">Trigger when a data source refresh fails.</span></span> 
- <span data-ttu-id="88179-108">當資料來源重新整理成功時觸發。</span><span class="sxs-lookup"><span data-stu-id="88179-108">Trigger when a data source refresh succeeds.</span></span>
- <span data-ttu-id="88179-109">在區段上越過閾值時觸發。</span><span class="sxs-lookup"><span data-stu-id="88179-109">Trigger when a threshold is crossed on a segment.</span></span> <span data-ttu-id="88179-110">觸發程序受限在需要超過閾值以上。</span><span class="sxs-lookup"><span data-stu-id="88179-110">The trigger is limited to crossing above the threshold.</span></span>
- <span data-ttu-id="88179-111">在業務量值上越過閾值時觸發。</span><span class="sxs-lookup"><span data-stu-id="88179-111">Trigger when a threshold is crossed on a business measure.</span></span> <span data-ttu-id="88179-112">此處僅顯示缺少維度的業務量值。</span><span class="sxs-lookup"><span data-stu-id="88179-112">Only business measures without a dimension are supported.</span></span> <span data-ttu-id="88179-113">觸發程序限制為必須超過閾值以上。</span><span class="sxs-lookup"><span data-stu-id="88179-113">The trigger is limited crossing above the threshold.</span></span>
- <span data-ttu-id="88179-114">當完成 (資料來源、區段、量值，...) 的完整重新整理時，會引發發射鍵。</span><span class="sxs-lookup"><span data-stu-id="88179-114">Trigger when a full refresh of (data sources, segments, measures,...) is completed.</span></span>
- <span data-ttu-id="88179-115">在完成統整程序 (對應、比對、合併) 機重新整理時觸發。</span><span class="sxs-lookup"><span data-stu-id="88179-115">Trigger when a refresh of the unification process (map, match, merge) is completed.</span></span>

<span data-ttu-id="88179-116">[在 Power Automate 中設定您的觸發程序](https://flow.microsoft.com/connectors/shared_customerinsights/dynamics-365-customer-insights-connector/)。</span><span class="sxs-lookup"><span data-stu-id="88179-116">[Configure your triggers in Power Automate](https://flow.microsoft.com/connectors/shared_customerinsights/dynamics-365-customer-insights-connector/).</span></span>

## <a name="power-automate-actions"></a><span data-ttu-id="88179-117">Power Automate 動作</span><span class="sxs-lookup"><span data-stu-id="88179-117">Power Automate actions</span></span>
<span data-ttu-id="88179-118">Power Automate 連接器提供可用觸發程序以外的動作。</span><span class="sxs-lookup"><span data-stu-id="88179-118">The Power Automate connector provides other actions than the available triggers.</span></span> <span data-ttu-id="88179-119">如需詳細資訊，請參閱《[Dynamics 365 Customer Insights Connector](/connectors/customerinsights/)》。</span><span class="sxs-lookup"><span data-stu-id="88179-119">For more information, see the [Dynamics 365 Customer Insights Connector](/connectors/customerinsights/).</span></span>

## <a name="create-a-power-automate-flow"></a><span data-ttu-id="88179-120">建立 Power Automate 流程</span><span class="sxs-lookup"><span data-stu-id="88179-120">Create a Power Automate flow</span></span>

1. <span data-ttu-id="88179-121">在對象見解中，前往 **系統管理員** > **匯出目的地**。</span><span class="sxs-lookup"><span data-stu-id="88179-121">In audience insights, go to **Admin** > **Export destinations**.</span></span>

1. <span data-ttu-id="88179-122">在 **Power Automate** 圖格中，選取 **設定**。</span><span class="sxs-lookup"><span data-stu-id="88179-122">On the **Power Automate** tile, select **Set up**.</span></span>

1. <span data-ttu-id="88179-123">Power Automate 中的 Customer Insights 連結器 (preview) 開啟。</span><span class="sxs-lookup"><span data-stu-id="88179-123">The Customer Insights Connector (preview) in Power Automate opens.</span></span> <span data-ttu-id="88179-124">**登入** Power Automate。</span><span class="sxs-lookup"><span data-stu-id="88179-124">**Sign in** to Power Automate.</span></span>

1. <span data-ttu-id="88179-125">選擇其中一個可用的觸發程序，並在新流程中新增更多步驟。</span><span class="sxs-lookup"><span data-stu-id="88179-125">Choose one of the available triggers and add more steps to your new flow.</span></span> <span data-ttu-id="88179-126">如需詳細資訊，請參閱[在 Power Automate 中建立雲端工作流程](/power-automate/get-started-logic-flow)。</span><span class="sxs-lookup"><span data-stu-id="88179-126">For more information, see [Create a cloud flow in Power Automate](/power-automate/get-started-logic-flow).</span></span>

<span data-ttu-id="88179-127">如何使用流程的範例：</span><span class="sxs-lookup"><span data-stu-id="88179-127">Examples how to use flows:</span></span> 
- <span data-ttu-id="88179-128">若資料來源重新整理失敗，請將訊息張貼到 Microsoft Teams 頻道。</span><span class="sxs-lookup"><span data-stu-id="88179-128">Post a message to a Microsoft Teams channel if a data source refresh fails.</span></span> 
- <span data-ttu-id="88179-129">達到客戶細分上的閾值時，將電子郵件傳送給資料負責人。</span><span class="sxs-lookup"><span data-stu-id="88179-129">Send an email to the data owners when a threshold on a segment is crossed.</span></span>



[!INCLUDE[footer-include](../includes/footer-banner.md)]
