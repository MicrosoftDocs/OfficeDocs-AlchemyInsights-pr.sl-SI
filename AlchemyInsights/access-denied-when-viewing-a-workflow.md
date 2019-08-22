---
title: Postranski tajivec čas sanjarstvo potek dela
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495839"
---
# <a name="access-denied-when-viewing-a-workflow"></a><span data-ttu-id="55585-102">Postranski tajivec čas sanjarstvo potek dela</span><span class="sxs-lookup"><span data-stu-id="55585-102">Access denied when viewing a Workflow</span></span>

<span data-ttu-id="55585-103">SharePoint 2013 poteki dela, ki poskušajo poslati email skupino SharePoint lahko ne zadostovati s "Postranski tajivec" zmota vest če članstvo skupine SharePoint ne vsem.</span><span class="sxs-lookup"><span data-stu-id="55585-103">SharePoint 2013 Workflows that attempt to send an email to a SharePoint group can fail with an "Access Denied" error message if the membership of the SharePoint group is not set to Everyone.</span></span>
  
 <span data-ttu-id="55585-104">**Če želite odpraviti težavo, naredite te korake:**</span><span class="sxs-lookup"><span data-stu-id="55585-104">**To resolve this issue, do these steps:**</span></span>
  
 1. <span data-ttu-id="55585-105">Omogočajo vsi ogled članov skupine SharePoint.</span><span class="sxs-lookup"><span data-stu-id="55585-105">Allow everybody to see the members of the SharePoint group.</span></span>
  
 2. <span data-ttu-id="55585-106">Skupine SharePoint odstranite za ali Kp črta email.</span><span class="sxs-lookup"><span data-stu-id="55585-106">Remove the SharePoint group from the To or CC line of the email.</span></span>
  
 3. <span data-ttu-id="55585-107">Izrecno dodati uporabnike za ali Kp če članstvo vidljivost ni mogoče spremeniti za SharePointovo skupino.</span><span class="sxs-lookup"><span data-stu-id="55585-107">Explicitly add the users to the To or CC line if the membership visibility cannot be changed for SharePoint group.</span></span>
  
<span data-ttu-id="55585-108">Če si želite ogledati več podrobnosti si oglejte [HTTP nepooblaščeno za /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="55585-108">To view more details please refer to [HTTP Unauthorized to /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).</span></span>
  