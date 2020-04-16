---
title: 為使用者信箱設定自動回覆
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506423"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>為使用者信箱設定自動回覆

**方法 1**

1. 登入 Office 365 入口網站。

2. 移至 [使用者] > [作用中使用者]**** (如果您在共用信箱上進行設定，則移至或 [群組] > [共用信箱]****)。

3. 選取擁有 Microsoft Exchange 信箱的使用者。

4. 在右側的飛出功能表中，移至 [郵件設定] > [自動回覆]**** (如果這是共用信箱，只要按一下飛出功能表上的 [自動回覆]**** 即可)。

**方法 2**

1. 使用系統管理員認證登入 Office 365 系統管理入口網站。

2. 展開 [系統管理中心]****，然後按一下 [Exchange]****。

3. 按一下右上角的圖片、按一下 [其他使用者]****，然後選取您要變更的使用者信箱。

4. 在左側選取 [選項]****、按一下 [組織電子郵件]****，再按一下 [自動回覆]****。

**方法 3**

在 Exchange Online PowerShell 中執行下列 Cmdlet：

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

如需有關此 Cmdlet 的詳細資訊，請參閱 [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) (英文)。