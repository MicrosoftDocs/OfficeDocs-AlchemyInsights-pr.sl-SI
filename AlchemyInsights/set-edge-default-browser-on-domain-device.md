---
title: Nastavitev brskalnika Microsoft Edge kot privzetega brskalnika v napravi, pridruženi domeni
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491878"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="e975e-102">Nastavitev brskalnika Microsoft Edge kot privzetega brskalnika v napravi, pridruženi domeni</span><span class="sxs-lookup"><span data-stu-id="e975e-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="e975e-103">Nastavite Microsoft Edge kot privzeti brskalnik:</span><span class="sxs-lookup"><span data-stu-id="e975e-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="e975e-104">[Ustvarite privzeto konfiguracijsko datoteko s povezavami](https://go.microsoft.com/fwlink/?linkid=2132437) in jo shranite lokalno ali v omrežni pogon.</span><span class="sxs-lookup"><span data-stu-id="e975e-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="e975e-105">Odprite urejevalnik pravilnika skupine in pojdite v Raziskovalca **za** komponente datoteke s komponentami sistema Windows za konfiguracijo  >    >    >  **računalnika.**</span><span class="sxs-lookup"><span data-stu-id="e975e-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="e975e-106">Izberite **Nastavitev privzete konfiguracijske datoteke s povezavami.**</span><span class="sxs-lookup"><span data-stu-id="e975e-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="e975e-107">Izberite **Nastavitev pravilnika** in nato **Omogočeno.**</span><span class="sxs-lookup"><span data-stu-id="e975e-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="e975e-108">V **razdelku** Možnosti vnesite mesto privzete konfiguracijske datoteke s povezavami in izberite V **redu.**</span><span class="sxs-lookup"><span data-stu-id="e975e-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
