---
title: 軟體庫存遺失或不正確
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658047"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="a467c-102">軟體庫存遺失或不正確</span><span class="sxs-lookup"><span data-stu-id="a467c-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="a467c-103">威脅與弱點管理 (TVM) 中的軟體清查是貴組織中具有官方通用平台列舉 (CPE) 的已知軟體清單。</span><span class="sxs-lookup"><span data-stu-id="a467c-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="a467c-104">沒有官方 CPE 的軟體產品不會發佈弱點。</span><span class="sxs-lookup"><span data-stu-id="a467c-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="a467c-105">清查也包含詳細資料，例如廠商名稱、弱點數目、威脅，以及暴露的裝置數目。</span><span class="sxs-lookup"><span data-stu-id="a467c-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="a467c-106">裝置上的軟體變更通常會在兩小時內反映在安全性入口網站中。</span><span class="sxs-lookup"><span data-stu-id="a467c-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="a467c-107">不過，有時可能需要較長的時間。</span><span class="sxs-lookup"><span data-stu-id="a467c-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="a467c-108">目前無法強制同步處理；此為持續進行的評估。</span><span class="sxs-lookup"><span data-stu-id="a467c-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="a467c-109">如果您進行軟體變更，但 5 小時後變更未正確反映在 TVM 中，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="a467c-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="a467c-110">檢查軟體證據區段，以了解偵測軟體的方式。</span><span class="sxs-lookup"><span data-stu-id="a467c-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="a467c-111">確定軟體受到支援。</span><span class="sxs-lookup"><span data-stu-id="a467c-111">Make sure that the software is supported.</span></span> <span data-ttu-id="a467c-112">軟體只能在裝置層級顯示，即使威脅與弱點管理目前不支援該軟體也一樣。</span><span class="sxs-lookup"><span data-stu-id="a467c-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="a467c-113">不過，只可使用有限的資料。</span><span class="sxs-lookup"><span data-stu-id="a467c-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="a467c-114">如需從入口網站報告錯誤的步驟，請參閱[報告錯誤](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)。</span><span class="sxs-lookup"><span data-stu-id="a467c-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="a467c-115">**注意**：從 MDE 入口網站報告錯誤是進行工程設計的單向通道。</span><span class="sxs-lookup"><span data-stu-id="a467c-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="a467c-116">如果問題緊急，請開立支援票證。</span><span class="sxs-lookup"><span data-stu-id="a467c-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="a467c-117">如需詳細資訊，請參閱[軟體清查 - 威脅與弱點管理](/microsoft-365/security/defender-endpoint/tvm-software-inventory)。</span><span class="sxs-lookup"><span data-stu-id="a467c-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>