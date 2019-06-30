---
title: Varnost nasvet za odkrivanje goljufij za odpravljanje težav preveri
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353265"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="a799f-102">Varnost nasvet za odkrivanje goljufij za odpravljanje težav preveri</span><span class="sxs-lookup"><span data-stu-id="a799f-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="a799f-103">Če ste dobili varnosti tip, ki pravi "pošiljatelj ni naše preglede odkrivanje goljufij in ki se zdi, da ne sme biti", nato pa pošiljatelj ni prestal preverjanja pristnosti DKIM ali SPF.</span><span class="sxs-lookup"><span data-stu-id="a799f-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="a799f-104">Najboljši način za to rešitev je za pošiljatelja pooblastiti sami.</span><span class="sxs-lookup"><span data-stu-id="a799f-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="a799f-105">Če pošiljatelj pošilja v vašem imenu, morate dovoliti jih z dodajanjem pošiljatelja IP naslov za SPF zapis.</span><span class="sxs-lookup"><span data-stu-id="a799f-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="a799f-106">Za več informacij glej [rdeče (sumljivo) varnost nasvet za odkrivanje goljufij za odpravljanje težav preveri](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="a799f-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="a799f-107">Tukaj je nekaj povezav, ki lahko pomagajo:</span><span class="sxs-lookup"><span data-stu-id="a799f-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="a799f-108">Kako Office 365 uporablja oddajnik zvitost tramovje (SPF) za preprečevanje prevara</span><span class="sxs-lookup"><span data-stu-id="a799f-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="a799f-109">Nastavite v Office 365 SPF pomagate preprečiti lažno predstavljanje</span><span class="sxs-lookup"><span data-stu-id="a799f-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
