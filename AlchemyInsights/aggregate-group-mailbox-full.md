---
title: AggregateGroupMailbox Full NDR, ki ste ga prejeli za e-pošto, poslano v skupino Microsoft 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722079"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a><span data-ttu-id="400b6-102">AggregateGroupMailbox Full NDR, ki ste ga prejeli za e-pošto, poslano v skupino Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="400b6-102">AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group</span></span>

<span data-ttu-id="400b6-103">Z ukazom EKSO Shell lahko ustvarite pravilo za prenos prenosa za tiho spuščanje e-poštnih sporočil, poslanih v združevalni nabiralnik skupine:</span><span class="sxs-lookup"><span data-stu-id="400b6-103">Use the following EXO Shell command to create an Exchange transport rule to silently drop emails sent to aggregate group mailbox:</span></span>

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> <span data-ttu-id="400b6-104">Zamenjajte naslov SMTP v storitvi **SentTo** z naslovom SMTP za Združeno skupino nabiralnika v najemniku.</span><span class="sxs-lookup"><span data-stu-id="400b6-104">Replace the SMTP address in **-SentTo** with SMTP address of aggregate group mailbox in your tenant.</span></span> <span data-ttu-id="400b6-105">Naslov SMTP Združenega skupinskega nabiralnika lahko pridobite iz prejetega poročila NDR.</span><span class="sxs-lookup"><span data-stu-id="400b6-105">You can get the SMTP address of aggregate group mailbox from the NDR received.</span></span>



