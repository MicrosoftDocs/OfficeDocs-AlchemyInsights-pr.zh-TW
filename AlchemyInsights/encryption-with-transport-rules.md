---
title: 使用傳輸規則加密
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813859"
---
# <a name="encryption-with-transport-rules"></a>使用傳輸規則加密

在 [Exchange 系統管理中心](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) 中，您可以在郵件流程規則中使用 Office 郵件加密 (OME) 功能來觸發郵件加密。 在 [傳出規則] 條件上選擇 [套用 Office 365 郵件加密與權限保護] 選項。

- 如需詳細資訊，請參閱[定義郵件流程以進行加密](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。

- 在 Powershell 中，使用 [TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) Cmdlet，並將 *ApplyOME* 參數設為 $true。
