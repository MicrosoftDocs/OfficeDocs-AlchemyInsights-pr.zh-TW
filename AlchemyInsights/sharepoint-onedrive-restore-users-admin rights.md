---
title: 疑難排解 OneDrive 商務網站的拒絕存取郵件
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670607"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>疑難排解 OneDrive 商務網站的拒絕存取郵件

當使用者使用相同使用者主體名稱 (UPN) 進行刪除及重新建立時，最常發生此問題。 新帳戶是使用不同的 PUID (Passport 唯一識別碼) 值建立。 當使用者嘗試存取網站集合或其 OneDrive 時，使用者的 PUID 不正確。 第二個案例是以 Active Directory 組織單位 (OU) 進行目錄同步處理。 如果使用者已經登入 SharePoint，然後將其移至不同的 OU，並使用 SharePoint 進行 resynced，可能會發生此問題。

1. 若要解決此問題，您應該使用本文中的步驟還原原始的 UPN，在 [Microsoft 365 中還原使用者](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)。
2. 如果您無法還原原始使用者，您應該使用這些步驟從 OneDrive 網站移除舊的使用者，並 [從 [使用者資訊] 清單中移除使用者]()。 
3. 完成之後，您可以依照下列步驟，確認使用者對 OneDrive 網站具有系統管理員許可權： [針對使用者的 OneDrive 新增系統管理員許可權。](https://docs.microsoft.com/sharepoint/manage-user-profiles)

如需許可權等級的詳細資訊，請參閱 [瞭解 SharePoint 中的許可權等級](https://docs.microsoft.com/sharepoint/understanding-permission-levels)一文。
