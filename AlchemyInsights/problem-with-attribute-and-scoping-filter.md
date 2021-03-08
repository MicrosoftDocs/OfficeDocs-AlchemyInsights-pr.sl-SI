---
title: Težava z filtrom» atribut «in» določanje obsega «
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482922"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="8e82d-102">Težava z filtrom» atribut «in» določanje obsega «</span><span class="sxs-lookup"><span data-stu-id="8e82d-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="8e82d-103">**Težave s spornimi vrednostmi UPN**</span><span class="sxs-lookup"><span data-stu-id="8e82d-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="8e82d-104">Delovni dan za omogočanje uporabe delovnega dne na spletnem mestu AD uporabnik omogoča omogočanje uporabe sporočila o napaki **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span><span class="sxs-lookup"><span data-stu-id="8e82d-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="8e82d-105">Operacija ni uspela, ker vrednost UPN za dodatek/spreminjanje ni enolična za celotno vrsto gozda.</span><span class="sxs-lookup"><span data-stu-id="8e82d-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="8e82d-106">Podrobnosti o napaki: **CONSTRAINT_ATT_TYPE-userPrincipalName**.</span><span class="sxs-lookup"><span data-stu-id="8e82d-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="8e82d-107">Vrednost **userPrincipalName** , ki jo priključek delovnega dne poskuša nastaviti, ko ustvarja uporabniški račun oglasa že obstaja v ciljni domeni oglasa.</span><span class="sxs-lookup"><span data-stu-id="8e82d-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="8e82d-108">To pomeni, da uporabnik že obstaja in preverjanje ujemanja ID-ja ni uspelo za uporabnika ali (2) pravilo generiranja UPN je ustvarilo sporno vrednost.</span><span class="sxs-lookup"><span data-stu-id="8e82d-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="8e82d-109">Tukaj so navodila za predlagano rešitev:</span><span class="sxs-lookup"><span data-stu-id="8e82d-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="8e82d-110">Če uporabnik že obstaja in preverjanje ujemanja ID-ja ni uspelo povezati računa za delovni dan z računom imenika Active Directory, nato preverite, ali je atribut» ujemanje ID-ja «(običajno **IDzaposlenega**) v obeh delovnih dneh in ad natančno ujemanje.</span><span class="sxs-lookup"><span data-stu-id="8e82d-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="8e82d-111">Če se ne ujemajo, je to podatkovna težava, ki jo je treba popraviti.</span><span class="sxs-lookup"><span data-stu-id="8e82d-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="8e82d-112">Če je na primer IDZaposlenega v delovnem programu 001052 in je v OGLASu 1052, potem mehanizem za omogočanje uporabe ne bo mogel povezati dveh računov in bo poskušal ustvariti uporabnika, ki že obstaja.</span><span class="sxs-lookup"><span data-stu-id="8e82d-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="8e82d-113">Rešitev v tem primeru je, da spremenite vrednost **IDzaposlenega** v programu ad, da vključite vodilne ničle, da bo 001052.</span><span class="sxs-lookup"><span data-stu-id="8e82d-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="8e82d-114">Če izraz, ki ustvarja UPN, ne ustvari enolične vrednosti, uporabite funkcijo de-podvajanja **SelectUniqueValue** , da vsakič ustvarite enolično vrednost.</span><span class="sxs-lookup"><span data-stu-id="8e82d-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="8e82d-115">**Delovni dan za omogočanje uporabe uporabnika ne Nastavi vrednosti atributa upravitelja za uporabniški račun OGLASa**</span><span class="sxs-lookup"><span data-stu-id="8e82d-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="8e82d-116">Posel za omogočanje uporabe uporabnika delovnega dne v OGLASu ne določa vrednosti atributa **upravitelja** za UPORABNIŠKE račune oglasa.</span><span class="sxs-lookup"><span data-stu-id="8e82d-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="8e82d-117">Ko je to vedenje prikazano, sta na voljo dva možna scenarija:</span><span class="sxs-lookup"><span data-stu-id="8e82d-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="8e82d-118">Upravitelja v delavniku ni mogoče razrešiti z ustreznim uporabniškim računom OGLASa, ker upravitelj ni v obsegu.</span><span class="sxs-lookup"><span data-stu-id="8e82d-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="8e82d-119">V scenariju z **več domenami oglasa** upravitelj v delovnem programu ni prisoten v isti domeni kot uporabnik.</span><span class="sxs-lookup"><span data-stu-id="8e82d-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="8e82d-120">Če želite odpraviti težavo, poskusite s temi koraki:</span><span class="sxs-lookup"><span data-stu-id="8e82d-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="8e82d-121">Če ste določili filtre za določanje obsega, najprej preverite, ali je upravitelj v obsegu in ali ustreza stavku za določanje obsega.</span><span class="sxs-lookup"><span data-stu-id="8e82d-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="8e82d-122">Če upravitelj ne izpolnjuje filtra za določanje obsega, spremenite filter tako, da je upravitelj tudi v obsegu uporabe postopka uporabe.</span><span class="sxs-lookup"><span data-stu-id="8e82d-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="8e82d-123">Če imate več domen oglasov, ima povezovalnik znano omejitev nezmožnosti za razreševanje sklicev upravitelja navzkrižne domene.</span><span class="sxs-lookup"><span data-stu-id="8e82d-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="8e82d-124">Če želite več informacij o konfiguriranju delovnega dne za avtomatizirano omogočanje uporabe, glejte [Vadnica: konfiguracija delovnega dne za samodejno omogočanje uporabe uporabnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="8e82d-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>












