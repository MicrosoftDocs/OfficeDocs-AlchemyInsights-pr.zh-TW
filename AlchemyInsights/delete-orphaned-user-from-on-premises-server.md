---
title: 從內部部署的伺服器刪除孤立使用者
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/20/2020
ms.locfileid: "45186108"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="429f7-102">從內部部署的伺服器刪除孤立使用者</span><span class="sxs-lookup"><span data-stu-id="429f7-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="429f7-103">若要移除孤立使用者，請依循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="429f7-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="429f7-104">按照[什麼是 Azure Active Directory 的混合式身分識別？](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories) (英文) 中的指示，強制執行目錄同步處理。</span><span class="sxs-lookup"><span data-stu-id="429f7-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="429f7-105">若要驗證目錄同步處理，請參閱[什麼是 Azure Active Directory 的混合式身分識別？](https://technet.microsoft.com/library/jj151797.aspx) (英文)。</span><span class="sxs-lookup"><span data-stu-id="429f7-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="429f7-106">如果同步處理功能正常，但是 Active Directory 物件刪除並未傳播到 Azure AD，請使用下列其中一種適用於 Windows PowerShell Cmdlet 的 Azure Active Directory 模組來手動移除孤立物件：</span><span class="sxs-lookup"><span data-stu-id="429f7-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="429f7-107">Remove-MsolContact</span><span class="sxs-lookup"><span data-stu-id="429f7-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="429f7-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="429f7-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="429f7-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="429f7-109">Remove-MsolUser</span></span>

    <span data-ttu-id="429f7-110">例如，若要移除原本使用目錄同步處理所建立的孤立使用者識別碼 john.smith@contoso.com，請執行 Cmdlet：</span><span class="sxs-lookup"><span data-stu-id="429f7-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="429f7-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="429f7-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>