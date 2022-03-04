---
title: 了解並管理量值
description: 了解量值是如何協助分析並反映業務表現。
ms.date: 02/28/2022
ms.subservice: audience-insights
ms.topic: conceptual
author: m-hartmann
ms.author: wameng
ms.reviewer: mhart
manager: shellyha
searchScope:
- ci-measures
- ci-measure-builder
- ci-measure-template
- ci-enrichment-details
- customerInsights
ms.openlocfilehash: c46fcc3baba1d6c92c2c0fe459a62277343cc0e4
ms.sourcegitcommit: cf6a0ed44915908a44c70889a2dd199a9d0d4798
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 02/28/2022
ms.locfileid: "8359822"
---
# <a name="measures-overview"></a>量值概觀

量值可協助您更清晰地了解客戶行為和業務績效。 它們會從[整合個人資料](data-unification.md)中檢查相關的值。 例如，公司想要查看 *每位客戶的總花費*，以瞭解單一客戶的購買歷史，或量值 *公司的總銷售人*，以瞭解整體業務中的總營收。  

量值可以使用[量值建立器](measure-builder.md) 建立，量值建立器是一種包含各種運算子和簡單對應選項的資料查詢平臺。 它可讓您篩選資料、分組結果、偵測 [實體關聯路徑](relationships.md)，以及預覽輸出。 [使用預先定義的範本](measure-templates.md)可以有效率的設定常用量值。

規劃商務活動時，您可以使用量值建立工具查詢客戶資料並抽取見解。 例如，建立 *每個客戶的總消費額* 以及 *每個客戶的總利潤額*，能協助找出大量消費額度高且利潤高的客戶。 您可以根據這些量值[建立客戶細分](segments.md)，採取之後的最佳動作。 

## <a name="manage-your-measures"></a>管理您的量值

您可以在 **量值** 頁面上找到量值清單。

您可以找到有關量值類型、建立者、建立日期、狀態及狀況的資訊。 當您從清單中選取量值時，您可以預覽輸出並下載 CSV 檔。

若要同時重新整理所有的量值，請選取 **全部重新整理**，而不選取特定的量值。

:::image type="content" source="media/measure-actions.png" alt-text="管理單一量值的動作。":::

為下列選項，從清單中選取量值。

- 選取量值名稱以查看其詳細資料。
- **編輯** 量值的設定。
- **重新整理** 根據最新資料的量值。
- **重新命名** 量值。
- **刪除** 量值。
- **啟用** 或 **停用**。 停用量值時，不會在[排程的重新整理](system.md#schedule-tab)時進行重新整理。

[!INCLUDE [progress-details-include](../includes/progress-details-pane.md)]

## <a name="next-step"></a>下一個步驟

您可以使用現有的量值來建立[客戶細分](segments.md)。

[!INCLUDE[footer-include](../includes/footer-banner.md)]
