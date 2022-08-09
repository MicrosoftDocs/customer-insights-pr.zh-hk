---
title: 連接 (預覽版) 概觀
description: 從 Customer Insights 連接到其他服務。
ms.date: 04/09/2021
ms.reviewer: nikeller
ms.subservice: audience-insights
ms.topic: overview
author: m-hartmann
ms.author: mhart
manager: shellyha
searchScope:
- ci-connections
- customerInsights
ms.openlocfilehash: 4a0bc5dd4100b462a26660a0c51fda1fe92b6bb9
ms.sourcegitcommit: 594081c82ca385f7143b3416378533aaf2d6d0d3
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 07/27/2022
ms.locfileid: "9195201"
---
# <a name="connections-preview-overview"></a>連接 (預覽版) 概觀

連接是與 Customer Insights 啟用資料共用的關鍵。 每個連接都會對特定服務建立資料共用。 連接是[設定協力廠商擴充](enrichment-hub.md)和[設定匯出](export-destinations.md)的基礎。 同一個連接可以多次使用。 例如，一個對 Dynamics 365 Marketing 的連結可用於多個匯出，而另一個對 Leadspace 的連接可以用來進行多個擴充。

移至 **管理** > **連接** 以建立和查看連接。

**連接** 索引標籤顯示出所有使用中的連接。 每個連接顯示為清單上的一列。

取得簡易概觀、說明，以及使用 **探索** 索引標籤上的每個擴充性選項，了解可以執行的動作。

## <a name="data-privacy-and-compliance"></a>資料隱私權與合規性

當您啟用 Dynamics 365 Customer Insights 將資料傳輸至協力廠商或其他 Microsoft 產品時，您允許傳輸資料到 Dynamics 365 Customer Insights 合規性邊界之外，包括潛在的敏感性資料 (例如個人資料)。 Microsoft 將依據您的指示傳輸此資料，但您須負責確保協力廠商符合您可能應盡的任何隱私權或資訊安全義務。 如需詳細資訊，請參閱 [Microsoft 隱私權聲明](https://go.microsoft.com/fwlink/?linkid=396732)。

您的 Dynamics 365 Customer Insights 管理員可以隨時移除此連線，不再繼續使用該功能。

## <a name="exports"></a>匯出

只有系統管理員可以設定新的連接，但是他們可以將使用現有連接的存取權授予給參與者。 系統管理員控制資料的流向，參與者定義符合其需求的酬載和頻率。 如需詳細資訊，請參閱[允許參與者使用匯出的連接](#allow-contributors-to-use-a-connection-for-exports)。

## <a name="enrichments"></a>擴充

只有系統管理員才可以設定新的連接，但是所建立的連接都可供系統管理員和參與者使用。 系統管理員能管理認證並同意資料傳輸。 系統管理員和參與者都可以使用這些連接進行擴充。

## <a name="add-a-new-connection"></a>新增連接

若要新增連接，您必須具備[系統管理員權限](permissions.md)。 如果您連至其他 Microsoft 服務，我們預設這兩個服務位於相同的組織中。

1. 移至 **管理** > **連接 (預覽版)**。

1. 請選取 **新增連接** 建立新連接。 從下拉式功能表中選擇您要建立的連接類型。

1. 在 **設定連接** 窗格中，提供必要的詳細資料。
   1. 以連結的 **顯示名稱** 與類型設定連接。 我們建議您選取可以說明此連接用途和目標的名稱。
   1. 確切的欄位會視您要連接的服務而定。 在目標服務的相關文章中，可以了解特定連接的詳細資料。
   1. 如果您 [使用自己的金鑰保存庫](use-azure-key-vault.md)儲存祕密，請使用 **金鑰保存庫** 並從清單選擇祕密。

1. 選取 **儲存** 建立連結。

您也可以在 **探索** 索引標籤中選取圖標上的 **設定**。

### <a name="allow-contributors-to-use-a-connection-for-exports"></a>允許參與者使用匯出連接

設定或編輯匯出連接時，定義[匯出](export-destinations.md)要選擇允許哪些使用者使用此特定連接。 根據預設，具有系統管理員角色的使用者可以使用連接。 您可以在 **選取能使用此連接的人員** 下變更此設定，並允許具備參與者角色的使用者使用此連接。

- 參與者無法查看或編輯該連接。 在建立匯出時，他們只能看到顯示名稱及其類型。
- 透過共用連接，您可以讓參與者使用連接。 當參與者設定匯出時，會看到共用的連接。 他們可以管理使用此特定連接的每個匯出。
- 您可以保留參與者已定義的匯出，並變更此設定。

## <a name="edit-a-connection"></a>編輯連接

1. 移至 **管理** > **連接 (預覽版)**。

1. 移至 **連結** 索引標籤。

1. 對要編輯的連接，選取其垂直省略符號 (&vellip;)。

1. 選取 **編輯**。

1. 變更想要更新的值並選取 **儲存**。

## <a name="remove-a-connection"></a>移除連接

如果您要移除的連接是由擴充或匯出使用，您必須先將它們中斷連結或移除。 移除對話方塊將引導您到相關的擴充或匯出。

分離的擴充和匯出會變成停用。 您可以在[擴充](enrichment-hub.md)或[匯出](export-destinations.md)頁面上新增另一個連接給它們，以重新啟動。

1. 移至 **管理** > **連接 (預覽版)**。

1. 移至 **連結** 索引標籤。

1. 對要移除的連接，選取其垂直省略符號 (&vellip;)。

1. 從下拉式功能表中選取 **移除**。 確認對話方塊隨即出現。

   1. 如果有擴充或匯出使用此連接，請選取按鈕，以查看正在使用此連接的功能。
      - **匯出：** 要移除該連接，您可以對匯出選擇移除或中斷連接。 若要將匯出中斷連接，系統管理員可以使用 **中斷連接** 動作。 此動作可使用在選取單一和多個匯出。 中斷連接將保留匯出設定，但除非新增另一個連接至匯出，否則不會執行匯出。
      - **擴充：** 要移除該連接，您可以對擴充選擇移除或停用連接。
   1. 當連接不再有其他相依性時，請回到 **管理** > **連結**，然後嘗試再次移除該連接。

1. 請選取 **刪除**，來確認刪除。

## <a name="set-up-connections-with-secrets-managed-by-your-own-key-vault"></a>請借助您自己的金鑰保存庫管理的祕密設定連接

某些連接需要像 API 金鑰或密碼之類的祕密。 某些連接支援儲存在您自己金鑰保存庫的祕密。 了解更多支援的連接及在如何在[金鑰保存庫上設定 Customer Insights](use-azure-key-vault.md)。

[!INCLUDE [footer-include](includes/footer-banner.md)]
