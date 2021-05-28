---
title: 匯出 Customer Insights 資料到 Facebook Ads Manager
description: 了解如何設定連接並匯出至 Facebook 廣告管理員。
ms.date: 04/15/2021
ms.reviewer: mhart
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: how-to
author: pkieffer
ms.author: philk
manager: shellyha
ms.openlocfilehash: 37d25aa038ea32b98f2d1850d7b42b701292438d
ms.sourcegitcommit: e8e03309ba2515374a70c132d0758f3e1e1851d0
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 05/04/2021
ms.locfileid: "5976069"
---
# <a name="export-segments-list-to-facebook-ads-manager-preview"></a><span data-ttu-id="3d22d-103">將客戶細分清單匯出至 Facebook 廣告管理員 (預覽版)</span><span class="sxs-lookup"><span data-stu-id="3d22d-103">Export segments list to Facebook Ads Manager (preview)</span></span>

<span data-ttu-id="3d22d-104">將統一客戶設定檔的區段匯出至 Facebook 廣告管理員，以建立 Facebook 和 Instagram 上的行銷活動。</span><span class="sxs-lookup"><span data-stu-id="3d22d-104">Export segments of unified customer profiles to Facebook Ads Manager to create campaigns on Facebook and Instagram.</span></span>

## <a name="prerequisites-for-connection"></a><span data-ttu-id="3d22d-105">連接的先決條件</span><span class="sxs-lookup"><span data-stu-id="3d22d-105">Prerequisites for connection</span></span>

