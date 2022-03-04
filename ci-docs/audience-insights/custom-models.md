---
title: 自訂機器學習模型 | Microsoft Docs
description: 在 Dynamics 365 Customer Insights 中使用 Azure Machine Learning 的自訂模型。
ms.date: 12/01/2021
ms.reviewer: mhart
ms.subservice: audience-insights
ms.topic: tutorial
author: zacookmsft
ms.author: zacook
manager: shellyha
searchScope:
- ci-custom-models
- customerInsights
ms.openlocfilehash: 460b68e1e65b3033af0a03d1bcc27e718c79d7aa
ms.sourcegitcommit: 73cb021760516729e696c9a90731304d92e0e1ef
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 02/25/2022
ms.locfileid: "8355113"
---
# <a name="custom-machine-learning-models"></a>自訂機器學習模型

> [!NOTE]
> Machine Learning Studio (傳統) 將於 2024 年 8 月 31 日停止支援。 我們建議您在該日期之前轉換到 [Azure Machine Learning](/azure/machine-learning/overview-what-is-azure-machine-learning)。
>
> 從 2021 年 12 月 1 月開始，您將無法建立新的 Machine Learning Studio (傳統) 資源。 到 2024 年 8 月 31 日，您可以繼續使用現有的 Machine Learning Studio (傳統) 資源。 如需詳細資訊，請參閱[遷移至 Azure Machine Learning](/azure/machine-learning/migrate-overview)。


**智慧** > **自訂模型** 讓您根據 Azure Machine Learning 模型管理工作流程。 工作流程協助您選擇要用來產生見解的資料，並將結果對應您的統一客戶資料。 如需組建自訂 ML 模型的詳細資訊，請見 [使用 Azure Machine Learning 模型](azure-machine-learning-experiments.md)。

## <a name="responsible-ai"></a>負責的 AI

預測提供各項功能建立更佳的客戶體驗、改善業務功能和營收資料流。 我們強烈建議您比對預測會有的影響後取出餘值，並以符合道德的方式偏移可能帶入的餘值。 進一步瞭解 Microsoft 如何 [定址負責的 AI](https://www.microsoft.com/ai/responsible-ai?activetab=pivot1%3aprimaryr6)。 您也可以瞭解 Azure Machine Learning 專門負責的機器學習 [技術與流程](/azure/machine-learning/concept-responsible-ml)。

## <a name="prerequisites"></a>先決條件

- 此功能支援那些透過 [Azure Machine Learning 批次處理管道](/azure/machine-learning/concept-ml-pipelines)發行的 web 服務 。

- 您需要與您的 Azure Studio 執行個體產生關聯的 Azure Data Lake Gen2 儲存體帳戶使用此功能。 如需詳細資訊，請參閱[建立 Azure Data Lake Storage Gen2 儲存體帳戶](/azure/storage/blobs/data-lake-storage-quickstart-create-account)。

- 前往具備準銷售案源的 Azure Machine Learning 工作區，您需要具備 Azure Machine Learning 工作區負責人或使用者存取權系統管理員的權限。

   > [!NOTE]
   > 在您的 Customer Insights 執行個體與選取的 Azure web 服務或工作流程中的準銷售案源之間傳輸資料。 當您將資料轉移到 Azure 服務時，請確保將服務設為以必要的方式和位置處理資料，以符合組織中對此資料的任何法律或法規要求。

> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RWRElk]

## <a name="add-a-new-workflow"></a>新增工作流程

1. 前往 **智慧** > **自訂模型** 並選取 **新增工作流程**。

1. 在 **名稱** 欄位中，為自訂模型提供可辨識的名稱。

   > [!div class="mx-imgBorder"]
   > ![新增工作流程窗格的螢幕擷取畫面。](media/new-workflowv2.png "新增工作流程窗格的螢幕擷取畫面")

1. 在 **包含您的 Web 服務的用戶** 中，選取包含 Web 服務的組織。

1. 如果您的 Azure Machine Learning 訂閱與 Customer Insights 位於不同的用戶，請選取 **登入**，並針對所選組織使用您的認證登入。

1. 選取與您的 web 服務相關聯的 **工作區**。 

