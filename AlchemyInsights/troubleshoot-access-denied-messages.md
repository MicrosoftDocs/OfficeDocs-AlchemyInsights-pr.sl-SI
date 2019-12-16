---
title: Odpravljanje težav s sporočili o zavrnitvi dostopa
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050721"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="7277c-102">Odpravljanje težav s sporočili o zavrnitvi dostopa</span><span class="sxs-lookup"><span data-stu-id="7277c-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="7277c-103">Če je nekdo dobil sporočilo» dostop zavrnjen «v mapo v skupni rabi v SharePointu, je skrbnik zbirke mest morda omogočil» omejen dostop uporabnika dovoljenje za zaklepanje «.</span><span class="sxs-lookup"><span data-stu-id="7277c-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="7277c-104">Če želite to izklopiti:</span><span class="sxs-lookup"><span data-stu-id="7277c-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="7277c-105">Prebrskajte do mesta, kliknite ikono nastavitve in nato kliknite **Nastavitve mesta**.</span><span class="sxs-lookup"><span data-stu-id="7277c-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="7277c-106">V razdelku **skrbništvo zbirke mest**kliknite **funkcije zbirke mest**.</span><span class="sxs-lookup"><span data-stu-id="7277c-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="7277c-107">Poleg **omejenega dostopa do dovoljenja za zaklepanje uporabnika**, kliknite **Deaktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="7277c-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="7277c-108">V mapah v skupni rabi se lahko pojavi tudi sporočilo za dostop zavrnjen, če je spletno mesto založništvo.</span><span class="sxs-lookup"><span data-stu-id="7277c-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="7277c-109">Če želite več informacij, glejte [dostop zavrnjen, ko dostopate do mape v skupni rabi](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="7277c-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="7277c-110">Če je pri poskusu vpogleda v zahteve za dostop nekdo dobil sporočilo» dostop zavrnjen «, mora uporabnik dodati bodisi skrbnika zbirke mest bodisi člana skupine lastnikov za spletno mesto.</span><span class="sxs-lookup"><span data-stu-id="7277c-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="7277c-111">Če želite več informacij, glejte [dostop zavrnjen na seznam zahtev za dostop](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="7277c-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="7277c-112">Če je uporabnik dobil sporočilo» zavrnjeno dostop «po tem, ko so bili odstranjeni iz imenika Active Directory na mestu uporabe in nato znova dodani, glejte [dostop zavrnjen, ko je uporabniški račun sinhroniziran z officeom 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="7277c-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

