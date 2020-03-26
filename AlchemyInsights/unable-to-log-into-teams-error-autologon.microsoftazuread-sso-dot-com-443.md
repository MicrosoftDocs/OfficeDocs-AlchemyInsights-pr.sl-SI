---
title: Ni se mogoče prijaviti v aplikacijo Teams zaradi napake autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932289"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="11cdd-102">Ni se mogoče prijaviti v aplikacijo Teams zaradi napake autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="11cdd-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="11cdd-103">Če je za vrsto preverjanja pristnosti O365 omogočena nemotena enotna prijava, bo treba intranetnim mestom morda dodali URL »autologon.microsoftazuread-sso.com«.</span><span class="sxs-lookup"><span data-stu-id="11cdd-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="11cdd-104">Če ste ga že dodeli zaupanja vrednim spletnim mestom, nemotena enotna prijava pa je v uporabi, ga odstranite iz razdelka zaupanja vrednih mest.</span><span class="sxs-lookup"><span data-stu-id="11cdd-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="11cdd-105">Preglejte [kontrolni seznam za odpravljanje težav pri nemoteni enotni prijavi](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="11cdd-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="11cdd-106">Upoštevajte ta navodila, da dodate URL seznamu intranetnih mest:</span><span class="sxs-lookup"><span data-stu-id="11cdd-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="11cdd-107">Zaženite Internet Explorer tako, da kliknete gumb **Start**.</span><span class="sxs-lookup"><span data-stu-id="11cdd-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="11cdd-108">V iskalno polje vnesite Internet Explorer, nato pa na seznamu rezultatov kliknite **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="11cdd-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="11cdd-109">Kliknite **Orodja** in nato **Internetne možnosti**.</span><span class="sxs-lookup"><span data-stu-id="11cdd-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="11cdd-110">Kliknite zavihek **Varnost**.</span><span class="sxs-lookup"><span data-stu-id="11cdd-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="11cdd-111">Zdaj kliknite **Lokalna intranetna mesta**, kliknite gumb **mesta** in nato še **Dodatno**.</span><span class="sxs-lookup"><span data-stu-id="11cdd-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="11cdd-112">Vnesite URL spletnega mesta in kliknite **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="11cdd-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="11cdd-113">Ko končate, kliknite **Zapri**.</span><span class="sxs-lookup"><span data-stu-id="11cdd-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="11cdd-114">Če želite več informacij, glejte [Dokumentacija za nemoteno enotno prijavo za O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (vključuje na pravilniku temelječ postopek za dodajanje URL-ja intranetnim mestom v 3. koraku).</span><span class="sxs-lookup"><span data-stu-id="11cdd-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
