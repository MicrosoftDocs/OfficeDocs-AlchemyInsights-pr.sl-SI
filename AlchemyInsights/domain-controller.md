---
title: Krmilnik domene
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
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901314"
---
# <a name="domain-controller"></a><span data-ttu-id="fcaba-102">Krmilnik domene</span><span class="sxs-lookup"><span data-stu-id="fcaba-102">Domain controller</span></span>

<span data-ttu-id="fcaba-103">**Ne morete omogočiti ZVOČNIh naprav – DS ali uvedbe ni mogoče**</span><span class="sxs-lookup"><span data-stu-id="fcaba-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="fcaba-104">Če želite odpraviti težavo z domensko storitvijo Azure AD (ZVOČNa-DS), ki ni omogočena ali ni bila uvedena, izvedite te korake:</span><span class="sxs-lookup"><span data-stu-id="fcaba-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="fcaba-105">Če uporabljate že obstoječo navidezno omrežje, potrdite NSG za pravila, ki blokirajo vrata, potrebna za sinhronizacijo v storitvi ZVOČNa-DS v portalu https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="fcaba-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="fcaba-106">Preverite, ali je odgovor na sporočilo o napaki v tem vodniku za odpravljanje težav, ki je na voljo  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="fcaba-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="fcaba-107">Poskusite uporabiti domenske storitve Azure AD v novem navideznem omrežju.</span><span class="sxs-lookup"><span data-stu-id="fcaba-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="fcaba-108">Navodila za uvod v priročnik za uvajanje ZVOČNIh naprav – DS, ki je na voljo na spletnem mestu [Vadnica za ustvarjanje domenskih storitev storitve AZURE ad](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="fcaba-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="fcaba-109">Če imate težave z uvajanjem domen v storitvi Azure AD Services, glejte [Odpravljanje težav z domenami storitve AZURE ad](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , da odpravite pogoste napake, s katerimi lahko znova začnete delati.</span><span class="sxs-lookup"><span data-stu-id="fcaba-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="fcaba-110">**Ne morete onemogočiti ZVOČNIh-DS**</span><span class="sxs-lookup"><span data-stu-id="fcaba-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="fcaba-111">ZVOČNa-DS ne more biti začasno ustavljena.</span><span class="sxs-lookup"><span data-stu-id="fcaba-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="fcaba-112">Če želite prenehati uporabljati upravljano domeno, jo morate izbrisati.</span><span class="sxs-lookup"><span data-stu-id="fcaba-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="fcaba-113">Če naletite na težave, razrešite pogosta sporočila o napakah in povezane korake za odpravljanje težav, ki vam bodo v pomoč pri ponovnem zagonu, glejte [Odpravljanje težav z domenami storitve Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="fcaba-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