1. **在包含您的模型 Web 服務** 下拉式清單中，選擇 Azure Machine Learning 管道。 然後選取 **下一步**。    
   深入瞭解關於 [使用 Designer 程式](/azure/machine-learning/concept-ml-pipelines#building-pipelines-with-the-designer) 或 [SDK](/azure/machine-learning/concept-ml-pipelines#building-pipelines-with-the-python-sdk) 發佈 Azure Machine Learning 中的管道。 您的管道必須在 [管道端點](/azure/machine-learning/how-to-run-batch-predictions-designer#submit-a-pipeline-run) 下發佈。

1. 各 **Web 服務輸入** 方面，請從對象見解選取符合的 **實體** 並選取 **下一步**。
   > [!NOTE]
   > 自訂模型工作流程將會套用啟發型方法，根據欄位的名稱和資料類型，將 web 服務輸入欄位對應至實體屬性。 如果 web 服務欄位無法對應至實體，則會出現錯誤。

   > [!div class="mx-imgBorder"]
   > ![設定工作流程。](media/intelligence-screen2-updated.png "設定工作流程")

1. 請在 **模型輸出參數** 步驟中設定下列屬性：
      1. 輸入您想讓管道輸出結果流入的輸出 **實體名稱**。
      1. 請從下拉式選單選取您的批次處理管道的 **輸出資料存放區參數名稱**。
      1. 請從下拉式選單選取您的批次處理管道的 **輸出路徑參數名稱**。

      > [!div class="mx-imgBorder"]
      > ![模型輸出參數窗格。](media/intelligence-screen3-outputparameters.png "模型輸出參數窗格")

1. 從 **結果中的客戶識別碼** 下拉式清單選取可以找到客戶對應屬性，並選取 **儲存**。

   > [!div class="mx-imgBorder"]
   > ![客戶資料相關結果窗格。](media/intelligence-screen4-relatetocustomer.png "客戶資料相關結果窗格")

1. 您會看到 **工作流程已儲存** 畫面，其中包含工作流程的詳細資料。    
   如果您已針對 Azure Machine Learning 管道組態工作流程，對象見解將附加到包含管道的工作區。 對象見解在 Azure 工作區取得 **參與者** 角色。

1. 選取 **完成**。

1. 您現在可以從 **自訂模型** 頁面執行工作流程。

## <a name="edit-a-workflow"></a>編輯工作流程

1. 在 **自訂模型** 頁面上，選取先前建立之工作流程旁邊 **動作** 欄中的垂直省略符號，然後選取 **編輯**。

1. 您可以在 **顯示名稱** 欄位中更新您的工作流程可識別名稱，但不能變更已組態的 Web 服務或管道。 選取 **下一步**。

1. 各 **Web 服務輸入** 方面，您可以從對象見解更新符合的 **實體**。 然後選取 **下一步**。

1. 請在 **模型輸出參數** 步驟中設定下列屬性：
      1. 輸入您想讓管道輸出結果流入的輸出 **實體名稱**。
      1. 請針對您的測試管道選取 **輸出資料存放區參數名稱**。
      1. 請針對您的測試管道選取 **輸出路徑參數名稱**。

1. 從 **結果中的客戶識別碼** 下拉式清單選取可以找到客戶對應屬性，並選取 **儲存**。
   從推論輸出中選擇屬性，其值類似客戶實體的客戶識別碼資料欄。 如果您的資料集沒有此欄位，請選擇唯一識別該行的屬性。

## <a name="run-a-workflow"></a>執行工作流程

1. 在 **自訂模型** 頁面上，選取先前建立之工作流程旁邊 **動作** 欄中的垂直省略符號。

1. 選取 **執行**。

工作流程也會自動隨每個排定的重新整理一起執行。 進一步了解[設定排定的更新](system.md#schedule-tab)。

## <a name="delete-a-workflow"></a>刪除工作流程

1. 在 **自訂模型** 頁面上，選取先前建立之工作流程旁邊 **動作** 欄中的垂直省略符號。

1. 選取 **刪除**，並確認刪除。

將會刪除您的工作流程。 您建立工作流程時所建立的 [實體](entities.md)仍然存在，而且可以從 **實體** 頁面來檢視此實體。

## <a name="results"></a>結果​​

工作流程的結果會儲存在模型輸出參數階段時設定的實體中。 您可以從[實體頁面](entities.md)或使用 [API 存取](apis.md)存取此資料。

### <a name="api-access"></a>API 存取

若要讓特定 OData 查詢從自訂模型實體取得資料，請使用下列格式：

`https://api.ci.ai.dynamics.com/v1/instances/<your instance id>/data/<custom model output entity name>%3Ffilter%3DCustomerId%20eq%20'<guid value>'`

1. 以 Customer Insights 環境的識別碼取代 `<your instance id>`，在您存取 Customer Insights 時可以在瀏覽器的網址列中找到識別碼。

1. 將 `<custom model output entity>` 以實體名稱取代，即您在自訂模型設定的模型輸出參數步驟中所提供的名稱。

1. 您想要為哪位客戶存取記錄，將 `<guid value>` 以其客戶識別碼取代。 您通常可以在[客戶個人資料頁面](customer-profiles.md)的 CustomerID 欄位中找到此識別碼。

## <a name="frequently-asked-questions"></a>常見問題集

- 為何在設定自訂模型工作流程時看不到我的準銷售案源？    
  發生此問題的原因通常是由於準銷售案源的設定有問題。 確定[輸入參數已設定](azure-machine-learning-experiments.md#dataset-configuration)，而且[輸出資料存儲和路徑參數](azure-machine-learning-experiments.md#import-pipeline-data-into-customer-insights)也已設定完成。

- 錯誤「無法儲存智慧工作流程」是什麼意思？    
  通常使用者看到此錯誤訊息，是當他沒有工作區的負責人或使用者存取權系統管理員權限。 使用者需要更高等級的權限，才能以作為服務的方式啟用 Customer Insights 來處理工作流程，而非以使用者認證進行工作流程的後續執行。

[!INCLUDE[footer-include](../includes/footer-banner.md)]
