---
title: 726 blokiranje posredovanja e-pošte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219871"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="14f26-102">Blokiranje ali odblokiranje posredovanja e-pošte</span><span class="sxs-lookup"><span data-stu-id="14f26-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="14f26-103">Če želite omogočiti ali onemogočiti posredovanje e-pošte za določen nabiralnik, glejte [Konfiguracija posredovanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="14f26-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="14f26-104">Na ravni najemnika se nadzor zunanjega posredovanja izvaja s pravilnikom odhodne neželene pošte.</span><span class="sxs-lookup"><span data-stu-id="14f26-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="14f26-105">Če je nastavljena na izklopljeno ali samodejno, lahko blokira posredovanje e-pošte s storitvijo» 550 5.7.520 Access je zavrnjena, vaša organizacija ne dovoljuje zunanjega posredovanja «.</span><span class="sxs-lookup"><span data-stu-id="14f26-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="14f26-106">Če je bila preusmeritev nastavljena na blokirano, je to napaka, ki jo bodo videli uporabniki.</span><span class="sxs-lookup"><span data-stu-id="14f26-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="14f26-107">Če je preusmeritev blokirana, se prepričajte, da je pravilnik konfiguriran tako, da omogoča zunanjo samoposredovanje.</span><span class="sxs-lookup"><span data-stu-id="14f26-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="14f26-108">Pravilnik za filtriranje neželene pošte lahko preverite v središču za varnost in skladnost s predpisi ali z ukazom Get-HostedOutboundSpamFilterPolicy | ime FL, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="14f26-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="14f26-109">Če želite nastaviti samodejno blokiranje blokiranja, vam bo isti ukaz povedal trenutno stanje pravilnika.</span><span class="sxs-lookup"><span data-stu-id="14f26-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="14f26-110">Opomba: priporočamo, da zunanje samodejno posredovanje onemogočite na privzetem pravilniku za filtriranje neželene pošte in jo omogočite le za uporabnike, ki potrebujejo zunanjo preusmeritev tako, da ustvarijo pravilnik po meri za te uporabnike.</span><span class="sxs-lookup"><span data-stu-id="14f26-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="14f26-111">Več informacij najdete v članku [Konfiguriranje posredovanja zunanjih e-poštnih sporočil v sistemu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="14f26-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>