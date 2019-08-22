---
title: Vsebine ne rezultati iskanja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516795"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="5bbb1-102">Ni rezultatov iz vsebine iskanje/izvoz</span><span class="sxs-lookup"><span data-stu-id="5bbb1-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="5bbb1-103">Vprašanja z vsebino iskanje/izvoz ne vračajo podatkov je lahko posledica nekaterih skladnosti varnostnega filtra, da je bila namestitev posebnih Admin in ne komunicira vse administratorji.</span><span class="sxs-lookup"><span data-stu-id="5bbb1-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="5bbb1-104">Če želite to odpraviti, preverite, če obstajajo kakršne koli skladnosti varnostnih filtrov, ki lahko povzroča to:</span><span class="sxs-lookup"><span data-stu-id="5bbb1-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="5bbb1-105">Povezati varnost in skladnost Center Powershell</span><span class="sxs-lookup"><span data-stu-id="5bbb1-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="5bbb1-106">Zaženite naslednje commandlets:</span><span class="sxs-lookup"><span data-stu-id="5bbb1-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="5bbb1-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="5bbb1-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="5bbb1-108">Get-ComplianceSecurityFilter-organizacija $org</span><span class="sxs-lookup"><span data-stu-id="5bbb1-108">Get-ComplianceSecurityFilter -Organization $org</span></span>