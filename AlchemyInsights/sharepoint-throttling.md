---
title: Spletno mesto za zadaviti SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931458"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="d2340-102">Spletno mesto za zadaviti SharePoint</span><span class="sxs-lookup"><span data-stu-id="d2340-102">SharePoint Online throttling</span></span>

<span data-ttu-id="d2340-103">**Pomembno**: mnogi uporabniki storitve SharePoint online in OneDrive vodijo aplikacije, ki so kritične za podjetja, proti storitvi, ki se zažene v ozadju.</span><span class="sxs-lookup"><span data-stu-id="d2340-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="d2340-104">Ti vključujejo vsebino migracije, preprečevanje izgube podatkov (DLP), in backup rešitve.</span><span class="sxs-lookup"><span data-stu-id="d2340-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="d2340-105">V teh neprimerljivo času, smo sprejeti ukrepe za zagotovitev, da SharePoint online in storitve OneDrive ostajajo zelo na voljo in zanesljive za vaše uporabnike, ki so odvisni od storitve bolj kot kdajkoli prej v oddaljenih delovnih scenarijev.</span><span class="sxs-lookup"><span data-stu-id="d2340-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="d2340-106">V podporo temu cilju smo izvedli strožje omejitve omejevanja osnovnih aplikacij (migracije, DLP in varnostne rešitve) med tednom podnevi.</span><span class="sxs-lookup"><span data-stu-id="d2340-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="d2340-107">Pričakovati je, da bodo te aplikacije dosegle zelo omejene prepustne čase v teh časih.</span><span class="sxs-lookup"><span data-stu-id="d2340-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="d2340-108">Vendar pa bo v večernih urah in vikendih za regijo, storitev pripravljena obdelati bistveno večji obseg zahtevkov iz ozadja aplikacij.</span><span class="sxs-lookup"><span data-stu-id="d2340-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="d2340-109">**Spletno mesto za zadaviti SharePoint**</span><span class="sxs-lookup"><span data-stu-id="d2340-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="d2340-110">SharePoint online uporablja zadaviti za ohranjanje optimalne učinkovitosti in zanesljivosti storitve SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="d2340-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="d2340-111">Throttling omejuje število uporabniških dejanj ali sočasnih klicev (po skriptu ali kodi), da se prepreči prekomerna uporaba virov.</span><span class="sxs-lookup"><span data-stu-id="d2340-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="d2340-112">Več informacij najdete v spodnjih povezavah.</span><span class="sxs-lookup"><span data-stu-id="d2340-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="d2340-113">Izogibajte se temu, da bi v SharePoint online dobili ali blokirali</span><span class="sxs-lookup"><span data-stu-id="d2340-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="d2340-114">Podatki migracije in SPO Throttling</span><span class="sxs-lookup"><span data-stu-id="d2340-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="d2340-115">Hitrost selitve storitve SharePoint online in OneDrive</span><span class="sxs-lookup"><span data-stu-id="d2340-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="d2340-116">Rokovanje s storitvijo SharePoint online z uporabo eksponentne nazaj</span><span class="sxs-lookup"><span data-stu-id="d2340-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="d2340-117">Načrtovanje zmogljivosti in preskušanje obremenitve SharePoint online</span><span class="sxs-lookup"><span data-stu-id="d2340-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

