---
title: 建立和管理環境
description: 瞭解如何註冊服務及管理環境。
ms.date: 12/06/2021
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: how-to
ms.reviewer: mhart
author: NimrodMagen
ms.author: nimagen
manager: shellyha
---

# <a name="manage-environments"></a>管理環境



## <a name="switch-environments"></a>切換環境

選取頁面右上角的 **環境** 控制項，以變更環境。

:::image type="content" source="media/home-page-environment-switcher.png" alt-text="螢幕擷取畫面，圖為切換環境的控制項。":::

系統管理員能夠[建立](create-environment.md)和管理環境。

## <a name="edit-an-existing-environment"></a>編輯現有環境

您可以編輯現有環境的部分詳細資料。

1.  在應用程式的標頭中選取 **環境** 選取器。

2.  選取 **編輯** 圖示。

3. 您可以在 **編輯環境** 方塊中更新環境設定。

如需環境設定的詳細資訊，請參閱[建立新環境](create-environment.md)。

## <a name="connect-to-microsoft-dataverse"></a>連線至 Microsoft Dataverse
   
**Microsoft Dataverse** 步驟讓您連接 Customer Insights 和您的 Dataverse 環境。

若要使用[開箱即用預測模型](predictions-overview.md#out-of-box-models)，請組態與 Dataverse 共用的資料。 或者您可以從內部部署資料來源擷取，提供貴組織管理的 Microsoft Dataverse 環境 URL。 選取 **啟用資料共用** 功能以便和 Dataverse 託管的資料湖共用 Customer Insights 輸出資料。

> [!IMPORTANT]
> Customer Insights 與 Dataverse 必須位於相同的地區，才能啟用資料共用。

:::image type="content" source="media/dataverse-data-sharing.png" alt-text="啟用與 Microsoft Dataverse 共用資料的設定選項。":::

> [!NOTE]
> Customer Insights 不支援的資料共用案例如下：
> - 如果您儲存所有資料到 Azure Data Lake Storage，您就不能啟用與 Dataverse 託管的資料湖共用資料的功能。
> - 如果您啟用與 Dataverse 共享資料的功能，您就無法[在實體建立預測或遺漏的數值](predictions.md)。

## <a name="copy-the-environment-configuration"></a>複製環境設定

當您建立新的環境時，您可以選擇從現有的環境複製設定。 

:::image type="content" source="media/environment-settings-dialog.png" alt-text="螢幕擷取畫面，圖為環境設定中的設定選項。":::

您會看到組織中所有可用環境的清單，您可以從此清單複製資料。

下列組態設定已複製，

- 內嵌/匯入的資料來源
- 資料統一 (對應、比對、合併) 設定
- 客戶細分
- 量值
- 關聯
- 活動
- 搜尋和篩選索引
- 匯出目的地
- 已排程的重新整理
- 擴充
- 模型管理
- 角色指派

*不會* 複製下列資料：

- 客戶設定檔。
- 資料來源認證。 您必須提供每個資料來源的認證，並手動重新整理資料來源。

- 取自 Common Data Model 資料夾和 Dataverse 託管資料湖的資料來源。 您必須使用與來源環境相同的名稱，手動建立這些資料來源。

複製環境時，您會看到一則指示已建立新環境的確認訊息。 選取 **移至資料來源** 以查看資料來源清單。

所有的資料來源都會顯示 **需要認證** 狀態。 編輯資料來源，並輸入認證以進行重新整理。

:::image type="content" source="media/data-sources-copied.png" alt-text="已複製且需要驗證的資料來源清單。":::

重新整理資料來源之後，移至 **資料** > **統一**。 您會在此處找到來源環境的設定。 視需要編輯，或選取 **執行** 以開始進行資料統一處理程序，並建立統一的客戶實體。

資料統一完成時，移至 **測量** 和 **分段** 進行重新整理。

## <a name="reset-an-existing-environment"></a>重設現有環境中

作為管理員，如果您要刪除所有組態並移除內嵌的資料，您可以將環境重設為空白狀態。

1.  在應用程式的標頭中選取 **環境** 選取器。 

2.  選取您要重設的環境，並選取省略號 (**...**)。 

3. 選擇 **重設** 選項。 

4.  若要確認刪除，請輸入環境名稱並選取 **重設**。

## <a name="delete-an-existing-environment"></a>刪除現有環境

作為管理員，您可以刪除您所管理的環境。

1.  在應用程式的標頭中選取 **環境** 選取器。

2.  選取您要重設的環境，並選取省略號 (**...**)。 

3. 選擇 **刪除** 選項。 

4.  若要確認刪除，請輸入環境名稱，然後選取 **刪除**。


[!INCLUDE[footer-include](../includes/footer-banner.md)]
