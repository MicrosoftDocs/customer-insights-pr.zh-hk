---
title: 管理客戶細分的預設同意規則
description: 有了同意管理功能，您可以停用或變更預設同意規則 (如果已啟用覆寫)。
ms.date: 12/01/2021
ms.service: customer-insights
mms.topic: how-to
author: smithy7
ms.author: smithc
ms.reviewer: mhart
manager: shellyha
ms.openlocfilehash: 28c9ea49b1f3aebd3abd7d4de58fe61e6474158b
ms.sourcegitcommit: 48d799535fad84e8b63c80aef48b5c5e87628f58
ms.translationtype: HT
ms.contentlocale: zh-HK
ms.lasthandoff: 12/03/2021
ms.locfileid: "7884197"
---
# <a name="disable-or-change-default-consent-rules"></a>停用或變更預設同意規則

如果您的組織使用[同意管理功能](../consent-management/overview.md)搭配對象見解，[系統管理員便可以對客戶細分強制實施同意規則](activate-consent.md)。 

在客戶細分區域中有強制性的同意規則，則每一個客戶細分都會通知您同意檢查和規則的狀態。 如果允許覆寫，將關閉特定客戶細分的預設同意規則。 除了預設規則外，客戶細分的每個建立者都可以在該客戶細分中新增更多同意規則。 

## <a name="for-administrators"></a>適用於系統管理員

:::image type="content" source="../consent-management/media/consent-rules-segment.png" alt-text="含同意規則選項的客戶細分建立器。":::

**停用預設同意規則：**

1. 在 **同意規則** 通知中，選取 **查看詳細資料**。 

1. 把 **預設同意規則** 切換設定為 **關閉**。

**新增更多同意規則：**

1. 在 **同意規則** 通知中，選取 **查看詳細資料**。 

1. 選取 **新增同意規則** ，然後從 **選取同意資料類型** 下拉式功能表中選擇一種同意規則 。

1. 選取 **儲存**，將新規則套用至該客戶細分。

## <a name="for-contributors"></a>對於參與者

若要建立客戶細分而不使用強制許可規則，您必須請您的系統管理員在客戶細分上將它們停用。 不過，您可以新增您的同意規則到您擁有和管理的客戶細分。

這是三個步驟程序： 
1. 在對象見解中[建立客戶細分](segments.md)並儲存。 

1. 與您的系統管理員共用客戶細分名稱，並要求他們[對客戶細分啟用覆寫](activate-consent.md)。 

1. 再次打開您的客戶細分。 在 **同意規則** 通知中，選取 **查看詳細資料**，並新增您想套用的同意規則。 接著，**儲存** 並 **執行** 您的客戶細分。



[!INCLUDE[footer-include](../includes/footer-banner.md)] 
