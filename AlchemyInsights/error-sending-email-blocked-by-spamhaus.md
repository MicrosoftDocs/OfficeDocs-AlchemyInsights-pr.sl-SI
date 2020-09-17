---
title: Napaka pri pošiljanju e-pošte, ki jo je blokiral SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783819"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="74e07-102">Napaka pri pošiljanju e-pošte: gostitelj odjemalca je blokiran s storitvijo Spamhaus</span><span class="sxs-lookup"><span data-stu-id="74e07-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="74e07-103">Naslov IP, ki je poslal sporočilo, je na seznamu blokov, ki je v lasti [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="74e07-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="74e07-104">Razlogi za blokiranje s Spamhaus vključujejo ogrožene račune, ogrožene stroje, ki imajo v skupni rabi javni naslov IP in pravilnike internetnih storitev (ISP).</span><span class="sxs-lookup"><span data-stu-id="74e07-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="74e07-105">Možni popravki so:</span><span class="sxs-lookup"><span data-stu-id="74e07-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="74e07-106">Za blokirana dohodna sporočila, kjer nadzorujete izvorni e-poštni strežnik, morate določiti vzrok in odstraniti blok s spletnega mesta Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="74e07-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="74e07-107">Za blokirana dohodna sporočila, v katerih izvorni naslov IP pripada drugi osebi, mora lastnik naslova odstraniti blok s spletnega mesta Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="74e07-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="74e07-108">Če je naslov IP na seznamu za pravilnike (PBL), lahko lastnik dodeli drug statični naslov IP ali pa odstrani naslov iz PBL.</span><span class="sxs-lookup"><span data-stu-id="74e07-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="74e07-109">Za blokirana odhodna sporočila iz domene, ki je povezana z Microsoftom, se lahko prikaže to sporočilo o napaki, če so sporočila preusmerjena v storitev tretje osebe.</span><span class="sxs-lookup"><span data-stu-id="74e07-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="74e07-110">Z orodjem za iskanje v storitvi WHOIS lahko poiščete lastnika blokiranega naslova IP.</span><span class="sxs-lookup"><span data-stu-id="74e07-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
