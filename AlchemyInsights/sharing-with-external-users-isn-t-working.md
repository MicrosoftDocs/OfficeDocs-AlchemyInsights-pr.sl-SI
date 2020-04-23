---
title: Deljenje z zunanjimi uporabniki ne deluje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 285535d6144825f0935bf72579a483260c2f2bd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767265"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="cb6d4-102">Odpravljanje težav pri skupni rabi SharePointove vsebine z zunanjimi Uporabniki</span><span class="sxs-lookup"><span data-stu-id="cb6d4-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="cb6d4-103">Prepričajte se, da je zunanja skupna raba vklopljena za vašo organizacijo:</span><span class="sxs-lookup"><span data-stu-id="cb6d4-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="cb6d4-104">Pojdite na [stran» &amp; dodatki za storitve «v skrbniškem središču za Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)in kliknite **mesta**.</span><span class="sxs-lookup"><span data-stu-id="cb6d4-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="cb6d4-105">Prepričajte se, da je nastavitev vklopljena.</span><span class="sxs-lookup"><span data-stu-id="cb6d4-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="cb6d4-106">Če je izbrana možnost» samo obstoječi zunanji Uporabniki «, se prepričajte, da je zunanji uporabnik naveden v skrbniškem središču Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cb6d4-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="cb6d4-107">Prepričajte se, da je zunanja skupna raba vklopljena za spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="cb6d4-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="cb6d4-108">Za klasično zbirko mest:</span><span class="sxs-lookup"><span data-stu-id="cb6d4-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="cb6d4-109">V novem skrbniškem središču SharePoint v levem podoknu kliknite **mesta**.</span><span class="sxs-lookup"><span data-stu-id="cb6d4-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="cb6d4-110">Izberite spletno mesto ali spletna mesta in na traku kliknite **Skupna raba**.</span><span class="sxs-lookup"><span data-stu-id="cb6d4-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="cb6d4-111">Za spletno mesto skupine, ki pripada skupini Office 365 ali na mestu za komunikacijo:</span><span class="sxs-lookup"><span data-stu-id="cb6d4-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="cb6d4-112">Te nove vrste mest imajo enako nastavitev skupne rabe kot nastavitev za celotno organizacijo, razen če nastavitev za celotno organizacijo omogoča skupno rabo datotek s povezavami, ki ne zahtevajo prijave.</span><span class="sxs-lookup"><span data-stu-id="cb6d4-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="cb6d4-113">V tem primeru spletna mesta omogočajo skupno rabo z novimi in obstoječimi zunanjimi Uporabniki, ki se vpisljajo.</span><span class="sxs-lookup"><span data-stu-id="cb6d4-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="cb6d4-114">Če želite spremeniti nastavitev za določena mesta, uporabite nov SharePointov skrbniški center ali PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cb6d4-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="cb6d4-115">[Več informacij](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="cb6d4-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="cb6d4-116">Nastavitev zunanje delitve za poljubno spletno mesto je lahko bolj omejevalna kot nastavitev za celotno organizacijo, vendar ne bolj permisivno kot nastavitev za celotno organizacijo.</span><span class="sxs-lookup"><span data-stu-id="cb6d4-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

