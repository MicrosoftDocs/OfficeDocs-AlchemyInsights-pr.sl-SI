---
title: Elementov v SharePointu ali OneDrive ni mogoče izbrisati
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019599"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="925a5-102">Elementov ni mogoče izbrisati</span><span class="sxs-lookup"><span data-stu-id="925a5-102">Unable to delete items</span></span>

- <span data-ttu-id="925a5-103">Pravilniki o hranjenju lahko povzročijo to težavo, vendar morate onemogočiti ali izključiti ustrezno zadržanje, ki povzroča to težave.</span><span class="sxs-lookup"><span data-stu-id="925a5-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="925a5-104">Ko je pravilnik o hranjenju ali zadržanje odstranjen, lahko traja do 24 ur, da začne veljati sprememba.</span><span class="sxs-lookup"><span data-stu-id="925a5-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="925a5-105">Zagotovite, da v elementu ni nastavljene nastavitve [pravilnika o hranjenju](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) .</span><span class="sxs-lookup"><span data-stu-id="925a5-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="925a5-106">Mesto je morda preseglo omejitev shrambe, povečanje [količinske omejitve mesta](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) in brisanje elementa.</span><span class="sxs-lookup"><span data-stu-id="925a5-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="925a5-107">Zagotovite, da element ni [rezerviran](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) za drugega uporabnika.</span><span class="sxs-lookup"><span data-stu-id="925a5-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="925a5-108">Na koncu lahko skrbniki uporabljajo [SharePointove vzorce in prakse](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), ki vsebuje knjižnico ukazov PowerShell, ki omogočajo izvajanje zapletenih dejanj upravljanja, kot je na primer Vsiljevanje brisanja trmastih elementov.</span><span class="sxs-lookup"><span data-stu-id="925a5-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="925a5-109">Odstranjevanje datoteke PNP</span><span class="sxs-lookup"><span data-stu-id="925a5-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="925a5-110">Odstranjevanje mape PNP</span><span class="sxs-lookup"><span data-stu-id="925a5-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="925a5-111">Odstranjevanje elementa seznama PNP</span><span class="sxs-lookup"><span data-stu-id="925a5-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="925a5-112">Odstranjevanje seznama PNP</span><span class="sxs-lookup"><span data-stu-id="925a5-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="925a5-113">Odstranjevanje polja PNP (stolpec)</span><span class="sxs-lookup"><span data-stu-id="925a5-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)