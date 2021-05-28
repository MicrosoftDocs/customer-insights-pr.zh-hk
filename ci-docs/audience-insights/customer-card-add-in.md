---
title: Dynamics 365 應用程式的客戶卡片增益集
description: 以此增益集顯示位於 Dynamics 365 應用程式中的對象見解資料。
ms.date: 05/18/2021
ms.reviewer: mhart
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: conceptual
author: pkieffer
ms.author: philk
manager: shellyha
ms.openlocfilehash: 88492943ddbf9ae30c64d92b261433b74f34f682
ms.sourcegitcommit: d74430270f1b754322287c4f045d7febdae35be2
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 05/18/2021
ms.locfileid: "6059615"
---
# <a name="customer-card-add-in-preview"></a>客戶卡片增益集 (預覽)

[!INCLUDE [cc-data-platform-banner](../includes/cc-data-platform-banner.md)]

直接在 Dynamics 365 應用程式中取得您客戶的 360 度視圖。 在可支援的 Dynamics 365 應用程式中安裝客戶卡片增益集，您可以選擇顯示人口統計資訊、見解及活動時間軸。 增益集將從 Customer Insights 擷取資料，對被連接的 Dynamics 365 應用程式，不會影響其中的資料。 

## <a name="prerequisites"></a>先決條件

- 增益集只適用在 Dynamics 365 模型導向應用程式 (例如 Sales 或 Customer Service)，版本 9.0 或更新的版本。
- 為了讓您的 Dynamics 365 資料對應至對象見解客戶個人資料，這些資料需要 [從 Dynamics 365 應用程式使用 Common Data Service 連接器進行內嵌](connect-power-query.md)。
- 客戶卡片增益集的 Dynamics 365 使用者全部都必須[新增為](permissions.md)對象見解的使用者，才能查看資料。
- 在對象見解中必要有[完成設定的搜尋和篩選功能](search-filter-index.md)才能查詢用來作業的資料。
- 每個增益集控制項都依賴對象見解中的特定資料：
  - 量值控制項：需要 [組態的量值](measures.md)。
  - 智慧控制項：需要使用[預測](predictions.md)或[自訂模型](custom-models.md)生成資料。
  - 人口統計控制項：在統整的客戶設定檔中可以使用人口統計欄位 (如年齡或性別)。
  - 擴充控制項：需要將使用中[擴充內容](enrichment-hub.md)套用至客戶設定檔。
  - 時間表控制項：需要 [已組態的活動](activities.md)。

## <a name="install-the-customer-card-add-in"></a>安裝客戶卡片增益集

客戶卡片增益集是 Dynamics 365 中 Customer Engagement 應用程式的解決方案。 若要安裝此解決方案，請移至 AppSource 並搜尋 **Dynamics Customer 卡片**。 選取 [AppSource 上的客戶卡片增益集](https://appsource.microsoft.com/product/dynamics-365/mscrm.dynamics_365_customer_insights_customer_card_addin?tab=Overview)，然後選取 **立即取得**。

您可能必須使用 Dynamics 365 應用程式的系統管理員認證登入，才能安裝解決方案。

若要將解決方案安裝到您的環境，可能需要花費一些時間。

## <a name="configure-the-customer-card-add-in"></a>設定客戶卡片增益集

1. 以系統管理員身分，移至 Dynamics 365 中的 **設定** 區段，然後選取 **解決方案**。

1. 選取 **Dynamics 365 Customer Insights 客戶卡片增益集 (預覽)** 解決方案的 **顯示名稱** 連結。

   > [!div class="mx-imgBorder"]
   > ![選取顯示名稱](media/select-display-name.png "選取顯示名稱")

1. 選取 **登入**，然後輸入您用來設定 Customer Insights 的管理帳戶憑證。

   > [!NOTE]
   > 請檢查當您選取 **登入** 按鈕時，瀏覽器快顯封鎖程式不會封鎖驗證視窗。

1. 選取您要從中提取資料的 Customer Insights 環境。

1. 在 Dynamics 365 應用程式中定義記錄對欄位的對應。 視 Customer Insights 中的資料而定，您可以選擇對應下列選項：
   - 若要對應連絡人，請選取客戶實體中符合您的連絡人實體的識別碼欄位。
   - 若要對應帳戶，請選取客戶實體中符合您的帳戶實體的識別碼欄位。

   > [!div class="mx-imgBorder"]
   > ![連絡人識別碼欄位](media/contact-id-field.png "連絡人識別碼欄位")

1. 選取 **儲存設定** 以儲存設定。

1. 接下來，您必須指派 Dynamics 365 中的資訊安全角色，才能讓使用者自訂並查看客戶卡片。 在 Dynamics 365 中，移至 **設定** > **安全性** > **使用者**。 選取要編輯使用者角色的使用者，並選取 **管理角色**。

1. 將 **Customer Insights 卡片自訂員** 角色指派給要為整個組織自訂卡片顯示內容的使用者。

## <a name="add-customer-card-controls-to-forms"></a>新增客戶卡片控制項到表單
  
1. 若要將客戶卡片控制項新增至您的連絡人表單，請移至 Dynamics 365 中的 **設定** > **自訂**。

1. 選取 **自訂系統**。

1. 瀏覽至 **連絡人** 實體，展開它，然後選取 **表單**。

1. 選取您要新增客戶卡片控制項的連絡人表單。

    > [!div class="mx-imgBorder"]
    > ![選取連絡人表單](media/contact-active-forms.png "選取連絡人表單")

1. 若要新增控制項，請在表單編輯器中，將 **欄位總管** 中的任何欄位拖曳至要您希望控制項出現的位置。

1. 選取表單上您剛新增的欄位，然後選取 **變更屬性**。

1. 移至 **控制項** 索引標籤，然後選取 **新增控制項**。 選擇其中一個可用的自訂控制項，然後選取 **新增**。

1. 在 **欄位屬性** 對話方塊中，清除 **顯示表單的標籤** 核取方塊。

1. 選取控制項的 **Web** 選項。 對於擴充控制項，您可以設定 **enrichmentType** 欄位，以選取要顯示的擴充內容類型。 為每個擴充類型新增擴充控制項。

1. 選取 **儲存** 和 **發佈** 以發佈更新的連絡人表單。

1. 移至發行的連絡人表單。 您會看到最新新增的控制項。 您可能需要在第一次使用時登入。

1. 若要自訂想要在自訂控制項上顯示的內容，請在右上角選取編輯按鈕。

## <a name="upgrade-customer-card-add-in"></a>升級客戶卡片增益集
客戶卡片增益集不會自動升級。 若要升級為最新版本，請在已安裝增益集的 Dynamics 365 應用程式中執行此步驟。

1. 在 Dynamics 365 應用程式中，移至 **設定** > **自訂**，然後選取 **解決方案**。

1. 在增益集表格中尋找 **CustomerInsightsCustomerCard**，並選取該資料列。

1. 在動作列中選取 **套用解決方案升級**。

   :::image type="content" source="media/customer-card-add-in-upgrade.png" alt-text="在 Dynamics 365 應用程式的自訂區域中升級解決方案":::

1. 開始升級程序之後，會顯示載入指標直到升級完成。 如果不存在可更新的版本，會出現升級錯誤訊息。


[!INCLUDE[footer-include](../includes/footer-banner.md)]
