---
title: Odpravljanje težav z varnostnim namiga za preverjanje zaznavanja goljufij
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759528"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="6f2b3-102">Odpravljanje težav z varnostnim namiga za preverjanje zaznavanja goljufij</span><span class="sxs-lookup"><span data-stu-id="6f2b3-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="6f2b3-103">Če vi ste pridobivanje a varnost odlagališče to pravi "oddajnik ne zadostovati svoj goljufija odkritje ček ter maj ne obstati kdo oni pokazati se v obstati", torej oddajnik ne zadostovati v prelaz vsak izmed obeh DKIM ali SPF Authentication ček.</span><span class="sxs-lookup"><span data-stu-id="6f2b3-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="6f2b3-104">Najboljši način za rešitev tega je, da se pošiljatelj pooblasti.</span><span class="sxs-lookup"><span data-stu-id="6f2b3-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="6f2b3-105">Če pošiljatelj pošilja v vašem imenu, ga morate odobriti tako, da dodate pošiljateljevo IP-naslov v zapis SPF.</span><span class="sxs-lookup"><span data-stu-id="6f2b3-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="6f2b3-106">Če želite več informacij, glejte [Odpravljanje težav z rdečo (sumljivo) varnostno konico za preverjanje goljufij](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="6f2b3-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="6f2b3-107">Tukaj je nekaj drugih povezav, ki lahko pomagajo:</span><span class="sxs-lookup"><span data-stu-id="6f2b3-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="6f2b3-108">Kako Microsoft uporablja okvir pravilnika pošiljatelja (SPF) za preprečevanje prevara</span><span class="sxs-lookup"><span data-stu-id="6f2b3-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="6f2b3-109">Nastavite SPF za pomoč pri preprečevanju prevara</span><span class="sxs-lookup"><span data-stu-id="6f2b3-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
