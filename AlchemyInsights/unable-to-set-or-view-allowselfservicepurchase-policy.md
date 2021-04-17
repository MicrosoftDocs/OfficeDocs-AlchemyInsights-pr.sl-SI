---
title: Ni mogoče nastaviti ali si ogledati pravilnika AllowServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826107"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="b6f5c-102">Ni mogoče nastaviti ali si ogledati pravilnika AllowServicePurchase</span><span class="sxs-lookup"><span data-stu-id="b6f5c-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="b6f5c-103">Pri poskusu nastaviti ali si ogledati pravilnik o nakupu AllowServicePurchase se prikaže to sporočilo o napaki:</span><span class="sxs-lookup"><span data-stu-id="b6f5c-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="b6f5c-104">*HandleError : Pravilnika o izdelku ni bilo mogoče pridobiti s Pravilnikid 'Allow NarHriServicePurchase', ErrorMessage – temeljna povezava je bila zaprta: Pri pošiljanju je prišlo do nepričakovane napake.*</span><span class="sxs-lookup"><span data-stu-id="b6f5c-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="b6f5c-105">Do tega lahko pride zaradi starejše različice programa Transport Layer Security (TLS).</span><span class="sxs-lookup"><span data-stu-id="b6f5c-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="b6f5c-106">Če želite povezati storitev MSCommerce, morate uporabiti TLS 1.2 ali več.</span><span class="sxs-lookup"><span data-stu-id="b6f5c-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="b6f5c-107">Če želite omogočiti/nastaviti protokol TLS na 1.2, ga preveriti in znova izvesti, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="b6f5c-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="b6f5c-108">V ukazni poziv lupine PowerShell (PS C: vnesite ta ukaz, če želite \) nastaviti protokol TLS na različico 1.2:</span><span class="sxs-lookup"><span data-stu-id="b6f5c-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="b6f5c-109">Preverite protokole TLS v uporabi s tem ukazom:</span><span class="sxs-lookup"><span data-stu-id="b6f5c-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="b6f5c-110">Po potrebi poskusite znova izvesti ukaze »Dobi« ali »Posodobi«.</span><span class="sxs-lookup"><span data-stu-id="b6f5c-110">Retry the Get or Update commands as needed.</span></span>

