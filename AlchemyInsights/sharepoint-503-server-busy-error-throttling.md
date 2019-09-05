---
title: SharePoint online Throttling
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751904"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5701b-102">SharePoint online Throttling</span><span class="sxs-lookup"><span data-stu-id="5701b-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="5701b-103">Uporabnik maj sprejemati a 503 pomočnik je zaposlen zmota čas poskus v pluti v SharePoint ali OneDrive položaj.</span><span class="sxs-lookup"><span data-stu-id="5701b-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="5701b-104">To napako lahko povzroči zadavljenje znotraj storitve SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5701b-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="5701b-105">SharePoint online uporablja zadaviti za ohranjanje optimalne učinkovitosti in zanesljivosti storitve SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="5701b-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="5701b-106">Throttling omejuje število uporabniških dejanj ali sočasnih klicev (po skriptu ali kodi), da se prepreči prekomerna uporaba virov.</span><span class="sxs-lookup"><span data-stu-id="5701b-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="5701b-107">Če vi delati zaslužiti Throttled, 99% od čas ono je zaradi šega zbornik.</span><span class="sxs-lookup"><span data-stu-id="5701b-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="5701b-108">Za več informacij o zadaviti glej, [ne pridobivanje zadaviti ali blokiran v SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="5701b-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="5701b-109">Če menite, da ta napaka ni povezana z Throttling, lahko preverite, ali je aktivno vzdrževanje, ki se pojavljajo na vašem najemniku z navigacijo do [centra za sporočila](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="5701b-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="5701b-110">Slednjič, zavarovati vi kratek obisk [usluga zdravje](https://portal.office.com/adminportal/home#/servicehealth) stran v ček zakaj poljuben Advisories/nezgoda to maj obstati dogodek.</span><span class="sxs-lookup"><span data-stu-id="5701b-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

