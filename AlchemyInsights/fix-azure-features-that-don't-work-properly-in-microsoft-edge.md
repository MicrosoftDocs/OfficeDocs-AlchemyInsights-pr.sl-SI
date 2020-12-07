---
title: Kaj storiti, če funkcije Azure ne delujejo pravilno v brskalniku Microsoft Edge
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583782"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="81df7-102">Kaj storiti, če funkcije Azure ne delujejo pravilno v brskalniku Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="81df7-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="81df7-103">Microsoft Edge ima [znane težave](https://go.microsoft.com/fwlink/?linkid=2140608) , ki so povezane z varnostnimi območji, in lahko vpliva na to, kako se uporabniki Azure prijavijo v skrbniško središče sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="81df7-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="81df7-104">Če imate težave z uporabo funkcij Azure s programom Microsoft Edge, poskusite s temi koraki:</span><span class="sxs-lookup"><span data-stu-id="81df7-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="81df7-105">V **začetnem** meniju poiščite **Internetne možnosti** in jo izberite.</span><span class="sxs-lookup"><span data-stu-id="81df7-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="81df7-106">V pogovornem oknu **internetne lastnosti** odprite zavihek **varnost** .</span><span class="sxs-lookup"><span data-stu-id="81df7-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="81df7-107">Izberite območje **zaupanja vredna mesta** in nato izberite gumb **mesta** .</span><span class="sxs-lookup"><span data-stu-id="81df7-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="81df7-108">V pogovornem oknu **zaupanja vredna mesta** dodajte URL prehoda [https://login.microsoftonline.com](https://login.microsoftonline.com) in in [https://login.live.com](https://login.live.com) nato izberite **Zapri**.</span><span class="sxs-lookup"><span data-stu-id="81df7-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="81df7-109">V pogovornem oknu **internetne lastnosti** pojdite na zavihek **zasebnost** .</span><span class="sxs-lookup"><span data-stu-id="81df7-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="81df7-110">V razdelku **Preprečevalnik pojavnih oken** izberite **Nastavitve**.</span><span class="sxs-lookup"><span data-stu-id="81df7-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="81df7-111">V pogovornem oknu, ki se odpre, dodajte URL prehoda, kot tudi [https://login.microsoftonline.com](https://login.microsoftonline.com) in in [https://login.live.com](https://login.live.com) nato izberite **Zapri**.</span><span class="sxs-lookup"><span data-stu-id="81df7-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
