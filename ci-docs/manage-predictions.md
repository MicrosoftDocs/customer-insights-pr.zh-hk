---
title: 管理預測
description: 了解如何管理、疑難排解及修正預測。
ms.date: 11/01/2021
ms.reviewer: mhart
ms.subservice: audience-insights
ms.topic: how-to
author: m-hartmann
ms.author: mhart
manager: shellyha
ms.openlocfilehash: 42abfb305efaccaeef48e32f2cc69f3d36fbe73d
ms.sourcegitcommit: 49394c7216db1ec7b754db6014b651177e82ae5b
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 08/10/2022
ms.locfileid: "9245492"
---
# <a name="manage-predictions"></a>管理預測

本文討論大部分預測案例中都有的一些工作。

## <a name="troubleshoot-a-failed-prediction"></a>疑難排解失敗的預測

1. 請前往 **智慧** > **預測** 並選取 **我的預測** 索引標籤。

1. 選取您要檢視錯誤記錄的預測旁的垂直刪節號。

1. 選取 **記錄**。

1. 檢閱所有錯誤。 可能發生的錯誤有數種類型，這些類型描述造成錯誤的狀況。 例如，沒有足夠資料而無法準確預測的錯誤，通常是透過載入額外資料到 Customer Insights 中來解決。

## <a name="input-data-usability-report"></a>輸入資料可用性報表

輸入資料可用性報表提供錯誤和警告的整合檢視表，指出在您的立即可用的預測可能產生的錯誤和警告。 它也提供如何改善模型效能的建議。

在模型完成其定型程序之後，才可使用此報表。 它是單獨為每個模型建立的，不管其是否成功完成。

### <a name="view-the-input-data-usability-report"></a>查看輸入資料可用性報表

當立即可用的模型完成後，請查看報表：
- 選取模型名稱旁邊的省略號，然後選擇 **輸入資料可用性報表**。
- 選取模型的狀態，然後在側面窗格中選取 **查看輸入資料可用性報表**。
- 在清單中選取其中一個模型，然後在命令列中選取 **輸入資料可用性報表**。
- 打開模型結果頁面，然後在命令列中選取 **輸入資料可用性報表**。

### <a name="information-in-the-input-data-usability-report"></a>在輸入資料可用性報表的資訊

報表中的下列各資料行包含改善模型資料的實用資訊。

:::image type="content" source="media/input-data-usability-report.png" alt-text="輸入資料可用性報表範例，顯示內有錯誤、警告和建議的資料表。":::

- **名稱：** 錯誤、警告或建議的描述性名稱。
- **步驟：** 模型階段，定型或分數，參照資訊。
- **狀態：** 資訊的嚴重性 (錯誤、警告、建議)。
- **資料行名稱：** 需要修改來改善模型效能的實體內資料行。
- **實體名稱：** 需要修改來改善模型效能的實體名稱。
- **詳細資料：** 錯誤、警告或建議的詳細資料。

## <a name="refresh-a-prediction"></a>重新整理預測

測試會依照設定中所設定的同樣[資料重新整理排程](schedule-refresh.md)自動重新整理。 您也可以手動重新整理它們。

1. 請前往 **智慧** > **預測** 並選取 **我的預測** 索引標籤。

1. 選取您要重新整理之預測旁邊的垂直省略符號。

1. 選取 **重新整理**。

[!INCLUDE [progress-details-include](includes/progress-details-pane.md)]

## <a name="delete-a-prediction"></a>刪除預測

刪除預測也會同時移除其輸出實體。

1. 請前往 **智慧** > **預測** 並選取 **我的預測** 索引標籤。

1. 選取您要刪除之預測旁邊的垂直省略符號。

1. 選取 **刪除**。
