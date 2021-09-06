---
title: 將 Customer Insights 資料匯出至 LinkedIn Ads
description: 了解如何設定連接並匯出至 LinkedIn Ads。
ms.date: 05/12/2021
ms.reviewer: mhart
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: conceptual
author: pkieffer
ms.author: philk
manager: shellyha
ms.openlocfilehash: 2cfaa37fd0ac697f29665792bab27a925d8ea1eede0519d424524a7e5accbfeb
ms.sourcegitcommit: aa0cfbf6240a9f560e3131bdec63e051a8786dd4
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 08/10/2021
ms.locfileid: "7034250"
---
# <a name="export-segments-to-linkedin-ads-preview"></a>將客戶細分匯出至 LinkedIn Ads (預覽版)

將整合客戶個人資料的客戶細分匯出至LinkedIn Ads，以建立符合的對象。 使用符合對象給公司鎖定和連絡人鎖定。

## <a name="prerequisites"></a>先決條件

-   您擁有一個　[LinkedIn Campaign Manager 帳戶](https://business.linkedin.com/marketing-solutions/ads) 及對應的系統管理員認證。
-   您在對象見解中具有 [組態區域](segments.md) 權限。
-   在匯出客戶細分中的客戶個人資料，包含有電子郵件地址的欄位。

## <a name="known-limitations"></a>已知限制

- 每次匯出中您最多可以將 10 萬筆個人資料匯出至 LinkedIn Ads。
- 匯出到 LinkedIn Ads 時，會被限制為客戶細分。
- 將最多 10 萬筆個人資料匯出至 LinkedIn Ads 可能需要花費 10 分鐘的時間才能完成。 

## <a name="set-up-the-connection-to-linkedin-ads"></a>設定連線至 LinkedIn Ads

1. 在對象見解中，移至 **管理** > **連接**。

1. 選取 **新增連接**，然後選擇 **LinkedIn Ads** 來設定連接。

1. 在 **顯示名稱** 中，給連接一個能夠辨識的名稱。 連接的名稱與類型能說明此連接。 我們建議您選取可以說明此連接用途和目標的名稱。

1. 選擇可使用此連接的人員。 如果您不採取任何動作，預設值是系統管理員。 如需詳細資訊，請參閱[允許參與者使用匯出的連接](connections.md#allow-contributors-to-use-a-connection-for-exports)。

1. 提供您的 [LinkedIn Campaign Manager 帳戶識別碼](https://www.linkedin.com/help/lms/answer/a424270)。

1. 選取 **我同意** 以確認 **資料隱私權與合規性**。

1. 選取 **連接** 來初始化與 Campaign Monitor 的連接。

1. 選取 **驗證 LinkedIn**，並提供 LinkedIn Campaign Manager 的系統管理員認證。

1. 選取 **將您自己新增為匯出使用者** 並提供您的 Customer Insights 認證。

1. 選取 **儲存** 來完成連接。

## <a name="configure-an-export"></a>設定匯出

若您擁有取此類型的連接的存取權，則可以設定此匯出。 如需詳細資訊，請參閱[設定匯出所需的權限](export-destinations.md#set-up-a-new-export)。

1. 移至 **資料** > **匯出**。

1. 若要建立新的匯出，請選取 **新增目的地**。

1. 在 **匯出的連結** 欄位中，在 LinkedIn Ads 區段中選擇連接。 如果您看不到此區段名稱，代表沒有此類型的連接可供您使用。

1. 選擇您是否要匯出資料，以執行 LinkedIn 上的[連絡人鎖定](https://business.linkedin.com/marketing-solutions/ad-targeting/contact-targeting)或[公司鎖定](https://business.linkedin.com/marketing-solutions/ad-targeting/account-targeting)。 

1. 在 **資料比對** 區段的電子郵件欄位中，在您的整合客戶個人資料中，選取呈現客戶的電子郵件地址欄位。 這必須匯出客戶細分到 LinkedIn Ads。

1. 選取您要匯出的客戶細分。 使用您選取要匯出的區段名稱，LinkedIn Campaign Manager 中的符合對象會自動建立。 每一個客戶細分都會造成不同的符合對象。 

1. 選取 **儲存**。

儲存匯出並不會立即執行匯出。

每次[排定重新整理](system.md#schedule-tab)會一起執行匯出。 您也可以依[需求匯出資料](export-destinations.md#run-exports-on-demand)。 


## <a name="data-privacy-and-compliance"></a>資料隱私權與合規性

當您啟用 Dynamics 365 Customer Insights 將資料傳輸至 LinkedIn Ads 時，您允許傳輸資料到 Dynamics 365 Customer Insights 合規性邊界之外，包括潛在的敏感性資料 (例如個人資料)。 Microsoft 將會在您的指示下傳送這類資料，但是您必須負責確保 LinkedIn Ads 符合您可能會承擔的任何隱私權或資訊安全義務。 如需詳細資訊，請參閱 [Microsoft 隱私權聲明](https://go.microsoft.com/fwlink/?linkid=396732)。

您的 Dynamics 365 Customer Insights 系統管理員可以隨時移除此匯出目的地，停止使用此功能。