- <span data-ttu-id="3d22d-106">您必須擁有 [**Facebook 廣告帳戶**](https://www.facebook.com/business/learn/lessons/step-by-step-ads-manager-account) 且其中要包含 [**Facebook 商務帳戶**](https://business.facebook.com/)。</span><span class="sxs-lookup"><span data-stu-id="3d22d-106">You need to have a [**Facebook Ad Account**](https://www.facebook.com/business/learn/lessons/step-by-step-ads-manager-account) that includes a [**Facebook Business Account**](https://business.facebook.com/).</span></span>
- <span data-ttu-id="3d22d-107">您在 [**Facebook 廣告帳戶**](https://www.facebook.com/business/learn/lessons/step-by-step-ads-manager-account) 上必須是管理員身份。</span><span class="sxs-lookup"><span data-stu-id="3d22d-107">You need to be an administrator on the [**Facebook Ad Account**](https://www.facebook.com/business/learn/lessons/step-by-step-ads-manager-account).</span></span>

## <a name="known-limitations"></a><span data-ttu-id="3d22d-108">已知限制</span><span class="sxs-lookup"><span data-stu-id="3d22d-108">Known limitations</span></span>

- <span data-ttu-id="3d22d-109">每次最多可匯出 1 千萬份客戶個人資料至 Facebook 廣告管理員。</span><span class="sxs-lookup"><span data-stu-id="3d22d-109">Up to 10 million customer profile per export to Facebook Ads Manager.</span></span>
- <span data-ttu-id="3d22d-110">僅客戶細分可以匯出到 Facebook 廣告管理員。</span><span class="sxs-lookup"><span data-stu-id="3d22d-110">Export to Facebook Ads Manager is limited to segments.</span></span>
- <span data-ttu-id="3d22d-111">僅能在 Facebook 建立或更新 *客戶清單* 類型中的自訂對象。</span><span class="sxs-lookup"><span data-stu-id="3d22d-111">Create or update custom audiences in Facebook of type *customer list* only.</span></span>
- <span data-ttu-id="3d22d-112">匯出總計 1 千萬份個人資料的客戶細分可能需要 90 分鐘完成。</span><span class="sxs-lookup"><span data-stu-id="3d22d-112">Exporting segments with a total of 10 million profiles can take up to 90 minutes to complete.</span></span>

## <a name="set-up-connection-to-facebook-ads-manager"></a><span data-ttu-id="3d22d-113">設定與 Facebook 廣告管理員的連接</span><span class="sxs-lookup"><span data-stu-id="3d22d-113">Set up connection to Facebook Ads Manager</span></span>

<span data-ttu-id="3d22d-114">系統管理員必須設定與服務的連接，並允許參與者使用該連接，使用者才能建立匯出。</span><span class="sxs-lookup"><span data-stu-id="3d22d-114">Before users can create an export, an administrator must configure the connection to the service and allow contributors to use the connection.</span></span>

1. <span data-ttu-id="3d22d-115">移至 **管理** > **連接**。</span><span class="sxs-lookup"><span data-stu-id="3d22d-115">Go to **Admin** > **Connections**.</span></span>

1. <span data-ttu-id="3d22d-116">選取 **新增連接**，然後選擇 **Facebook 廣告管理員** 來設定連接。</span><span class="sxs-lookup"><span data-stu-id="3d22d-116">Select **Add connection** and choose **Facebook Ads Manager** to configure the connection.</span></span>

1. <span data-ttu-id="3d22d-117">在 **顯示名稱** 中，給連接一個能夠辨識的名稱。</span><span class="sxs-lookup"><span data-stu-id="3d22d-117">Give your connection a recognizable name in the **Display name** field.</span></span> <span data-ttu-id="3d22d-118">連接的名稱與類型能說明此連接。</span><span class="sxs-lookup"><span data-stu-id="3d22d-118">The name and the type of the connection describe this connection.</span></span> <span data-ttu-id="3d22d-119">我們建議您選取可以說明此連接用途和目標的名稱。</span><span class="sxs-lookup"><span data-stu-id="3d22d-119">We recommend choosing a name that explains the purpose and target of the connection.</span></span>

1. <span data-ttu-id="3d22d-120">選擇可使用此連接的人員。</span><span class="sxs-lookup"><span data-stu-id="3d22d-120">Choose who can use this connection.</span></span> <span data-ttu-id="3d22d-121">如果您不採取任何動作，預設值將為 **系統管理員**。</span><span class="sxs-lookup"><span data-stu-id="3d22d-121">If you take no action, the default will be **Administrators**.</span></span> <span data-ttu-id="3d22d-122">如需詳細資訊，請參閱[允許參與者使用匯出的連接](connections.md#allow-contributors-to-use-a-connection-for-exports)。</span><span class="sxs-lookup"><span data-stu-id="3d22d-122">For more information, see [Allow contributors to use a connection for exports](connections.md#allow-contributors-to-use-a-connection-for-exports).</span></span>

1. <span data-ttu-id="3d22d-123">進行 Facebook 廣告驗證：</span><span class="sxs-lookup"><span data-stu-id="3d22d-123">Authenticate with Facebook Ads:</span></span> 

   1. <span data-ttu-id="3d22d-124">選取 **繼續使用 Facebook** 登入您的 Facebook 廣告帳戶。</span><span class="sxs-lookup"><span data-stu-id="3d22d-124">Select **Continue with Facebook** to sign in to your Facebook Ad Account.</span></span>

   1. <span data-ttu-id="3d22d-125">使用 Facebook 驗證之後，允許 **ads_management** 權限。</span><span class="sxs-lookup"><span data-stu-id="3d22d-125">Allow the **ads_management** permission after authenticating with Facebook.</span></span>

   1. <span data-ttu-id="3d22d-126">選取您要使用的 **Facebook 廣告帳戶**。</span><span class="sxs-lookup"><span data-stu-id="3d22d-126">Select the **Facebook Ads Account** that you want to work with.</span></span>

   1. <span data-ttu-id="3d22d-127">從下拉式清單選取 **現有的自訂對象**，或建立 **新的自訂對象**。</span><span class="sxs-lookup"><span data-stu-id="3d22d-127">Select an **Existing custom audience** from the drop-down list or create a **New custom audience**.</span></span> <span data-ttu-id="3d22d-128">如需詳細資訊，請參閱 [**Facebook 廣告管理員中的對象**](https://www.facebook.com/business/help/744354708981227?id=2469097953376494)。</span><span class="sxs-lookup"><span data-stu-id="3d22d-128">For more information, see [**Audiences in Facebook Ads Manager**](https://www.facebook.com/business/help/744354708981227?id=2469097953376494).</span></span>
      > [!NOTE]
      > <span data-ttu-id="3d22d-129">使用此匯出，您只能在 Facebook 建立或更新 *客戶清單* 類型中的自訂對象。</span><span class="sxs-lookup"><span data-stu-id="3d22d-129">You can only create or update custom audiences on Facebook of the type *customer list* with this export.</span></span> <span data-ttu-id="3d22d-130">在某些案例中，您會在下拉式清單中看到不同類型的自訂對象。</span><span class="sxs-lookup"><span data-stu-id="3d22d-130">In some cases, you see custom audiences of different types in the drop-down list.</span></span> <span data-ttu-id="3d22d-131">選取與 *客戶清單* 不同的類型會導致匯出失敗。</span><span class="sxs-lookup"><span data-stu-id="3d22d-131">Selecting a different type than *customer list* will result in a failing export.</span></span> 

1. <span data-ttu-id="3d22d-132">請檢查 **資料隱私權和合規性**，並選取 **我同意**。</span><span class="sxs-lookup"><span data-stu-id="3d22d-132">Review the **Data privacy and compliance** and select **I agree**.</span></span>

1. <span data-ttu-id="3d22d-133">選取 **儲存** 來完成連接。</span><span class="sxs-lookup"><span data-stu-id="3d22d-133">Select **Save** to complete the connection.</span></span>

## <a name="configure-an-export"></a><span data-ttu-id="3d22d-134">設定匯出</span><span class="sxs-lookup"><span data-stu-id="3d22d-134">Configure an export</span></span>

<span data-ttu-id="3d22d-135">若您擁有取此類型的連接的存取權，則可以設定此匯出。</span><span class="sxs-lookup"><span data-stu-id="3d22d-135">You can configure this export if you have access to a connection of this type.</span></span> <span data-ttu-id="3d22d-136">如需詳細資訊，請參閱[設定匯出所需的權限](export-destinations.md#set-up-a-new-export)。</span><span class="sxs-lookup"><span data-stu-id="3d22d-136">For more information, see [Permissions needed to configure an export](export-destinations.md#set-up-a-new-export).</span></span>

1. <span data-ttu-id="3d22d-137">移至 **資料** > **匯出**。</span><span class="sxs-lookup"><span data-stu-id="3d22d-137">Go to **Data** > **Exports**.</span></span>

1. <span data-ttu-id="3d22d-138">若要建立新的匯出，請選取 **新增目的地**。</span><span class="sxs-lookup"><span data-stu-id="3d22d-138">To create a new export, select **Add destination**.</span></span> 

1. <span data-ttu-id="3d22d-139">在 **匯出的連接** 欄位中，在 **Facebook 廣告管理員** 區段中選擇連接。</span><span class="sxs-lookup"><span data-stu-id="3d22d-139">In **Connection for export** choose a connection from the **Facebook Ads Manager** section.</span></span> <span data-ttu-id="3d22d-140">如果您看不到此區段名稱，代表沒有此類型的連接可供您使用。</span><span class="sxs-lookup"><span data-stu-id="3d22d-140">If you don't see this section name, there are no connections of this type available to you.</span></span>

1. <span data-ttu-id="3d22d-141">在 **選擇金鑰識別元欄位** 中，選取要傳送給 Facebook 廣告管理員的 **電子郵件**、**姓名和地址** 或 **電話**。</span><span class="sxs-lookup"><span data-stu-id="3d22d-141">In the **Choose your key identifier field**, select **Email**, **Name and address**, or **Phone** to send to Facebook Ads Manager.</span></span> 

1. <span data-ttu-id="3d22d-142">在 **顯示名稱** 中，給連接一個能夠辨識的名稱。</span><span class="sxs-lookup"><span data-stu-id="3d22d-142">Give your connection a recognizable name in the **Display name** field.</span></span>

1. <span data-ttu-id="3d22d-143">從您的統一客戶實體中對應所選金鑰識別元的相應屬性。</span><span class="sxs-lookup"><span data-stu-id="3d22d-143">Map the corresponding attributes from your unified customer entity for the selected key identifier.</span></span>
   > <span data-ttu-id="3d22d-144">[提示] 如果您選取 **電子郵件** 做為金鑰識別元，則最有可能找到有相符項目。</span><span class="sxs-lookup"><span data-stu-id="3d22d-144">[TIP] The best chances for a match occur if you select **Email** as key identifier.</span></span> <span data-ttu-id="3d22d-145">新增其他識別元可能會改善比對情況。</span><span class="sxs-lookup"><span data-stu-id="3d22d-145">Adding additional identifiers may improve the matching.</span></span>

1. <span data-ttu-id="3d22d-146">選取 **新增屬性** 對應更多屬性，以傳送至 Facebook 廣告管理員。</span><span class="sxs-lookup"><span data-stu-id="3d22d-146">Select **Add attribute** to map more attributes to send to Facebook Ads Manager.</span></span> <span data-ttu-id="3d22d-147">Facebook 廣告管理員中的屬性將會對應至下列友善使用者的名稱：**FN** = **名**、**LN** = **姓氏**、**FI** = **名字字首**、**PHONE** = **電話**、**GEN** = **性別**、**DOB** = **出生日期**、**ST** = **縣/市**、**CT** = **市/鎮**、**ZIP** = **郵遞區號**、**COUNTRY** = **國家/地區**</span><span class="sxs-lookup"><span data-stu-id="3d22d-147">Attributes from Facebook Ads Manager are mapping to the following user-friendly names: **FN** = **First Name**, **LN** = **Last Name**, **FI** = **First Initial**, **PHONE** = **Phone**, **GEN** = **Gender**, **DOB** = **Date of birth**, **ST** = **State**, **CT** = **City**, **ZIP** = **Postal code / Zip code**, **COUNTRY** = **Country / Region**</span></span>

1. <span data-ttu-id="3d22d-148">選取您要匯出的客戶細分。</span><span class="sxs-lookup"><span data-stu-id="3d22d-148">Select the segments you want to export.</span></span>

1. <span data-ttu-id="3d22d-149">選取 **儲存**。</span><span class="sxs-lookup"><span data-stu-id="3d22d-149">Select **Save**.</span></span>

<span data-ttu-id="3d22d-150">儲存匯出並不會立即執行匯出。</span><span class="sxs-lookup"><span data-stu-id="3d22d-150">Saving an export doesn't run the export immediately.</span></span>

<span data-ttu-id="3d22d-151">每次[排定重新整理](system.md#schedule-tab)會一起執行匯出。</span><span class="sxs-lookup"><span data-stu-id="3d22d-151">The export runs with every [scheduled refresh](system.md#schedule-tab).</span></span> <span data-ttu-id="3d22d-152">您也可以依[需求匯出資料](export-destinations.md#run-exports-on-demand)。</span><span class="sxs-lookup"><span data-stu-id="3d22d-152">You can also [export data on demand](export-destinations.md#run-exports-on-demand).</span></span> 

## <a name="data-privacy-and-compliance"></a><span data-ttu-id="3d22d-153">資料隱私權與合規性</span><span class="sxs-lookup"><span data-stu-id="3d22d-153">Data privacy and compliance</span></span>

<span data-ttu-id="3d22d-154">當您啟用 Dynamics 365 Customer Insights 將資料傳輸給 Facebook Ads Manager 時，您允許在 Dynamics 365 Customer Insights 合規性邊界之外傳輸資料，包括潛在敏感性資料如個人資料。</span><span class="sxs-lookup"><span data-stu-id="3d22d-154">When you enable Dynamics 365 Customer Insights to transmit data to Facebook Ads Manager, you allow transfer of data outside of the compliance boundary for Dynamics 365 Customer Insights, including potentially sensitive data such as Personal Data.</span></span> <span data-ttu-id="3d22d-155">Microsoft 將依據您的指示傳輸此資料，但您須負責確保 Facebook 廣告符合您可能應盡的任何隱私權或資訊安全義務。</span><span class="sxs-lookup"><span data-stu-id="3d22d-155">Microsoft will transfer such data at your instruction, but you are responsible for ensuring that Facebook Ads meet any privacy or security obligations you may have.</span></span> <span data-ttu-id="3d22d-156">如需詳細資訊，請參閱 [Microsoft 隱私權聲明](https://go.microsoft.com/fwlink/?linkid=396732)。</span><span class="sxs-lookup"><span data-stu-id="3d22d-156">For more information, see [Microsoft Privacy Statement](https://go.microsoft.com/fwlink/?linkid=396732).</span></span>
<span data-ttu-id="3d22d-157">您的 Dynamics 365 Customer Insights 系統管理員可以隨時移除此匯出目的地，以便不再繼續使用此功能。</span><span class="sxs-lookup"><span data-stu-id="3d22d-157">Your Dynamics 365 Customer Insights Administrator can remove this export destination at any time to discontinue use of this functionality.</span></span>


[!INCLUDE[footer-include](../includes/footer-banner.md)]
