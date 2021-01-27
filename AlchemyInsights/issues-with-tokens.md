---
title: 權杖問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/20/2021
ms.locfileid: "49911984"
---
# <a name="issues-with-tokens"></a><span data-ttu-id="7a3e3-102">權杖問題</span><span class="sxs-lookup"><span data-stu-id="7a3e3-102">Issues with tokens</span></span>

<span data-ttu-id="7a3e3-103">要管理與權杖相關的問題，可以執行以下步驟：</span><span class="sxs-lookup"><span data-stu-id="7a3e3-103">To manage issues related to tokens, you can perform the following steps:</span></span>

1. <span data-ttu-id="7a3e3-104">您可以指定由 Microsoft 身分識別平台發出的存取、識別碼或 SAML 權杖的存留期。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-104">You can specify the lifetime of an access, ID, or SAML token issued by Microsoft identity platform.</span></span> <span data-ttu-id="7a3e3-105">您可以為組織中的所有應用程式、多租用戶 (多組織) 應用程式或組織中的特定服務主體設定權杖存留期。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-105">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="7a3e3-106">有關詳細資訊，請參閱[Microsoft 身分識別平台中的可設定權杖存留期 (預覽)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-106">For more information, see [Configurable token lifetimes in Microsoft identity platform (preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
2. <span data-ttu-id="7a3e3-107">存取權杖使用戶端能夠安全地呼叫受保護的 Web API，並被 Web API 用來執行身份驗證和授權。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-107">Access tokens enable clients to securely call protected web APIs, and are used by web APIs to perform authentication and authorization.</span></span> <span data-ttu-id="7a3e3-108">根據 OAuth 規格，存取權杖是沒有設定格式的不透明字串 — 一些識別提供者 (IDP) 使用 GUID，另一些使用加密 blob。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-108">As per the OAuth specification, access tokens are opaque strings without a set format - some identity providers (IDPs) use GUIDs, others use encrypted blobs.</span></span> <span data-ttu-id="7a3e3-109">Microsoft 身分識別平台使用多種存取權杖格式，具體取決於接受權杖的 API 的設定。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-109">The Microsoft identity platform uses a variety of access token formats, depending on the configuration of the API that accepts the token.</span></span> <span data-ttu-id="7a3e3-110">要瞭解 API 如何驗證和使用存取權杖內的宣告，請參閱 [Microsoft 身分識別平台存取權杖](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-110">To learn how your API can validate and use the claims inside an access token, see [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).</span></span>
3. <span data-ttu-id="7a3e3-111">Microsoft 驗證程式庫 (MSAL) 支援在不同應用程式方案中使用的多個驗證流程。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-111">The Microsoft Authentication Library (MSAL) supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="7a3e3-112">有關更多資訊，請參閱[驗證流程](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes)。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-112">For more information, see [Authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).</span></span>
4. <span data-ttu-id="7a3e3-113">OAuth2.0 授權碼授權可用於安裝在裝置上的應用程式，以存取受保護的資源，如 Web API。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-113">The OAuth 2.0 authorization code grant can be used in apps that are installed on a device to gain access to protected resources, such as web APIs.</span></span> <span data-ttu-id="7a3e3-114">使用 OAuth 2.0 的 Microsoft 身分識別平台實作，可以向行動裝置和桌面應用程式新增登入和 API 存取。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-114">Using the Microsoft identity platform implementation of OAuth 2.0, you can add sign-in and API access to your mobile and desktop apps.</span></span> <span data-ttu-id="7a3e3-115">請參閱 [Microsoft 身分識別平台和 OAuth 2.0 授權碼流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token)，瞭解如何使用任何語言直接對應用程式中的通訊協定進行程式設計。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-115">See [Microsoft identity platform and OAuth 2.0 authorization code flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) for how to program directly against the protocol in your application, using any language.</span></span>
5. <span data-ttu-id="7a3e3-116">OpenID Connect (OIDC) 是建立在 oauth2.0 上的驗證通訊協定，可以使用它安全地將使用者登入至應用程式。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-116">OpenID Connect (OIDC) is an authentication protocol built on OAuth 2.0 that you can use to securely sign in a user to an application.</span></span> <span data-ttu-id="7a3e3-117">使用 Microsoft 身分識別平台端點的 OpenID Connect 實作時，可以向應用程式新增登入和 API 存取。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-117">When you use the Microsoft identity platform endpoint's implementation of OpenID Connect, you can add sign-in and API access to your apps.</span></span> <span data-ttu-id="7a3e3-118">[Microsoft 身分識別平台和 OpenID Connect 通訊協定](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request)演示了如何獨立於語言進行此動作，並描述了如何在不使用任何 Microsoft 開放原始碼庫的情況下傳送和接收 HTTP 訊息。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-118">[Microsoft identity platform and OpenID Connect protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) shows how to do this independent of language and describes how to send and receive HTTP messages without using any Microsoft open-source libraries.</span></span>
    - <span data-ttu-id="7a3e3-119">UserInfo 端點是 OIDC 標準的一部分，專爲傳回有關已驗證使用者的宣告而設計。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-119">The UserInfo endpoint is part of the OIDC standard, designed to return claims about the user that authenticated.</span></span> <span data-ttu-id="7a3e3-120">有關詳細資訊，請參閱 [Microsoft 身分識別平台 UserInfo 端點](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead)。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-120">For more information, see [Microsoft identity platform UserInfo endpoint](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).</span></span>
    - <span data-ttu-id="7a3e3-121">[使用 Azure AD 和 OpenID Connect 在 Web 應用程式中呼叫 Web API](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) 範例顯示如何建置 MVC Web 應用程式，該應用程式使用 OpenID Connect 通訊協定以使用 Azure AD 進行登入，然後使用透過 OAuth 2.0 取得的權杖在登入使用者的身分識別下呼叫 Web API。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-121">The [Calling a web API in a web app using Azure AD and OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) sample shows how to build an MVC web application that uses Azure AD for sign-in using the OpenID Connect protocol, and then call a web API under the signed-in user's identity using tokens obtained via OAuth 2.0.</span></span> <span data-ttu-id="7a3e3-122">本示例使用 OpenID Connect ASP .Net OWIN 中介軟體和 ADAL .Net。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-122">This sample uses the OpenID Connect ASP .Net OWIN middleware and ADAL .Net.</span></span>
6. <span data-ttu-id="7a3e3-123">[設定應用程式以公開 Web API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) — 在此快速入門中，可以向 Microsoft 身分識別平台登錄 Web API，並透過新增範例範圍將其公開給用戶端應用程式。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-123">[Configure an application to expose a web API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) - In this quickstart, you register a web API with the Microsoft identity platform and expose it to client apps by adding an example scope.</span></span> <span data-ttu-id="7a3e3-124">注冊 Web API 並透過作用域公開它，可以向存取您的 API 的授權使用者和用戶端應用程式提供對其資源之以權限為基礎的存取。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-124">By registering your web API and exposing it through scopes, you can provide permissions-based access to its resources to authorized users and client apps that access your API.</span></span>
7. <span data-ttu-id="7a3e3-125">在 Azure Active Directory B2C (Azure AD B2C) 中，資源擁有者密碼認證 (ROPC) 流程是 OAuth 標準驗證流程。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-125">In Azure Active Directory B2C (Azure AD B2C), the resource owner password credentials (ROPC) flow is an OAuth standard authentication flow.</span></span> <span data-ttu-id="7a3e3-126">在此流程中，應用程式（也稱為信賴憑證者）為權杖交換有效認證。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-126">In this flow, an application, also known as the relying party, exchanges valid credentials for tokens.</span></span> <span data-ttu-id="7a3e3-127">認證包括使用者識別碼和密碼。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-127">The credentials include a user ID and password.</span></span> <span data-ttu-id="7a3e3-128">傳回的權杖是識別碼權杖、存取權杖和重新整理權杖。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-128">The tokens returned are an ID token, access token, and a refresh token.</span></span> <span data-ttu-id="7a3e3-129">有關更多資訊，請參閱[在 Azure Active Directory B2C 中設定資源擁有者密碼認證流程](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow)。</span><span class="sxs-lookup"><span data-stu-id="7a3e3-129">For more information, see [Set up a resource owner password credentials flow in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow).</span></span> 
