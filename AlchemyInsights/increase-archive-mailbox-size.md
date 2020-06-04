---
title: 305增加封存信箱大小
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f80b2a10ebc17cd98ed1d29b0e6ba3ca01eb1d62
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508799"
---
# <a name="increase-the-archive-mailbox-size"></a><span data-ttu-id="e125f-102">增加封存信箱大小</span><span class="sxs-lookup"><span data-stu-id="e125f-102">Increase the archive mailbox size</span></span>

<span data-ttu-id="e125f-103">Microsoft 365 會根據指派給使用者帳戶的授權，[限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)封存信箱的大小。</span><span class="sxs-lookup"><span data-stu-id="e125f-103">Microsoft 365 [limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) the size of archive mailboxes based on the license that's assigned to the user account.</span></span> <span data-ttu-id="e125f-104">當封存信箱達到其允許大小的90% 時，使用者會收到電子郵件通知。</span><span class="sxs-lookup"><span data-stu-id="e125f-104">When the archive mailbox reaches 90% of its allowed size, the user receives an email notification.</span></span> <span data-ttu-id="e125f-105">當封存信箱達到其大小限制時，使用者就無法將更多專案移至封存信箱。</span><span class="sxs-lookup"><span data-stu-id="e125f-105">When an archive mailbox reaches its size limit, the user can't move more items to the archive mailbox.</span></span> <span data-ttu-id="e125f-106">達到大小限制時，Microsoft 365 不會增加封存信箱的大小。</span><span class="sxs-lookup"><span data-stu-id="e125f-106">Microsoft 365 won't increase the size of an archive mailbox once the size limit is reached.</span></span> <span data-ttu-id="e125f-107">相反地，使用者可以採取下列動作來釋放封存信箱中的空間：</span><span class="sxs-lookup"><span data-stu-id="e125f-107">Instead, users can take the following actions to free up space in the archive mailbox:</span></span>

- <span data-ttu-id="e125f-108">使用 Outlook 將專案匯出為 .pst 檔案。</span><span class="sxs-lookup"><span data-stu-id="e125f-108">Export the the items to a .pst file using Outlook.</span></span>

- <span data-ttu-id="e125f-109">刪除封存信箱中的專案。</span><span class="sxs-lookup"><span data-stu-id="e125f-109">Delete items from the archive mailbox.</span></span>

<span data-ttu-id="e125f-110">Microsoft 365 為 Office 365 企業版 E3 和 E5 授權提供**無限制**的封存。</span><span class="sxs-lookup"><span data-stu-id="e125f-110">Microsoft 365 provides **unlimited archiving** for Office 365 Enterprise E3 and E5 licenses.</span></span> <span data-ttu-id="e125f-111">管理員必須啟用此功能，封存信箱才能達到其大小上限。</span><span class="sxs-lookup"><span data-stu-id="e125f-111">An admin must enable this feature before the archive mailbox reaches its maximum size.</span></span> <span data-ttu-id="e125f-112">當無限期封存啟用時，最多可能需要30天才能將可用空間新增至封存信箱。</span><span class="sxs-lookup"><span data-stu-id="e125f-112">When unlimited archiving is enabled, it can take up to 30 days before free space is added to the archive mailbox.</span></span> <span data-ttu-id="e125f-113">因此，建議系統管理員驗證封存信箱中的可用空間，讓使用者可以在展開時繼續使用封存信箱。</span><span class="sxs-lookup"><span data-stu-id="e125f-113">Therefore, we recommend that admins verify the free space in the archive mailbox, which allows the user to continue using the archive mailbox while it expands.</span></span> <span data-ttu-id="e125f-114">如需詳細資訊，請參閱[microsoft 365 中的無限](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving)封存，並[在 Microsoft 365 中啟用無限](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving)封存。</span><span class="sxs-lookup"><span data-stu-id="e125f-114">For more information, see [Overview of unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) and [Enable unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).</span></span>

<span data-ttu-id="e125f-115">如需從 Outlook 存取封存信箱的詳細資訊，請參閱[在自動展開的封存中存取專案的 Outlook 需求](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)。</span><span class="sxs-lookup"><span data-stu-id="e125f-115">For more information on accessing the archive mailbox from Outlook, see [Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span></span> <span data-ttu-id="e125f-116">若要設定自動將專案移至封存信箱的保留原則，請參閱[設定 Microsoft 365 組織中信箱的封存和刪除原則](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="e125f-116">To configure a retention policy that automatically moves items to the archive mailbox, see [Set up an archive and deletion policy for mailboxes in your Microsoft 365 organization](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span></span>

<span data-ttu-id="e125f-117">**附注**： Exchange 2010 上的主要信箱不支援自動展開的封存。</span><span class="sxs-lookup"><span data-stu-id="e125f-117">**Note**: Auto-expanding archives aren't supported for primary mailboxes on Exchange 2010.</span></span>