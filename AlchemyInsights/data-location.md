---
title: Lokacija podatkov
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655298"
---
# <a name="data-location"></a><span data-ttu-id="4f946-102">Lokacija podatkov</span><span class="sxs-lookup"><span data-stu-id="4f946-102">Data location</span></span>

<span data-ttu-id="4f946-103">Lokacijo svojega najemnika si lahko ogledate v skrbniškem središču ali pa s povezavo na Exchange Online prek lupine PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4f946-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="4f946-104">**Skrbniško središče:**</span><span class="sxs-lookup"><span data-stu-id="4f946-104">**Admin center:**</span></span>
1. <span data-ttu-id="4f946-105">Prijavite se v [skrbniško središče](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="4f946-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="4f946-106">Izberite **Nastavitve** > **organizacije profil**.</span><span class="sxs-lookup"><span data-stu-id="4f946-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="4f946-107">Pod **lokacijo podatkov**izberite **Ogled podrobnosti**.</span><span class="sxs-lookup"><span data-stu-id="4f946-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="4f946-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="4f946-108">**PowerShell:**</span></span>
1. <span data-ttu-id="4f946-109">Z lupino Windows PowerShell vzpostavite povezavo s storitvijo Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="4f946-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="4f946-110">Izvršiti [zaslužiti-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet razpoložiti a zapisati v seznam od vaš najemnik ' premožen.</span><span class="sxs-lookup"><span data-stu-id="4f946-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="4f946-111">Poglejte lastnost OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="4f946-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="4f946-112">Ko imate podatkovno lokacijo za EXO in SPO, lahko določite lokacijo podatkov za druge storitve, ki jih lahko uporabljate od koder se [nahajajo vaši podatki](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="4f946-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>