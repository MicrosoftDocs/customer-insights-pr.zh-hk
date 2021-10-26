---
title: 將 Customer Insights 資料匯出至 Omnisend
description: 了解如何設定連接並匯出至 Omnisend。
ms.date: 10/08/2021
ms.reviewer: mhart
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: conceptual
author: pkieffer
ms.author: philk
manager: shellyha
ms.openlocfilehash: 5496efa075fa3474c579366d143ea55e86ec3995
ms.sourcegitcommit: 23c8973a726b15050e368cc6e0aab78b266a89f6
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 10/08/2021
ms.locfileid: "7619055"
---
# <a name="export-segments-to-omnisend-preview"></a>將客戶細分匯出至 Omnisend (預覽版)

將整合客戶個人資料的客戶細分匯出至 Omnisend，並用於行銷活動。

## <a name="prerequisites"></a>先決條件

-   您擁有一個 [Omnisend 帳戶](https://www.omnisend.com/)及對應的系統管理員認證。
-   您在對象見解中具有 [組態區域](segments.md) 權限。
-   匯出區段的統一客戶設定檔包含代表電子郵件地址的欄位。

## <a name="known-limitations"></a>已知限制

- 您最多可以匯出 1 百萬個客戶設定檔到 Omnisend，它需要長達 4 小時完成。
- 匯出到 Omnisend 時，會被限制為客戶細分。
- 您可以匯出到 Omnisend 的客戶設定檔數目取決於您和 Omnisend 簽訂的契約。

## <a name="set-up-connection-to-omnisend"></a>設定與 Omnisend 的連接

1. 移至 **管理** > **連接**。

1. 選取 **新增連接**，然後選擇 **Omnisend** 來設定連接。

1. 在 **顯示名稱** 中，給連接一個能夠辨識的名稱。 連接的名稱與類型能說明此連接。 我們建議您選取可以說明此連接用途和目標的名稱。

1. 選擇可使用此連接的人員。 根據預設，只有系統管理員。 如需詳細資訊，請參閱[允許參與者使用匯出的連接](connections.md#allow-contributors-to-use-a-connection-for-exports)。

1. 請輸入您的 [Omnisend API 金鑰](https://support.omnisend.com/en/articles/1061890-generating-api-key).

1. 選取 **我同意** 以確認 **資料隱私權與合規性**。

1. 選取 **連接** 來初始化與 Omnisend 的連接。

1. 選取 **將您自己新增為匯出使用者** 並提供您的 Customer Insights 認證。

1. 選取 **儲存** 來完成連接。

## <a name="configure-an-export"></a>設定匯出

若您擁有取此類型的連接的存取權，則可以設定此匯出。 如需詳細資訊，請參閱[設定匯出所需的權限](export-destinations.md#set-up-a-new-export)。

1. 移至 **資料** > **匯出**。

1. 若要建立新的匯出，請選取 **新增目的地**。

1. 在 **匯出的連結** 欄位中，在 Omnisend 區段中選擇連接。 如果您看不到此區段名稱，代表沒有此類型的連接可供您使用。

1. 請在 **資料相符** 分段的 **電子郵件** 欄位中選取代表客戶電子郵件地址的欄位。 這必須匯出客戶細分到 Omnisend。 或者，您可以匯出名、姓、地址、國家/地區、市/鎮、縣/市、郵遞區號，以建立更多的個人化電子郵件。 選取 **新增屬性** 對應這些欄位。

1. 選取 **儲存**。

儲存匯出並不會立即執行匯出。

每次[排定重新整理](system.md#schedule-tab)會一起執行匯出。 您也可以依[需求匯出資料](export-destinations.md#run-exports-on-demand)。 


## <a name="data-privacy-and-compliance"></a>資料隱私權與合規性

當您啟用 Dynamics 365 Customer Insights 將資料傳輸至 Omnisend 時，您允許傳輸資料到 Dynamics 365 Customer Insights 合規性邊界之外，包括潛在的敏感性資料 (例如個人資料)。 Microsoft 將會在您的指示下傳送這類資料，但是您必須負責確保 Omnisend 符合您可能會承擔的任何隱私權或資訊安全義務。 如需詳細資訊，請參閱 [Microsoft 隱私權聲明](https://go.microsoft.com/fwlink/?linkid=396732)。

您的 Dynamics 365 Customer Insights 系統管理員可以隨時移除此匯出目的地，不再繼續使用此功能。
