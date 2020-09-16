---
title: O identiteti v Bastard
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664186"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="a0c9e-102">O identiteti v Bastard</span><span class="sxs-lookup"><span data-stu-id="a0c9e-102">About identity in Yammer</span></span>

<span data-ttu-id="a0c9e-103">Priporočamo, da v vseh omrežjih naredite te korake, da se izognete težavam, povezanim z identiteto:</span><span class="sxs-lookup"><span data-stu-id="a0c9e-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="a0c9e-104">Uveljavite identiteto sistema Office 365 po omogočanju uporabe računov Microsoft 365 za uporabnike v storitvi Azure AD za zagotovitev, da se vsi uporabniki vpišejo s primarnim računom Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a0c9e-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="a0c9e-105">Če želite več informacij, glejte [uveljavitev identitete sistema Office 365 za uporabnike Bastard](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="a0c9e-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="a0c9e-106">Uskladitev več Bastard omrežij.</span><span class="sxs-lookup"><span data-stu-id="a0c9e-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="a0c9e-107">Podedovane Bastard konfiguracije omogočajo, da je več Bastard omrežij povezano z enim najemnikom.</span><span class="sxs-lookup"><span data-stu-id="a0c9e-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="a0c9e-108">Če želite več informacij, glejte [selitev omrežja – uskladitev več Bastard omrežij](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="a0c9e-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="a0c9e-109">Po želji lahko uveljavite licenciranje za Bastard za blokiranje uporabnikov iz Bastard, če nimajo licence.</span><span class="sxs-lookup"><span data-stu-id="a0c9e-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="a0c9e-110">Če želite več informacij, glejte [upravljanje Bastard uporabniških licenc v sistemu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="a0c9e-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="a0c9e-111">Na koncu Revidirajte seznam uporabnikov starejših Bastard omrežij in ustavite starejše uporabnike.</span><span class="sxs-lookup"><span data-stu-id="a0c9e-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="a0c9e-112">Priporočamo vam, da začasno ustavite (deaktivirate) uporabnike, namesto da jih izbrišete, ker je brisanje nepreklicno.</span><span class="sxs-lookup"><span data-stu-id="a0c9e-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="a0c9e-113">Če želite več informacij, glejte [nadzor Bastard uporabnikov v omrežjih, povezanih s sistemom Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) in [odstranjevanje uporabnikov](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="a0c9e-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="a0c9e-114">Ko konfigurirate Bastard s temi koraki, boste prav tako pripravljeni, da konfigurirate Bastard omrežje za izvorni način za Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="a0c9e-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="a0c9e-115">Če želite več informacij, glejte [Konfiguracija omrežja Bastard za izvorni način za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="a0c9e-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>