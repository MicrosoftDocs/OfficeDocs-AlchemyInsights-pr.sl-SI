---
title: Iskanje vsebine ni rezultat
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680663"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="b36ae-102">Ni rezultatov iskanja/izvoza vsebine</span><span class="sxs-lookup"><span data-stu-id="b36ae-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="b36ae-103">Težave z iskanjem/izvozom vsebine ne vračajo nobenih podatkov je morda zaradi določenega filtra varnosti skladnosti, ki ga je nastavil določen skrbnik in ga ni mogoče sporočiti vsem skrbnikom.</span><span class="sxs-lookup"><span data-stu-id="b36ae-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="b36ae-104">To težavo odpravite tako, da preverite, ali obstajajo filtri varnosti skladnosti, ki jih lahko povzroči to:</span><span class="sxs-lookup"><span data-stu-id="b36ae-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="b36ae-105">Vzpostavljanje povezave z lupino PowerShell za varnost in skladnost s predpisi</span><span class="sxs-lookup"><span data-stu-id="b36ae-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="b36ae-106">Zaženite ta ukazov:</span><span class="sxs-lookup"><span data-stu-id="b36ae-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="b36ae-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="b36ae-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="b36ae-108">Get-ComplianceSecurityFilter-organizacija $org</span><span class="sxs-lookup"><span data-stu-id="b36ae-108">Get-ComplianceSecurityFilter -Organization $org</span></span>