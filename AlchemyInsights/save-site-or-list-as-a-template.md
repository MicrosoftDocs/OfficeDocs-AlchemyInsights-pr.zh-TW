---
title: 儲存為範本的網站或清單
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 03258ec4f5476a1ea6dd3a31d17bda815bc5a18a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/24/2019
ms.locfileid: "33243173"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="9d354-102">儲存為範本的網站或清單</span><span class="sxs-lookup"><span data-stu-id="9d354-102">Save site or list as a template</span></span>

<span data-ttu-id="9d354-103">SharePoint 網站範本是預先的定義專為特定的業務需求。</span><span class="sxs-lookup"><span data-stu-id="9d354-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="9d354-104">如需詳細資訊，請參閱[使用範本來建立不同類型的 SharePoint 網站](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)。</span><span class="sxs-lookup"><span data-stu-id="9d354-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="9d354-105">以下是一些常見的問題/解決方案有關儲存網站或清單作為範本，在 SharePoint Online 中。</span><span class="sxs-lookup"><span data-stu-id="9d354-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="9d354-106">**儲存網站/清單範本] 按鈕會無法使用，或遺失**。</span><span class="sxs-lookup"><span data-stu-id="9d354-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="9d354-107">系統管理員就必須允許自訂指令碼來啟用範本的功能。</span><span class="sxs-lookup"><span data-stu-id="9d354-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="9d354-108">如需詳細的步驟、 範例及考量請參閱[允許或防止自訂指令碼](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)。</span><span class="sxs-lookup"><span data-stu-id="9d354-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="9d354-109">另存網站為範本] 命令不支援，及使用 SharePoint Server 發佈基礎結構的網站上可能會造成問題。</span><span class="sxs-lookup"><span data-stu-id="9d354-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="9d354-110">**[網站] 範本無法建立或無法正常運作**</span><span class="sxs-lookup"><span data-stu-id="9d354-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="9d354-111">範本可能會遺失的[功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)，並不會啟動。</span><span class="sxs-lookup"><span data-stu-id="9d354-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="9d354-112">如果找不到可在目前的網站集合中啟動的功能，您無法使用網站範本建立網站。</span><span class="sxs-lookup"><span data-stu-id="9d354-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="9d354-113">請查看是否任何清單或文件庫超過 5000 的項目[清單檢視的限制臨界值](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)為這可以封鎖架設的網站範本。</span><span class="sxs-lookup"><span data-stu-id="9d354-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="9d354-114">網站使用太多的資源並因此網站範本超過 50 mb 的限制。</span><span class="sxs-lookup"><span data-stu-id="9d354-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="9d354-115">有問題，顯示使用查閱欄的清單中的資料。</span><span class="sxs-lookup"><span data-stu-id="9d354-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="9d354-116">如需詳細資訊，請參閱[範本產生清單不會顯示來自 SharePoint Online 中正確的查閱清單的資料](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a)。</span><span class="sxs-lookup"><span data-stu-id="9d354-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="9d354-117">常見的問題與解決方案的詳細資訊，請參考，請[建立及使用網站範本](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。</span><span class="sxs-lookup"><span data-stu-id="9d354-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>
