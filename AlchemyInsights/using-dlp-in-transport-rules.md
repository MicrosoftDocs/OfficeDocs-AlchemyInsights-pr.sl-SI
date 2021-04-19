---
title: Uporaba pravilnika DLP v pravilih prenosa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827232"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="6157a-102">Uporaba pravilnika DLP v pravilih prenosa</span><span class="sxs-lookup"><span data-stu-id="6157a-102">Using DLP in transport rules</span></span>

<span data-ttu-id="6157a-103">Če želite preprečitev izgube podatkov (DLP) vgraditi v obstoječi prenos, v nastavitvah pravila prenosa uporabite pogoj »**Če so v sporočilu...občutljive informacije**«.</span><span class="sxs-lookup"><span data-stu-id="6157a-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="6157a-104">**Če želite dodatne podrobnosti, glejte:**</span><span class="sxs-lookup"><span data-stu-id="6157a-104">**For more details, see:**</span></span>

- <span data-ttu-id="6157a-105">Vgrajene vrste občutljivih informacij DLP v pravilih prenosa: [Vgraditev pravil o občutljivih informacijah](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="6157a-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="6157a-106">Pravilo lahko preizkusite tudi s preizkusom pravilnika ali brez njega tako, da za pravilo uporabite način preizkusa.</span><span class="sxs-lookup"><span data-stu-id="6157a-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="6157a-107">Ko ustvarite pravilo, počakajte 30 minut, preden ga preizkusite.</span><span class="sxs-lookup"><span data-stu-id="6157a-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="6157a-108">Glejte [Preizkus pravil za tok pošte/prenos](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="6157a-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="6157a-109">**Opomba**: če skušate v EAC uvesti nov pravilnik DLP s pravili prenosa, namesto tega uporabite [pravilnike DLP v središču za varnost in skladnost s predpisi](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="6157a-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
