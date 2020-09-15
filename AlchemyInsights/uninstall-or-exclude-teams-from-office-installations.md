---
title: Odstranjevanje ali izključevanje ekip iz Officeovih instalacij
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658237"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="33c63-102">Odstranjevanje ali izključevanje ekip iz novih ali obstoječih Officeovih namestitev</span><span class="sxs-lookup"><span data-stu-id="33c63-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="33c63-103">Microsoft Teams je vključen kot del programa Microsoft 365 apps za podjetja, Microsoft 365 apps za podjetja in Office za Mac.</span><span class="sxs-lookup"><span data-stu-id="33c63-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="33c63-104">Uporabite [orodje za uvajanje Officea](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , da izključite ekipe iz novih namestitev Officea.</span><span class="sxs-lookup"><span data-stu-id="33c63-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="33c63-105">Če želite *odstraniti* ekipe iz naprave, v kateri se izvaja Windows, glejte [odstranitev aplikacije Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="33c63-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="33c63-106">Če želite počistiti Microsoft Teams iz več ciljnih strojev ali uporabnikov, si oglejte [uvajanje storitve Microsoft Teams Clean Up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="33c63-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="33c63-107">Uporabite možnost [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) , če želite preprečiti, da bi Microsoft Teams samodejno nameščal Office.</span><span class="sxs-lookup"><span data-stu-id="33c63-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="33c63-108">Uporabite možnost [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *preden je ekipa nameščena*, da se Microsoft Teams ne zažene samodejno po namestitvi.</span><span class="sxs-lookup"><span data-stu-id="33c63-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="33c63-109">Če uporabljate Office za Mac, glejte [naprave Microsoft Teams v računalniku Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="33c63-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>