---
title: 1065 zastaranje odhodnega IP naslova EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704613"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="641d0-102">Zastareanje razponov odhodnega IP-naslova EOP</span><span class="sxs-lookup"><span data-stu-id="641d0-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="641d0-103">Odkrili smo morebitno težavo z vašo organizacijo, ki bi (če ne bi bila popravljena do 26. oktobra, 2018) morda prekinil pretok pošte v krajevnih ali zunanjih destinacijah.</span><span class="sxs-lookup"><span data-stu-id="641d0-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="641d0-104">Kot je bilo že sporočeno, da bi poenostavili upravljanje obsega IP naslovov, utrimo obsege IP naslovov za Exchange Online Protection (EOP), ki se uporabljajo za pošiljanje in prejemanje e-pošte zunaj Microsofta 365.</span><span class="sxs-lookup"><span data-stu-id="641d0-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="641d0-105">Naša analiza kaže, da eden ali več zunanjih virov e-pošte ali ciljev, ki ste jih konfigurirali v konektorje za pretok pošte, ne sprejema povezav iz obsegov naslovov IP, prikazanih [tukaj](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="641d0-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="641d0-106">Zakon pred oktobrom 26th za zagotovitev teh virov in destinacij bo sprejela povezave in iz vseh [objavljenih IP naslove EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="641d0-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="641d0-107">Če želite več informacij o tej spremembi, glejte sporočila center Posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)ali [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="641d0-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="641d0-108">**Opombe**: Če ste že uporabljali IP ali URL objavljanje prek HTML, XML in RSS za končne posodobitve, morate tudi preseliti v nove spletne storitve za avtomatizacijo teh vrst posodobitev.</span><span class="sxs-lookup"><span data-stu-id="641d0-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="641d0-109">Če želite več informacij, glejte [kategorije končnih točk microsoft 365 in spletna storitev microsoft 365 IP naslov in URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="641d0-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
