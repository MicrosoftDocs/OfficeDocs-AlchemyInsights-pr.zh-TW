---
title: 識別在稽核記錄中的信箱上的外部電子郵件轉寄
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 7fb2c161c558a7eb961f86ca2b86e33750d902fd
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32417203"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="decfe-102">找出何時會在信箱上設定外部電子郵件轉寄</span><span class="sxs-lookup"><span data-stu-id="decfe-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="decfe-103">當使用者在信箱上設定外部電子郵件轉寄時，活動被稽核**Set-mailbox**指令程式的一部分。</span><span class="sxs-lookup"><span data-stu-id="decfe-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="decfe-104">您可以查看使用中的安全性 & 合規性中心的稽核記錄搜尋的活動。</span><span class="sxs-lookup"><span data-stu-id="decfe-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="decfe-105">登入[Office 365 安全性 & 合規性中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="decfe-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="decfe-106">按一下 [**搜尋和調查**，然後選取 [**稽核記錄搜尋**。</span><span class="sxs-lookup"><span data-stu-id="decfe-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="decfe-107">在 [**開始日期**和**結束日期**] 欄位中選取日期範圍。</span><span class="sxs-lookup"><span data-stu-id="decfe-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="decfe-108">您不需要指定使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="decfe-108">You don't need to specify a username.</span></span> <span data-ttu-id="decfe-109">確認 [**活動**] 欄位設為**顯示結果的所有活動**。</span><span class="sxs-lookup"><span data-stu-id="decfe-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="decfe-110">Click **Search**.</span><span class="sxs-lookup"><span data-stu-id="decfe-110">Click **Search**.</span></span>

<span data-ttu-id="decfe-111">在結果中，按一下**篩選結果**，在 [活動篩選] 方塊中輸入**Set-mailbox** 。</span><span class="sxs-lookup"><span data-stu-id="decfe-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="decfe-112">在結果中，選取 [稽核記錄。</span><span class="sxs-lookup"><span data-stu-id="decfe-112">Select an audit record in the results.</span></span> <span data-ttu-id="decfe-113">在**詳細資料**彈出式視窗中，按一下 [**更多的資訊**。</span><span class="sxs-lookup"><span data-stu-id="decfe-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="decfe-114">您必須將看的每個稽核記錄，以判斷活動是否與電子郵件轉寄功能的相關詳細資料。</span><span class="sxs-lookup"><span data-stu-id="decfe-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="decfe-115">**ObjectId**： 上次修改信箱的別名值。</span><span class="sxs-lookup"><span data-stu-id="decfe-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="decfe-116">**參數**： _ForwardingSmtpAddress_指出目標電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="decfe-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="decfe-117">**UserId**: **ObjectId**欄位中信箱設定電子郵件轉寄功能的使用者。</span><span class="sxs-lookup"><span data-stu-id="decfe-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="decfe-118">如需詳細資訊，請參閱 <<c0>的判斷設定電子郵件轉寄的信箱。</span><span class="sxs-lookup"><span data-stu-id="decfe-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>