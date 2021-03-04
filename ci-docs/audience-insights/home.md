---
title: 對象見解中的首頁
description: 開始在首頁上探索應用程式。
ms.date: 01/07/2021
ms.reviewer: nimagen
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: conceptual
author: m-hartmann
ms.author: mhart
manager: shellyha
ms.openlocfilehash: 7cc767f5d80b213a4c1bb5b2e8062bd44c15279b
ms.sourcegitcommit: 0260ed244b97c2fd0be5e9a084c4c489358e8d4f
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 02/18/2021
ms.locfileid: "5477068"
---
# <a name="create-a-new-environment"></a><span data-ttu-id="60096-103">建立新環境</span><span class="sxs-lookup"><span data-stu-id="60096-103">Create a new environment</span></span>

## <a name="create-a-trial-environment"></a><span data-ttu-id="60096-104">建立試用環境</span><span class="sxs-lookup"><span data-stu-id="60096-104">Create a trial environment</span></span>

<span data-ttu-id="60096-105">您可以在[試用註冊頁面](https://dynamics.microsoft.com/get-started/free-trial/?appname=customerinsights)上註冊試用。</span><span class="sxs-lookup"><span data-stu-id="60096-105">You can sign up for a trial on the [trial sign up page](https://dynamics.microsoft.com/get-started/free-trial/?appname=customerinsights).</span></span> 

> [!NOTE]
> <span data-ttu-id="60096-106">試用會在 30 天後過期。</span><span class="sxs-lookup"><span data-stu-id="60096-106">Trials expire after 30 days.</span></span>

1. <span data-ttu-id="60096-107">選擇 **註冊免費試用** 選項，然後選取 **立即註冊**。</span><span class="sxs-lookup"><span data-stu-id="60096-107">Choose the **Sign up for a free trial** option and select **Sign up now**.</span></span>

1. <span data-ttu-id="60096-108">提供您的公司或學校電子郵件地址，告訴我們更多有關您個人的資訊，然後選取 **下一步**。</span><span class="sxs-lookup"><span data-stu-id="60096-108">Provide your work or school email address, tell us a more about yourself and select **Next**.</span></span>

   :::image type="content" source="media/trial-signup-dialog.png" alt-text="註冊試用執行個體的對話方塊":::

1. <span data-ttu-id="60096-110">提供您的新環境的 **名稱**。</span><span class="sxs-lookup"><span data-stu-id="60096-110">Provide a **Name** for your new environment.</span></span> 

1. <span data-ttu-id="60096-111">選取試用類型。</span><span class="sxs-lookup"><span data-stu-id="60096-111">Select the trial type.</span></span>

1. <span data-ttu-id="60096-112">選擇您的環境的 **區域**。</span><span class="sxs-lookup"><span data-stu-id="60096-112">Choose the **Region** for your environment.</span></span>

1. <span data-ttu-id="60096-113">(選擇性) 如果是 Dynamics 365 組織的系統管理員：選取 **進階設定**，並提供您的組織的 URL，以便使用像客戶流失這樣的預測功能。</span><span class="sxs-lookup"><span data-stu-id="60096-113">Optionally, for admins of a Dynamics 365 organization: Select **Advanced settings** and provide the URL of your organization to use prediction features like customer churn.</span></span>

1. <span data-ttu-id="60096-114">選取 **建立**。</span><span class="sxs-lookup"><span data-stu-id="60096-114">Select **Create**.</span></span> 

<span data-ttu-id="60096-115">建立環境之後，您會看到 **示範** 環境，讓您使用虛構資料探索應用程式。</span><span class="sxs-lookup"><span data-stu-id="60096-115">After the environment was created, you'll see the **Demo** environment which lets you explore the app with fictitious data.</span></span> <span data-ttu-id="60096-116">您可以變更範例資料，以符合您的行業。</span><span class="sxs-lookup"><span data-stu-id="60096-116">You can change the sample data to match your industry.</span></span> <span data-ttu-id="60096-117">選取標題中的 **設定** 圖示，然後選取 **示範設定**。</span><span class="sxs-lookup"><span data-stu-id="60096-117">Select the **Settings** icon in the header and select **Demo settings**.</span></span> <span data-ttu-id="60096-118">此外，您還可以變更視覺佈景主題。</span><span class="sxs-lookup"><span data-stu-id="60096-118">Additionally, you can change the visual theme.</span></span> 

<span data-ttu-id="60096-119">您可[切換至此環境](#switch-environments) (進行註冊程序時所建立的環境)，以使用您自己的資料。</span><span class="sxs-lookup"><span data-stu-id="60096-119">You [switch to the environment](#switch-environments) you created during the sign-up process to work with your own data.</span></span>

## <a name="create-a-new-production-or-sandbox-environment"></a><span data-ttu-id="60096-120">建立新的生產或沙箱環境</span><span class="sxs-lookup"><span data-stu-id="60096-120">Create a new production or sandbox environment</span></span>

<span data-ttu-id="60096-121">在您的環境中，選取應用程式標頭中的 **環境** 選取器，然後選取 **新增**。</span><span class="sxs-lookup"><span data-stu-id="60096-121">In your environment, select the **Environments** picker in the app header and select **New**.</span></span>

<span data-ttu-id="60096-122">依照您[建立試用環境](#create-a-trial-environment)時的步驟操作。</span><span class="sxs-lookup"><span data-stu-id="60096-122">Follow the steps as if you [create a trial environment](#create-a-trial-environment).</span></span> <span data-ttu-id="60096-123">根據預設，資料會儲存在 Customer Insights 管理的資料湖中。</span><span class="sxs-lookup"><span data-stu-id="60096-123">By default, data is stored in the Customer Insights managed data lake.</span></span> <span data-ttu-id="60096-124">選取 **進階設定** 時，您會看到可用來將資料儲存在您自己的 Azure Data Lake 中的其他選項。</span><span class="sxs-lookup"><span data-stu-id="60096-124">You get an additional option when selecting **Advanced settings** to store your data in your own Azure Data Lake.</span></span> <span data-ttu-id="60096-125">提供您的帳戶名稱及帳戶金鑰，以建立與 Azure Data Lake 的連接。</span><span class="sxs-lookup"><span data-stu-id="60096-125">Provide your account name and account key to establish a connection to your Azure Data Lake.</span></span> 

> [!IMPORTANT]
> <span data-ttu-id="60096-126">將資料儲存至您的 Azure Data Lake Storage，即表示您同意將資料傳送並儲存在相應的 Azure 儲存體帳戶的地理位置，這可能不同於將資料儲存於 Dynamics 365 Customer Insights 中的位置。</span><span class="sxs-lookup"><span data-stu-id="60096-126">By saving data to your Azure Data Lake Storage, you agree that data will be transferred to and stored in the appropriate geographic location for that Azure storage account, which may differ from where data is stored in Dynamics 365 Customer Insights.</span></span> [<span data-ttu-id="60096-127">在 Microsoft 信任中心深入了解。</span><span class="sxs-lookup"><span data-stu-id="60096-127">Learn more at the Microsoft Trust Center.</span></span>](https://www.microsoft.com/trust-center)

## <a name="explore-the-home-page"></a><span data-ttu-id="60096-128">探索首頁</span><span class="sxs-lookup"><span data-stu-id="60096-128">Explore the home page</span></span>

<span data-ttu-id="60096-129">您可以 [在 Dynamics 365 Customer Insights 存取對象見解](https://home.ci.ai.dynamics.com/)，請到下列 URL：[https://home.ci.ai.dynamics.com/](https://home.ci.ai.dynamics.com/)。</span><span class="sxs-lookup"><span data-stu-id="60096-129">You can [access audience insights from Dynamics 365 Customer Insights](https://home.ci.ai.dynamics.com/) on the following URL: [https://home.ci.ai.dynamics.com/](https://home.ci.ai.dynamics.com/).</span></span>
<span data-ttu-id="60096-130">在完成 [對應](map-entities.md)、[比對](match-entities.md)和 [合併](merge-entities.md)階段之後，**首頁** 就會顯示客戶細分、量值和擴充資料 (如果已設定) 的概觀。</span><span class="sxs-lookup"><span data-stu-id="60096-130">The **Home** page shows an overview of segments, measures, and enrichment data (if configured)after completing the [map](map-entities.md), [match](match-entities.md), and [merge](merge-entities.md) phases.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="60096-131">![首頁上的見解](media/home-page-insights.png "首頁上的見解")</span><span class="sxs-lookup"><span data-stu-id="60096-131">![Insights on Home page](media/home-page-insights.png "Insights on Home page")</span></span>

<span data-ttu-id="60096-132">在 **最新客戶細分** 底下，您可以根據您定義的人口統計、行為或交易屬性來查看客戶群組。</span><span class="sxs-lookup"><span data-stu-id="60096-132">Under **Recent segments**, you see groups of customers based on demographic, behavioral, or transactional attributes that you've defined.</span></span> <span data-ttu-id="60096-133">[建立客戶細分](segments.md)可協助您將您的客戶群分組，並找出更好的商務活動的目標。</span><span class="sxs-lookup"><span data-stu-id="60096-133">[Creating segments](segments.md) helps you to group your customer base and better target your business activities.</span></span>

<span data-ttu-id="60096-134">**最近量值** 會顯示您已定義的[關鍵效能指標(KPI) ](measures.md)圖格。</span><span class="sxs-lookup"><span data-stu-id="60096-134">**Recent measures** show tiles with [key performance indicators (KPIs)](measures.md) that you've defined.</span></span> <span data-ttu-id="60096-135">例如，客戶流失的平均可能性或每位客戶的平均上網消費量。</span><span class="sxs-lookup"><span data-stu-id="60096-135">For example, average likelihood of a customer to churn or the average online spend per customer.</span></span>

<span data-ttu-id="60096-136">**最新擴充** 區段會列出最近完成的擴充執行結果。</span><span class="sxs-lookup"><span data-stu-id="60096-136">The **Recent enrichments** section lists the results of the enrichment runs that completed recently.</span></span> <span data-ttu-id="60096-137">[擴充](enrichment-hub.md) 會新增關於您的客戶群的資訊。</span><span class="sxs-lookup"><span data-stu-id="60096-137">[Enrichments](enrichment-hub.md) add information about your customer base.</span></span> <span data-ttu-id="60096-138">例如，了解他們喜好的興趣和品牌。</span><span class="sxs-lookup"><span data-stu-id="60096-138">For example, by understanding the interests and brands that they have affinity for.</span></span>

## <a name="switch-environments"></a><span data-ttu-id="60096-139">切換環境</span><span class="sxs-lookup"><span data-stu-id="60096-139">Switch environments</span></span>

<span data-ttu-id="60096-140">選取頁面右上角的 **環境** 控制項，以變更環境。</span><span class="sxs-lookup"><span data-stu-id="60096-140">Select the **Environment** control in the upper-right corner of the page to change environments.</span></span>

> [!div class="mx-imgBorder"] 
> <span data-ttu-id="60096-141">![切換環境](media/home-page-environment-switcher.png "切換環境")</span><span class="sxs-lookup"><span data-stu-id="60096-141">![Switch environment](media/home-page-environment-switcher.png "Switch environment")</span></span>

<span data-ttu-id="60096-142">系統管理員可以建立和管理[多個環境 ](manage-environments.md)。</span><span class="sxs-lookup"><span data-stu-id="60096-142">Administrators can create and manage [multiple environments](manage-environments.md).</span></span> <span data-ttu-id="60096-143">例如，如果您的組織跨國營運，而您需要以不同的方式隔離資料與見解時，維護多個環境可能會很有用。</span><span class="sxs-lookup"><span data-stu-id="60096-143">Maintaining more than one environment may be useful if, for example, your organization operates internationally and you need to segregate data and insights in different ways.</span></span>

## <a name="next-step"></a><span data-ttu-id="60096-144">後續步驟</span><span class="sxs-lookup"><span data-stu-id="60096-144">Next step</span></span>

<span data-ttu-id="60096-145">若要在首頁查看您自己的見解，必須先[新增資料來源](data-sources.md)，然後[統整](data-unification.md)資料以建立客戶設定檔。</span><span class="sxs-lookup"><span data-stu-id="60096-145">To see your own insights on the home page, you'll first need to [add data sources](data-sources.md) and [unify](data-unification.md) your data to build customer profiles.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]