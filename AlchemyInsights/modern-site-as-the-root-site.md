---
title: Sodobna lokacija kot korensko mesto
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666886"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="ef876-102">Moderno mesto kot korensko mesto</span><span class="sxs-lookup"><span data-stu-id="ef876-102">Modern site as root site</span></span>

<span data-ttu-id="ef876-103">Začeli smo z uvajanjem nove funkcije, ki vam bo omogočila, da [zamenjate spletno mesto klasičnega spletnega mesta s sodobnim mestom](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="ef876-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="ef876-104">Uporabite funkcijo» [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) «, da zamenjate mesto mesta z drugim mestom, medtem ko arhivirate izvirno mesto.</span><span class="sxs-lookup"><span data-stu-id="ef876-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="ef876-105">Na voljo za spletno mesto skupine (ni povezano s skupino) in mesto za komunikacijo.</span><span class="sxs-lookup"><span data-stu-id="ef876-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="ef876-106">Klasičnega korenskega mesta ne izbrišite, če želite ustvariti sodobno mesto za komunikacijo.</span><span class="sxs-lookup"><span data-stu-id="ef876-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="ef876-107">Microsoft ne podpira tega.</span><span class="sxs-lookup"><span data-stu-id="ef876-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="ef876-108">Če izbrišete korensko mesto, bodo vsa SharePointova mesta v organizaciji nedostopna vsem uporabnikom, dokler ne obnovite mesta ali ustvarite novo mesto v istem URL-ju.</span><span class="sxs-lookup"><span data-stu-id="ef876-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="ef876-109">To funkcijo bomo komunicirali prek središča za sporočila.</span><span class="sxs-lookup"><span data-stu-id="ef876-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="ef876-110">Pričakujete, da bo funkcija v vašem najemniku kmalu vklopljena.</span><span class="sxs-lookup"><span data-stu-id="ef876-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="ef876-111">Znane težave s spletnimi mesti za zamenjavo</span><span class="sxs-lookup"><span data-stu-id="ef876-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="ef876-112">Ciljno mesto lahko vrne napako» not found «(HTTP 404) za kratek čas.</span><span class="sxs-lookup"><span data-stu-id="ef876-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="ef876-113">Vsebino bo treba znova preiskati in posodobiti indeks iskanja.</span><span class="sxs-lookup"><span data-stu-id="ef876-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="ef876-114">Tukaj ni potrebnega ročnega koraka, to bo samodejno opravljeno.</span><span class="sxs-lookup"><span data-stu-id="ef876-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="ef876-115">Vse, kar je odvisno od povezav» statičnih «(na primer sinhronizacije datotek in datotek programa OneNote), bo treba ročno popraviti.</span><span class="sxs-lookup"><span data-stu-id="ef876-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="ef876-116">Če želite zagotoviti, da so še vedno pravilno povezani, je treba potrditi mesta strežnika Project Server.</span><span class="sxs-lookup"><span data-stu-id="ef876-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
