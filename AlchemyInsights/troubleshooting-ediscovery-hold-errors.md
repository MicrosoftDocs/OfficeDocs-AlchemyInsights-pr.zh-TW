---
title: 疑難排解電子文件探索保留錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/20/2021
ms.locfileid: "52583750"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>疑難排解電子文件探索保留錯誤

發生電子文件探索保留問題嗎？ 以下是可考慮的一些最佳做法：

- 檢查保留發佈狀態。  若狀態為 **開啟 (擱置中)** 或 **關閉 (擱置中)**，請等候保留發布完成。
- 將電子文件探索保留更新合併入單一大量要求，而非重複地為每次交易更新此原則。
- 在安全性和合規性中心 PowerShell 中執行 Set-CaseHoldPolicy <policyname> -RetryDistribution。 如需詳細資料，請參閱 [連線到安全性和合規性中心 PowerShel](/powershell/exchange/connect-to-scc-powershell)。

如需緩解及解決電子文件探索保留問題的檢查設定和其它最佳做法的步驟，請參閱 [疑難排解電子文件探索保留錯誤](/microsoft-365/compliance/hold-distribution-errors)。
如需有關疑難排解其它常見電子文件探索問題的資訊，請參閱 [調查、疑難排解和解決常見電子文件探索問題](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)。
