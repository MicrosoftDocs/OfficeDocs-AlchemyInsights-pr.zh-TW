---
title: SSO 設定問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7760"
- "9004346"
ms.openlocfilehash: 5ab56ec1eda10ea059e600e8933ce85bb143b76e
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886803"
---
# <a name="sso-configuration-issues"></a><span data-ttu-id="88cd6-102">SSO 設定問題</span><span class="sxs-lookup"><span data-stu-id="88cd6-102">SSO configuration issues</span></span>

1. <span data-ttu-id="88cd6-103">遵循[快速入門：針對應用程式設定屬性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)指南中的屬性來設定您的應用程式。</span><span class="sxs-lookup"><span data-stu-id="88cd6-103">Follow the [Quickstart: Configure properties for an application](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guide to configure your application.</span></span>
2. <span data-ttu-id="88cd6-104">視您選擇的應用程式和[單一登入選項](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options)而定，請遵循以下的適當指導方針：a.</span><span class="sxs-lookup"><span data-stu-id="88cd6-104">Depending on the application and [Single sign-on option](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) that you chose, follow the appropriate guidance below: a.</span></span> <span data-ttu-id="88cd6-105">若要設定 **內部部署應用程式** 使用 **SAML 型單一登入 (SSO)**，請參閱[對使用應用程式 Proxy 的內部部署應用程式進行 SAML 單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)。</span><span class="sxs-lookup"><span data-stu-id="88cd6-105">To configure an **on-premises application** for **SAML-based single sign-on (SSO)**, see [SAML single-sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).</span></span>
    <span data-ttu-id="88cd6-106">b.</span><span class="sxs-lookup"><span data-stu-id="88cd6-106">b.</span></span> <span data-ttu-id="88cd6-107">若要為 **密碼型 SSO** 設定 **雲端應用程式**，請參閱[設定密碼單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)。</span><span class="sxs-lookup"><span data-stu-id="88cd6-107">To configure a **cloud application** for **password-based SSO**, see [Configure password single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).</span></span>
    <span data-ttu-id="88cd6-108">c.</span><span class="sxs-lookup"><span data-stu-id="88cd6-108">c.</span></span> <span data-ttu-id="88cd6-109">若要設定 **內部部署應用程式** 使用 **透過應用程式 Proxy 的 SSO**，請參閱[用於使用應用程式 Proxy 單一登入的密碼保存庫](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。</span><span class="sxs-lookup"><span data-stu-id="88cd6-109">To configure an **on-premises application** for **SSO through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
3. <span data-ttu-id="88cd6-110">**疑難排解應用程式 Proxy 問題**：建議您從檢查疑難排解流程[偵錯應用程式 Proxy 連接器問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)開始，以判斷是否正確已設定應用程式 Proxy 連接器。</span><span class="sxs-lookup"><span data-stu-id="88cd6-110">**Troubleshooting Application Proxy issues**: We recommend that you start with reviewing the troubleshooting flow - [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) - to determine if application proxy connectors are configured correctly.</span></span> <span data-ttu-id="88cd6-111">如果您仍然無法連線到應用程式，請遵循[偵錯應用程式 Proxy 應用程式問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)中的疑難排解步驟進行。</span><span class="sxs-lookup"><span data-stu-id="88cd6-111">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="88cd6-112">您可以執行下列瀏覽器偵錯步驟來[識別 CORS 問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues)：a.</span><span class="sxs-lookup"><span data-stu-id="88cd6-112">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by performing the following browser debug steps: a.</span></span> <span data-ttu-id="88cd6-113">啟動瀏覽器並瀏覽至 Web 應用程式。</span><span class="sxs-lookup"><span data-stu-id="88cd6-113">Launch the browser and browse to the web app.</span></span>
    <span data-ttu-id="88cd6-114">b.</span><span class="sxs-lookup"><span data-stu-id="88cd6-114">b.</span></span> <span data-ttu-id="88cd6-115">按 **F12** 以顯示偵錯主控台。</span><span class="sxs-lookup"><span data-stu-id="88cd6-115">Press **F12** to bring up the debug console.</span></span>
    <span data-ttu-id="88cd6-116">c.</span><span class="sxs-lookup"><span data-stu-id="88cd6-116">c.</span></span> <span data-ttu-id="88cd6-117">嘗試重現該交易，並檢閱主控台訊息。</span><span class="sxs-lookup"><span data-stu-id="88cd6-117">Try to reproduce the transaction and review the console message.</span></span> <span data-ttu-id="88cd6-118">CORS 違規產生關於來源的主控台錯誤。</span><span class="sxs-lookup"><span data-stu-id="88cd6-118">A CORS violation produces a console error about origin.</span></span>
    <span data-ttu-id="88cd6-119">d.</span><span class="sxs-lookup"><span data-stu-id="88cd6-119">d.</span></span> <span data-ttu-id="88cd6-120">某些 CORS 問題無法解決，例如，當您的應用程式重新導向到 login.microsoftonline.com 以進行驗證時，存取權杖到期。</span><span class="sxs-lookup"><span data-stu-id="88cd6-120">Some CORS issues can't be resolved, such as expiration of the access token when your app redirects to login.microsoftonline.com for authentication.</span></span> <span data-ttu-id="88cd6-121">由於存取權杖過期，CORS 呼叫會失敗。</span><span class="sxs-lookup"><span data-stu-id="88cd6-121">As a result of the access token expiration, the CORS call then fails.</span></span> <span data-ttu-id="88cd6-122">此案例的因應措施是延長存取權杖的存留期，以避免它在使用者工作階段期間過期。</span><span class="sxs-lookup"><span data-stu-id="88cd6-122">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="88cd6-123">如需如何執行此作業的詳細資訊，請參閱 [Microsoft 身分識別平台中可設定的權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="88cd6-123">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
4. <span data-ttu-id="88cd6-124">**疑難排解 SAML 型 SSO**：建議您查看[登入設定 SAML 型單一登入的應用程式時發生問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)，以尋找您最可能遇到的問題的解決方案。</span><span class="sxs-lookup"><span data-stu-id="88cd6-124">**Troubleshooting SAML-based SSO**: We recommend checking [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) to find the solutions to the issues you are most likely to encounter.</span></span>
5. <span data-ttu-id="88cd6-125">**疑難排解密碼型 SSO**：建議您查看[疑難排解 Azure AD 中的密碼型單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)，以尋找您最可能遇到的問題的解決方案。</span><span class="sxs-lookup"><span data-stu-id="88cd6-125">**Troubleshooting password-based SSO**: We recommend checking [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) to find the solutions to the issues you are most likely to encounter.</span></span>
6. <span data-ttu-id="88cd6-126">**我遇到設定錯誤**：若要疑難排解設定錯誤，建議您查看下列文章：a.</span><span class="sxs-lookup"><span data-stu-id="88cd6-126">**I received a configuration error**: To troubleshoot configuration errors, we recommend checking the following articles: a.</span></span> <span data-ttu-id="88cd6-127">[登入設定 SAML 型單一登入的應用程式時發生問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) b.</span><span class="sxs-lookup"><span data-stu-id="88cd6-127">[Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) b.</span></span> <span data-ttu-id="88cd6-128">[已填寫認證，但擴充功能未提交認證](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them) c.</span><span class="sxs-lookup"><span data-stu-id="88cd6-128">[Credentials are filled in, but the extension does not submit them](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them) c.</span></span> <span data-ttu-id="88cd6-129">[已填寫並提交認證，但是頁面指出認證不正確](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) d.</span><span class="sxs-lookup"><span data-stu-id="88cd6-129">[Credentials are filled in and submitted, but the page indicates the credentials are incorrect](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) d.</span></span> [<span data-ttu-id="88cd6-130">使用者登入後，應用程式頁面顯示錯誤訊息</span><span class="sxs-lookup"><span data-stu-id="88cd6-130">An app page shows an error message after the user signs in</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
7. <span data-ttu-id="88cd6-131">**將無縫 SSO 與我的內部部署應用程式整合發生問題**：若要針對有關無縫 SSO 與內部部署應用程式整合的問題進行疑難排解，建議您查看下列文章：a.</span><span class="sxs-lookup"><span data-stu-id="88cd6-131">**I am having issues integrating Seamless SSO with my on-premises apps**: To troubleshoot issues regarding integration of Seamless SSO with on-premises apps, we recommend checking the following articles: a.</span></span> <span data-ttu-id="88cd6-132">[如何設定單一登入到應用程式 Proxy 應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to) b.</span><span class="sxs-lookup"><span data-stu-id="88cd6-132">[How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to) b.</span></span> <span data-ttu-id="88cd6-133">[對使用應用程式 Proxy 的內部部署應用程式進行 SAML 單一登入](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps) c.</span><span class="sxs-lookup"><span data-stu-id="88cd6-133">[SAML single sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps) c.</span></span> <span data-ttu-id="88cd6-134">[了解並解決 Azure Active Directory 應用程式 Proxy CORS 問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues) d.</span><span class="sxs-lookup"><span data-stu-id="88cd6-134">[Understand and solve Azure Active Directory Application Proxy CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues) d.</span></span> [<span data-ttu-id="88cd6-135">疑難排解應用程式 Proxy 的 Kerberos 限制委派設定</span><span class="sxs-lookup"><span data-stu-id="88cd6-135">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
8. <span data-ttu-id="88cd6-136">**我需要修正宣告或延長權杖的存留期。我需要變更工作階段的長度**：若要這麼做，建議您查看下列文章：a.</span><span class="sxs-lookup"><span data-stu-id="88cd6-136">**I need to fix the claims or extend the lifetime of a token. I need to change the length of a session**: To do this, we recommend checking the following articles: a.</span></span> <span data-ttu-id="88cd6-137">[自訂傳送到應用程式的 SAML 宣告](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) b.</span><span class="sxs-lookup"><span data-stu-id="88cd6-137">[Customize SAML claims sent to an application](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) b.</span></span> <span data-ttu-id="88cd6-138">[使用宣告感知應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) c.</span><span class="sxs-lookup"><span data-stu-id="88cd6-138">[Working with claims-aware apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) c.</span></span> <span data-ttu-id="88cd6-139">[Microsoft 身分識別平台中可設定的權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) d.</span><span class="sxs-lookup"><span data-stu-id="88cd6-139">[Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) d.</span></span> <span data-ttu-id="88cd6-140">[使用條件式存取設定驗證工作階段管理](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) e.</span><span class="sxs-lookup"><span data-stu-id="88cd6-140">[Configure authentication session management with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) e.</span></span> [<span data-ttu-id="88cd6-141">用於存取內部部署應用程式的 Cookie 設定</span><span class="sxs-lookup"><span data-stu-id="88cd6-141">Cookie settings for accessing on-premises applications</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)
9. <span data-ttu-id="88cd6-142">**我需要協助管理使用者和來賓使用者的 (B2B) 存取**：如需有關管理使用者和來賓使用者的存取的詳細資訊，建議您查看下列文章：a.</span><span class="sxs-lookup"><span data-stu-id="88cd6-142">**I need help managing my user's and guest users' (B2B) access**: For detailed information on managing user's and guest user's access, we recommend checking the following articles: a.</span></span> <span data-ttu-id="88cd6-143">[管理應用程式的存取](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management) b.</span><span class="sxs-lookup"><span data-stu-id="88cd6-143">[Managing access to apps](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management) b.</span></span> <span data-ttu-id="88cd6-144">[管理 Azure Active Directory 中應用程式的使用者指派](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) c.</span><span class="sxs-lookup"><span data-stu-id="88cd6-144">[Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) c.</span></span> <span data-ttu-id="88cd6-145">[設定適用於 B2B 共同作業的 SaaS 應用程式](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) d.</span><span class="sxs-lookup"><span data-stu-id="88cd6-145">[Configure SaaS apps for B2B collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) d.</span></span> <span data-ttu-id="88cd6-146">[為 Azure AD 中的 B2B 使用者授與您的內部部署應用程式的存取](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) e.</span><span class="sxs-lookup"><span data-stu-id="88cd6-146">[Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) e.</span></span> [<span data-ttu-id="88cd6-147">使用 Azure AD B2B 共同作業為本機管理的合作夥伴帳戶授與的雲端資源的存取</span><span class="sxs-lookup"><span data-stu-id="88cd6-147">Grant locally-managed partner accounts access to cloud resources using Azure AD B2B collaboration</span></span>](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)
10. <span data-ttu-id="88cd6-148">**我想要自訂我的應用程式**：如需有關自訂應用程式的詳細資訊，建議您查看下列文章：a.</span><span class="sxs-lookup"><span data-stu-id="88cd6-148">**I want to customize my apps**: For detailed information on customizing apps, we recommend checking the following articles: a.</span></span> <span data-ttu-id="88cd6-149">[設定使用 Azure AD 應用程式 Proxy 的自訂網域](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain) b.</span><span class="sxs-lookup"><span data-stu-id="88cd6-149">[Configure custom domains with Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain) b.</span></span> <span data-ttu-id="88cd6-150">[為已發佈的應用程式設定自訂首頁](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) c.</span><span class="sxs-lookup"><span data-stu-id="88cd6-150">[Set a custom home page for published apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) c.</span></span> [<span data-ttu-id="88cd6-151">萬用字元應用程式</span><span class="sxs-lookup"><span data-stu-id="88cd6-151">Wildcard applications</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard)
11. <span data-ttu-id="88cd6-152">**我在將應用程式從 AD FS 移轉至 Azure 時遇到問題**：若要針對將應用程式從 AD FS 移轉至 Azure 時遇到的問題進行疑難排解，建議您查看下列文章：a.</span><span class="sxs-lookup"><span data-stu-id="88cd6-152">**I'm having issues migrating my app from AD FS to Azure**: To troubleshoot issues encountered during migration of your app from AD FS to Azure, we recommend checking the following articles: a.</span></span> <span data-ttu-id="88cd6-153">[將應用程式驗證從 Active Directory 同盟服務移至 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) b.</span><span class="sxs-lookup"><span data-stu-id="88cd6-153">[Moving application authentication from Active Directory Federation Services to Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) b.</span></span> [<span data-ttu-id="88cd6-154">用於將應用程式移轉至 Azure Active Directory 的資源</span><span class="sxs-lookup"><span data-stu-id="88cd6-154">Resources for migrating applications to Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/migration-resources)
