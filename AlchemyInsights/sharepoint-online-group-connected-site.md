---
title: Dodajanje skupine na SharePointovo mesto
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771224"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Težave pri ustvarjanju spletnega mesta, ki je povezano s skupino v SharePointu

1. Nekaj pogostih težav, ki so se pojavile pri ustvarjanju ali vnovičnem ustvarjanju skupine, ki je povezano na mestu.
Če ste izbrisali skupino in njeno povezano mesto in želite ustvariti drugo mesto z istim URL-jem, boste morali trajno odstraniti prejšnje mesto.

   - Prenesite [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Če želite več informacij o tem, kako začeti uporabljati PowerShell, glejte uvod [v storitev SharePoint online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Odstranite mesto iz izbrisanih mest z ukazom» cmdlet « [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell. PowerShell je zahtevan za trajno brisanje mest skupine.

1. Če ustvarjate spletno mesto skupine in prejmete opozorilo: **druga skupina z istim vzdevkom že obstaja**, preverite obstoječe skupine v [skrbniškem središču za Microsoft 365](https://admin.microsoft.com/AdminPortal/Home#/groups). Če želite odpraviti težavo, izbrišite obstoječo skupino, če ni več potrebna ali ustvarite mesto z drugim dodeljenim vzdevkom.

1. V SharePointu lahko ustvarite in uporabljate različne načine za ustvarjanje in uporabo sodobnih skupin.

   - Obstoječa mesta lahko povežete s skupino Microsoft 365. Če želite več informacij, glejte [povezovanje skupine Microsoft 365 s SharePointovim uporabniškim vmesnikom](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Če želite ustvariti spletno mesto, ki je povezano s skupino Microsoft 365, morate ustvariti [spletno mesto skupine](https://admin.microsoft.com/sharepoint).
