---
title: 使用 Intune 的條件式存取
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 20ef8205431aad821419f2559be3402c8228d838
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704777"
---
# <a name="conditional-access-with-intune"></a>使用 Intune 的條件式存取

使用具有 Intune 的  **條件式存取**  需要三個步驟：

- 建立  **相容性原則**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android)、  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios)、  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) ，以定義在將裝置視為合規性之前必須滿足的設定。 例如，裝置的 pin 碼至少必須是6位數，才會被視為相容。
- 建立 **條件式存取原則**  ，以定義要保護的資源，以及存取這些資源所需符合的條件。  [例如，](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  裝置必須先相容才能存取公司的電子郵件。
- 確定 **相容性原則**  和  **條件式存取原則**  都是以所需的使用者群組為目標。 這可能需要在 Azure Active Directory 中建立特定的使用者群組。

**有用的連結：**

[裝置合規性概述](https://docs.microsoft.com/intune/device-compliance-get-started)

[疑難排解 CA](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[疑難排解原則](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

若要保護電子郵件 (Exchange online) 不受相容裝置存取，必須遵循這兩個檔：

1. [使用 EAS 保護來自裝置的電子郵件存取](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [使用新式驗證用戶端（例如 Outlook）保護從裝置進行的電子郵件存取](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)