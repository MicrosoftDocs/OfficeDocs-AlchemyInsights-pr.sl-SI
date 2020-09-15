---
title: Skupna raba z zunanjimi uporabniki ne deluje
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691591"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="37319-102">Odpravljanje težav pri skupni rabi SharePointovih vsebin z zunanjimi Uporabniki</span><span class="sxs-lookup"><span data-stu-id="37319-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="37319-103">Prepričajte se, da je za vašo organizacijo vklopljena zunanja skupna raba:</span><span class="sxs-lookup"><span data-stu-id="37319-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="37319-104">Pojdite na [stran dodatki storitve &amp; v skrbniškem središču za Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)in kliknite **spletna mesta**.</span><span class="sxs-lookup"><span data-stu-id="37319-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="37319-105">Prepričajte se, da je nastavitev vklopljena na» vklopljeno «.</span><span class="sxs-lookup"><span data-stu-id="37319-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="37319-106">Če je izbrana možnost» le obstoječi zunanji Uporabniki «, se prepričajte, da je zunanji uporabnik naveden v skrbniškem središču za Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="37319-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="37319-107">Prepričajte se, da je za spletno mesto vklopljena zunanja skupna raba.</span><span class="sxs-lookup"><span data-stu-id="37319-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="37319-108">Za klasično zbirko mest:</span><span class="sxs-lookup"><span data-stu-id="37319-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="37319-109">V novem skrbniškem središču za SharePoint v levem podoknu kliknite **spletna mesta**.</span><span class="sxs-lookup"><span data-stu-id="37319-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="37319-110">Izberite mesto ali spletna mesta in na traku kliknite **Skupna raba**.</span><span class="sxs-lookup"><span data-stu-id="37319-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="37319-111">Za spletno mesto skupine, ki pripada skupini Microsoft 365 ali na spletnem mestu za komunikacijo:</span><span class="sxs-lookup"><span data-stu-id="37319-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="37319-112">Te nove vrste mest imajo enako nastavitev skupne rabe kot nastavitev za celotno organizacijo, razen če nastavitev za celotno organizacijo omogoča skupno rabo datotek s povezavami, ki ne zahtevajo vpisa.</span><span class="sxs-lookup"><span data-stu-id="37319-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="37319-113">V tem primeru spletna mesta omogočajo skupno rabo z novimi in obstoječimi zunanjimi Uporabniki, ki se vpišejo.</span><span class="sxs-lookup"><span data-stu-id="37319-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="37319-114">Če želite spremeniti nastavitev za določena mesta, uporabite novo skrbniško središče za SharePoint ali PowerShell.</span><span class="sxs-lookup"><span data-stu-id="37319-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="37319-115">[Več informacij](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="37319-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="37319-116">Nastavitev zunanje skupne rabe za katero koli spletno mesto je lahko bolj restriktivna kot nastavitev za celotno organizacijo, ne pa tudi bolj zahtevna kot nastavitev za celotno organizacijo.</span><span class="sxs-lookup"><span data-stu-id="37319-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

