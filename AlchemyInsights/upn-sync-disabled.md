---
title: UPN sync invalidi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532347"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="e9598-102">UPN sync invalidi</span><span class="sxs-lookup"><span data-stu-id="e9598-102">UPN sync disabled</span></span>

<span data-ttu-id="e9598-103">Če ste začeli omedlevičen v sinje AD pred 30 marec 2016, zaženite naslednje Azure AD PowerShell cmdlet omogočiti UPN mehko tekmo v organizaciji le:</span><span class="sxs-lookup"><span data-stu-id="e9598-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="e9598-104">**Set-MsolDirSyncFeature-značilnost EnableSoftMatchOnUpn-omogoči $True**</span><span class="sxs-lookup"><span data-stu-id="e9598-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="e9598-105">UPN mehko tekmo je samodejno vklopljeno za organizacije, ki se je začel sinhronizacijo Azure oglas na ali po 30 marec 2016.</span><span class="sxs-lookup"><span data-stu-id="e9598-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="e9598-106">Če želite izvedeti več o omogočanju mehko tekmo na UPN in drugih omedlevičen zunanja oblika, si oglejte [Azure AD povezavo sinhronizacijsko storitev funkcije](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="e9598-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

