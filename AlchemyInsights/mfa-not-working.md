---
title: MFA 的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250156"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="b404a-102">MFA 的問題</span><span class="sxs-lookup"><span data-stu-id="b404a-102">Issues with MFA</span></span>
<span data-ttu-id="b404a-103">有幾個事項檢查是否使用者無法登入使用多重要素驗證 (MFA)</span><span class="sxs-lookup"><span data-stu-id="b404a-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="b404a-104">受影響的使用者可能被封鎖在 Azure Active Directory 入口網站。</span><span class="sxs-lookup"><span data-stu-id="b404a-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="b404a-105">如果是這種情況，驗證嘗試的特定使用者會自動拒絕。</span><span class="sxs-lookup"><span data-stu-id="b404a-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="b404a-106">請遵循本篇文章以解除封鎖這些檔案中的步驟。</span><span class="sxs-lookup"><span data-stu-id="b404a-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="b404a-107">如果解除封鎖使用者沒有幫助或使用者不會遭到封鎖您可以嘗試使用重設使用者的 MFA，他們會再次經過註冊程序。</span><span class="sxs-lookup"><span data-stu-id="b404a-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="b404a-108">請遵循本文中的步驟。</span><span class="sxs-lookup"><span data-stu-id="b404a-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="b404a-109">如果這是您已啟用的 MFA 和您的使用者都無法登入非瀏覽器用戶端，例如 Outlook、 Skype 等至第一次，或許 ADAL (Active Directory Authentication Library) 上未啟用您的 O365 訂閱。</span><span class="sxs-lookup"><span data-stu-id="b404a-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="b404a-110">在此情況下必須連線至 Exchange Online Powershell 並執行此 cmdlet:  *Set-organizationconfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="b404a-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>