---
title: Navodila za skrivanje/razkrivanje skupine s seznama naslovov
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768952"
---
# <a name="hide-office-365-group-from-address-list-gal"></a><span data-ttu-id="f0afe-102">Skrij Office 365 skupina iz seznama naslovov (GAL)</span><span class="sxs-lookup"><span data-stu-id="f0afe-102">Hide Office 365 group from address list (GAL)</span></span>

<span data-ttu-id="f0afe-103">Če želite skriti skupino Office 365 iz seznamov naslovov (GAL) odjemalcev Exchange (kot je Outlook ali OWA), uporabite ta ukaz v lupini EXO:</span><span class="sxs-lookup"><span data-stu-id="f0afe-103">To hide an Office 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="f0afe-104">Če želite skriti skupino Office 365, ki je vidna odjemalcem Exchange, uporabite ta ukaz v lupini EXO:</span><span class="sxs-lookup"><span data-stu-id="f0afe-104">To hide the Office 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`
