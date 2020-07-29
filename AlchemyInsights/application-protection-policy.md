---
title: 應用程式保護原則
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/22/2020
ms.locfileid: "45266414"
---
# <a name="application-protection-policy"></a>應用程式保護原則

如果您不熟悉應用程式防護原則 (APP)，請參閱[應用程式保護原則概觀](https://docs.microsoft.com/intune/apps/app-protection-policy)。

若要開始使用 APP，請參閱[如何建立及指派應用程式保護原則](https://docs.microsoft.com/intune/app-protection-policies)。

應用程式保護原則需求：

- 使用者擁有 Intune 或 EMS 授權。
- 使用者屬於應用程式保護原則鎖定的群組。
- 裝置上只有一個公司使用者登入受保護的應用程式。
- 應用程式已實作 [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started)。 如需支援 SDK 的應用程式清單，請參閱 [Microsoft Intune 保護的應用程式](https://docs.microsoft.com/intune/apps-supported-intune-apps)。

當符合上述需求的使用者登入已啟用 Intune SDK 的應用程式後，會套用原則。 若要判斷是否已套用原則，最簡單的方法是要求使用者在原則中設定 PIN。 

如需詳細資訊，請參閱：

[APP/MAM 疑難排解常見問題集](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[如何驗證您的應用程式保護原則設定](https://docs.microsoft.com/intune/app-protection-policies-validate)

[了解應用程式保護原則傳遞時間表](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[如何監視應用程式保護原則](https://docs.microsoft.com/intune/app-protection-policies-monitor)