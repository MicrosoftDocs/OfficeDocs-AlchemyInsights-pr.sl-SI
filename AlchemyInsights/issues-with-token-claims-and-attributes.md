---
title: Težave s terjatvami in atributi žetona
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035973"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="31f9f-102">Težave s terjatvami in atributi žetona</span><span class="sxs-lookup"><span data-stu-id="31f9f-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="31f9f-103">**Posodobitev, konfiguracija ali odstranitev terjatev žetona**</span><span class="sxs-lookup"><span data-stu-id="31f9f-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="31f9f-104">Z uporabo imenika Azure Active Directory (Azure AD) lahko [prilagodite vrsto zahtevka za zahtevek vloge](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) v žetonu za odgovor, ki ga prejmete, ko pooblastite program.</span><span class="sxs-lookup"><span data-stu-id="31f9f-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="31f9f-105">Razvijalci aplikacij lahko v svojih aplikacijah Azure AD uporabljajo izbirne zahtevke, da določijo terjatve, ki jih želijo v žetonih, poslanih v njihovo aplikacijo.</span><span class="sxs-lookup"><span data-stu-id="31f9f-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="31f9f-106">Če želite več informacij, glejte [Omogočanje izbirnih zahtevkov za vašo aplikacijo](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="31f9f-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="31f9f-107">[Konfigurirajte zahteve skupine za aplikacije z imenikom Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="31f9f-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="31f9f-108">Če uporabljate nemoteno enotno prijavo v programu, glejte [prilagajanje terjatev, ki so bile izdane v SAML žetonu za podjetja](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="31f9f-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="31f9f-109">**Preslikava atributov» terjatve «**</span><span class="sxs-lookup"><span data-stu-id="31f9f-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="31f9f-110">Če želite konfigurirati pravilnik preslikave terjatev z uporabo lupine PowerShell, glejte [prilagajanje terjatev, ki jih oddajajo žetoni za določen program v najemniku (predogled)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="31f9f-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="31f9f-111">Atributi razširitve sheme Directory omogočajo shranjevanje dodatnih podatkov v imeniku Azure Active Directory na uporabniške predmete in druge predmete imenika, kot so skupine, podrobnosti najemnika, upravniki storitev.</span><span class="sxs-lookup"><span data-stu-id="31f9f-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="31f9f-112">Za oddajanje zahtevkov za aplikacije lahko uporabite le atribute razširitve na uporabniških predmetih.</span><span class="sxs-lookup"><span data-stu-id="31f9f-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="31f9f-113">[Z atributi pripone imeniške sheme v zahtevkih](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) je opisano, kako uporabite atribute razširitve sheme za pošiljanje uporabniških podatkov aplikacijam v žetonih.</span><span class="sxs-lookup"><span data-stu-id="31f9f-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="31f9f-114">Če želite več informacij o terjatvah žetona, glejte:</span><span class="sxs-lookup"><span data-stu-id="31f9f-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="31f9f-115">Terjatve v žetonih za dostop</span><span class="sxs-lookup"><span data-stu-id="31f9f-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="31f9f-116">Terjatve v id_token</span><span class="sxs-lookup"><span data-stu-id="31f9f-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="31f9f-117">[Terjatve](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , ki jih lahko pričakujete v žetonih z ID-jem in žetonih za dostop, ki jih je izdal AZURE ad B2C</span><span class="sxs-lookup"><span data-stu-id="31f9f-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="31f9f-118">Sklic na SAML žetona</span><span class="sxs-lookup"><span data-stu-id="31f9f-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
