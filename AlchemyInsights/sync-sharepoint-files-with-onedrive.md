---
title: 將 SharePoint 檔案與新的 OneDrive 同步處理用戶端同步
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757793"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="0197b-102">將 SharePoint 檔案與新的 OneDrive 同步處理用戶端同步</span><span class="sxs-lookup"><span data-stu-id="0197b-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="0197b-103">[在檔案總管中開啟] 命令會開啟 [Windows 檔案總管] 的本機執行個體，其中顯示主控 SharePoint 網站的伺服器上的資料夾結構。</span><span class="sxs-lookup"><span data-stu-id="0197b-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="0197b-104">因此，我們建議您將 SharePoint 檔案與新的 OneDrive 同步處理用戶端同步](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>，其提供[檔案隨選]，因為它可讓您在本機存取您的檔案，並提供最佳效能。</span><span class="sxs-lookup"><span data-stu-id="0197b-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="0197b-105">如果您選擇使用總管檢視，而非使用新的同步用戶端，請務必遵循以下文章中提供的步驟及最佳做法。</span><span class="sxs-lookup"><span data-stu-id="0197b-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- <span data-ttu-id="0197b-106">[如何使用 [在檔案總管中開啟] 命令以在 SharePoint Online 中針對問題進行疑難排解](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)</span><span class="sxs-lookup"><span data-stu-id="0197b-106">[How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)</span></span>

- <span data-ttu-id="0197b-107">[使用 [在檔案總管中開啟] 的方式複製或移動文件庫](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span><span class="sxs-lookup"><span data-stu-id="0197b-107">[Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span></span>

<span data-ttu-id="0197b-108">注意事項：新版文件庫不會顯示 [在檔案總管中開啟] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="0197b-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="0197b-109">按一下右上方 (下拉式清單的位置依您的檢視畫面而定) 的 [檢視] 下拉式清單，再按一下 [檔案總管] 中的 [檢視]。</span><span class="sxs-lookup"><span data-stu-id="0197b-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="0197b-110">SharePoint [在檔案總管中開啟] 使用 ActiveX 控制項，所以只支援 Internet Explorer 10 或 11。</span><span class="sxs-lookup"><span data-stu-id="0197b-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="0197b-111">[在檔案總管中開啟] 無法用於 Windows 的 Microsoft Edge、Google Chrome、Mozilla Firefox，或 Mac 平台上。</span><span class="sxs-lookup"><span data-stu-id="0197b-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="0197b-112">因為這個原因，[檔案總管檢視] 選項可能會呈現灰色。</span><span class="sxs-lookup"><span data-stu-id="0197b-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="0197b-113">[為什麼 SharePoint 功能區按鈕無法使用或呈現灰色](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)。</span><span class="sxs-lookup"><span data-stu-id="0197b-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  
