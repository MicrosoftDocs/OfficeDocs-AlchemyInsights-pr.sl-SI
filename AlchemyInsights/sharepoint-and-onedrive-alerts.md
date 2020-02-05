---
title: Zamude pri prejemanju opozoril za SharePoint in OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771231"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="90c23-102">Zamude pri prejemanju opozoril za SharePoint in OneDrive</span><span class="sxs-lookup"><span data-stu-id="90c23-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="90c23-103">Najprej preverite mapo junk ali spam v e-poštnem sporočilu.</span><span class="sxs-lookup"><span data-stu-id="90c23-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="90c23-104">Če **so vsa opozorila iz več datotek ali knjižnic zapoznela**, obiščite [nadzorno ploščo storitve Health](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) , da preverite morebitne advisorije/incidente, ki se lahko zgodijo s SharePointom ali Exchangeem.</span><span class="sxs-lookup"><span data-stu-id="90c23-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="90c23-105">Težava je lahko s SharePointovo možnostjo opozarjanja ali zakasnitvami v e-poštnih sporočilih prek Exchangeevega.</span><span class="sxs-lookup"><span data-stu-id="90c23-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="90c23-106">Upoštevajte tudi, ali se dostavi druga e-pošta-če ne, vprašanje je verjetno z zamudami Exchange.</span><span class="sxs-lookup"><span data-stu-id="90c23-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="90c23-107">Če **posamezno opozorilo iz določene datoteke ali knjižnice ni podano**, ga poskusite izbrisati in znova ustvariti.</span><span class="sxs-lookup"><span data-stu-id="90c23-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="90c23-108">Če želite znova ustvariti opozorilo, glejte [upravljanje, ogled ali brisanje SharePointovih opozoril](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) .</span><span class="sxs-lookup"><span data-stu-id="90c23-108">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="90c23-109">Opozoril ni mogoče poslati v distribucijsko skupino.</span><span class="sxs-lookup"><span data-stu-id="90c23-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="90c23-110">Podprte so samo skupine za varnost in O365.</span><span class="sxs-lookup"><span data-stu-id="90c23-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="90c23-111">Predloge za e-poštno sporočilo z opozorili ni mogoče prilagoditi.</span><span class="sxs-lookup"><span data-stu-id="90c23-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="90c23-112">Če želite doseči te cilje, morate uporabiti Microsoft Flow ali potek dela programa SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="90c23-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
