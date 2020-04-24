---
title: 2491警示來自「由於租使用者或使用者覆寫」原則，來自網路釣魚傳遞的電子郵件訊息
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758899"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="f3e41-102">警示來自「由於租使用者或使用者覆寫」原則，來自網路釣魚傳遞的電子郵件訊息</span><span class="sxs-lookup"><span data-stu-id="f3e41-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="f3e41-103">名為 "由於租使用者或使用者覆寫，已將「網路釣魚已傳送」的預設警示原則，已向租使用者提供 Office 365 ATP P1 和 P2 授權。</span><span class="sxs-lookup"><span data-stu-id="f3e41-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="f3e41-104">如果您收到此警示，請參閱下列步驟：</span><span class="sxs-lookup"><span data-stu-id="f3e41-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="f3e41-105">從警示訊息中，按一下 [**查看警示**]，以移至安全性 & 規範中心中的 [**警示**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="f3e41-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="f3e41-106">選取 [警示]，以查看在**瀏覽器中\*\*\*\*查看訊息清單**或查看訊息的選項。</span><span class="sxs-lookup"><span data-stu-id="f3e41-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="f3e41-107">這兩個選項都會帶您前往郵件的詳細資料，其中包含郵件識別碼。</span><span class="sxs-lookup"><span data-stu-id="f3e41-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="f3e41-108">請注意，威脅瀏覽器連結將會自動篩選符合警示準則的郵件。</span><span class="sxs-lookup"><span data-stu-id="f3e41-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="f3e41-109">您可能需要在威脅瀏覽器中調整日期篩選器。</span><span class="sxs-lookup"><span data-stu-id="f3e41-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="f3e41-110">由於手動設定的覆寫，所以已傳遞網路釣魚郵件：</span><span class="sxs-lookup"><span data-stu-id="f3e41-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="f3e41-111">由使用者設定的允許寄件者或網域。</span><span class="sxs-lookup"><span data-stu-id="f3e41-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="f3e41-112">反垃圾郵件原則中由系統管理員設定的允許寄件者或網域。</span><span class="sxs-lookup"><span data-stu-id="f3e41-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="f3e41-113">連線篩選原則中的允許 IP 位址。</span><span class="sxs-lookup"><span data-stu-id="f3e41-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="f3e41-114">設定為允許郵件的郵件流程規則（也稱為傳輸規則）。</span><span class="sxs-lookup"><span data-stu-id="f3e41-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="f3e41-115">如果您認為郵件已錯誤標示為網路釣魚，請使用 Outlook[報告訊息增益集](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)將郵件範例提交給 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="f3e41-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>