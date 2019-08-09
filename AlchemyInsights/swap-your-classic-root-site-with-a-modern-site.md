---
title: Swap vaš Classic korensko mesto z moderno mesto
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270760"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="7b2e8-102">Swap vaš Classic korensko mesto z moderno mesto</span><span class="sxs-lookup"><span data-stu-id="7b2e8-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="7b2e8-103">Če vaš okolja je bil ustanovljen pred aprila 2019, lahko spremenite korensko mesto na sodobno spletno stran z uporabo Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7b2e8-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="7b2e8-104">Če imate drugo mesto, ki ga želite uporabiti kot korensko mesto, lahko zamenjate (swap) je koren mesto z njim.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="7b2e8-105">Uporabite [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) da zamenjate mesto mesto z drugim mestom med arhiviranjem na izvirno mesto.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="7b2e8-106">Na voljo za mesto ekipe (ne povezani skupini) in komunikacija stran.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="7b2e8-107">Bo treba uvesti dodatne zmožnosti kmalu ki vam bo omogočilo, da še naprej uporabljati vsebino na mestu, ampak spremeniti obstoječega mesta na mesto komunikacije.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="7b2e8-108">Te zmogljivosti bo valjani ven postopoma.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="7b2e8-109">Nadaljuj, da preverite Office 365 vest središče za posodobitve.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="7b2e8-110">Znane težave z zamenjavo strani</span><span class="sxs-lookup"><span data-stu-id="7b2e8-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="7b2e8-111">Ciljno mesto lahko vrne "not found" napaka (HTTP 404) za kratek čas.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="7b2e8-112">Vsebino morate recrawled želite posodobiti kazalo iskanja.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="7b2e8-113">Ni noben priročnik korak zahteva - to hoteti obstati velja automatically.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="7b2e8-114">Vse, kar je odvisno od "statična" povezave (na primer datoteka sinhronizacijo in OneNote datoteke) morali ročno popraviti.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="7b2e8-115">Če se vir organizacijske novicami, posodobite URL.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="7b2e8-116">Dobili seznam vseh organizacijskih novicami.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="7b2e8-117">Projekt strežnika straneh morda morali potrditi, da se zagotovi, da so še vedno povezani pravilno.</span><span class="sxs-lookup"><span data-stu-id="7b2e8-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





