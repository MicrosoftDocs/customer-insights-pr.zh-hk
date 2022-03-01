---
title: 實體和實體路徑之間的關係
description: 從多個資料來源建立和管理實體之間的關係。
ms.date: 06/01/2020
ms.reviewer: mhart
ms.service: customer-insights
ms.subservice: audience-insights
ms.topic: conceptual
author: MichelleDevaney
ms.author: midevane
manager: shellyha
ms.openlocfilehash: d5b9566ec88096fec31d8e164a51598159ec26d4
ms.sourcegitcommit: ece48f80a7b470fb33cd36e3096b4f1e9190433a
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 06/03/2021
ms.locfileid: "6171191"
---
# <a name="relationships-between-entities"></a>實體間的關聯

當實體共用一般識別碼 (外部索引鍵) 時，關聯會連接實體並定義資料圖形。 此外部索引鍵可以從一個實體參照到另一個實體。 連接的實體依據多個資料來源來啟用客戶細分和量值定義。

有三種類型的關聯： 
- 不可編輯的系統關聯，是在資料整合程序中由系統建立的
- 不可編緝的繼承關聯，是內嵌資料來源時自動建立的 
- 可編輯的自訂關聯，由使用者建立和設定

## <a name="non-editable-system-relationships"></a>不可編輯的系統關聯

在資料整合時，會根據智慧比對自動建立系統關聯。 這些關聯有助於將客戶個人資料記錄關聯至其他對應記錄。 以下圖表將圖示三種系統型關聯的建立。 客戶實體與其他實體比對，以產生整合的的 *客戶* 實體。

:::image type="content" source="media/relationships-entities-merge.png" alt-text="具有三個 1-n 關聯的客戶實體關聯路徑圖表。":::

- ***CustomerToContact* 關聯** 是在 *客戶* 實體與 *連絡人* 實體之間建立的。 *客戶* 實體會取得 **Contact_contactID** 索引鍵欄位，來關聯 *連絡人* 實體索引鍵欄位 **contactID** 。
- ***CustomerToAccount* 關聯** 是在 *客戶* 實體與 *帳戶* 實體之間建立的。 *客戶* 實體會取得 **Account_accountID** 索引鍵欄位，來關聯 *帳戶* 實體索引鍵欄位 **accountID**。
- ***CustomerToWebAccount* 關聯** 是在 *客戶* 實體與 *WebAccount* 實體之間建立的。 *客戶* 實體會取得 **WebAccount_webaccountID** 索引鍵欄位，並關連到 *WebAccount* 實體索引鍵欄位 **webaccountID**。

## <a name="non-editable-inherited-relationships"></a>不可編輯的繼承關聯

資料擷取程序進行時，系統會檢查資料來源的現有關聯。 如果不存在任何關聯，系統會自動建立這些關聯。 這些關聯也用在下游程序中。

## <a name="create-a-custom-relationship"></a>建立自訂關聯

關聯是由包含外部索引鍵的 *來源實體* 和來源實體的外部索引鍵指向的 *目標實體* 組成。 

1. 請在對象見解中前往 **資料** > **關係**。

2. 選取 **新增關聯**。

3. 在 **新增關聯** 窗格上，提供下列資訊：

   :::image type="content" source="media/relationship-add.png" alt-text="具有空白輸入欄位的新關聯側邊窗格。":::

   - **關聯名稱**：反映關聯用途的名稱。 範例：CustomerToSupportCase。
   - **描述**：關聯的描述。
   - **來源實體**：在關聯中作為來源的實體。 範例：SupportCase。
   - **目標實體**：在關聯中作為目標的實體。 範例：客戶。
   - **來源基數**：指定來源實體的基數。 基數說明集合中可能的元素數目。 它總是與目標基數有關。 您可以選擇 **一** 和 **多個**。 只支援多對一或一對一關聯。  
     - 多對一：多個來源記錄可以關連到一個目標記錄。 範例：來自單一客戶的多個支援案例。
     - 一對一：單一來源記錄關連到一個目標記錄。 範例：一位客戶的一個忠誠度識別碼。

     > [!NOTE]
     > 多對多關聯可以使用兩個多對一關聯和一個連結實體 (連入來源實體和目標實體) 來建立。

   - **目標基數**：選取目標實體記錄的基數。 
   - **來源索引鍵欄位**：來源實體中的外部索引鍵欄位。 範例：SupportCase 可以使用 CaseID 作為外部索引鍵欄位。
   - **目標索引鍵欄位**：欄位表示目標實體的索引鍵欄位。 範例客戶可以使用 **CustomerID** 索引鍵鍵欄位。

4. 選取 **儲存** 以建立自訂關聯。

## <a name="view-relationships"></a>檢視關聯性

關聯頁面會列出已建立的所有關聯。 每一列代表一個關聯，裡面也包含有關來源實體、目標實體和基數的詳細資料。 

:::image type="content" source="media/relationships-list.png" alt-text="在關聯頁面的動作欄中的關聯和選項清單。":::

此頁面對現有與新關聯提供一組選項： 
- **新增關聯**：[建立自訂關聯](#create-a-custom-relationship)。
- **視覺化檢視**：[探索關聯視覺化檢視](#explore-the-relationship-visualizer)，以查看現有關聯及其基數的網狀圖表。
- **依...篩選**：選擇要在清單中顯示的關聯類型。
- **搜尋關聯**：在關聯的屬性上使用文字型搜尋。

### <a name="explore-the-relationship-visualizer"></a>探索關聯視覺化檢視

視覺化檢視顯示網狀圖表，表示在連接實體間的現有關聯及其基數。

若要自訂檢視表，您可以透過在畫布上拖動方塊來變更位置。

:::image type="content" source="media/relationship-visualizer.png" alt-text="關聯視覺化檢視的螢幕擷取畫面，圖上為相關實體間連接的網狀圖表。":::

可用的選項： 
- **匯出成影像**：將目前的檢視表儲存為影像檔。
- **變更為橫向/垂直版面配置**：變更實體與關聯的對齊方式。
- **編輯**：在編輯窗格中更新自訂關聯的屬性，並儲存變更。

## <a name="manage-existing-relationships"></a>管理現有關聯 

在關聯頁面上，每個關聯都是以資料列顯示。 

選取關聯，然後選擇下列其中一個選項： 
 
- **編輯**：在編輯窗格中更新自訂關聯的屬性，並儲存變更。
- **刪除**：刪除自訂關聯。
- **查看**：查看系統-建立和繼承的關聯。 

## <a name="next-step"></a>下一個步驟

因為多個資料來源不再孤立，系統和自訂關聯可以用來[建立客戶細分](segments.md)。

[!INCLUDE[footer-include](../includes/footer-banner.md)]
