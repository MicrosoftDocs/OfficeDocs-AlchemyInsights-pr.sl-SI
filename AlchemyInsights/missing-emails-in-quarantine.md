---
title: Manjkajoča e-poštna sporočila v karanteni
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
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539840"
---
# <a name="missing-emails-in-quarantine"></a>Manjkajoča e-poštna sporočila v karanteni«

Skrbniki si lahko [ogledajo ta sporočila, jih izdajajo ali izbrišejo.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Če želite odpreti Središče & za skladnost s predpisi, odprite [https://protection.office.com](https://protection.office.com/) . Če želite stran Karantena odpreti neposredno, odprite [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Iščete lahko po teh vrednostih:  

- **ID sporočila:** globalni enolični identifikator sporočila. Če na seznamu izberete sporočilo, se vrednost  **ID-ja**  sporočila prikaže v  **prikazanem podoknu**  s podrobnostmi. Skrbniki lahko s funkcijo [sledenja sporočilu](/microsoft-365/security/office-365-security/message-trace-scc) poiščejo sporočila in ustrezne vrednosti ID-ja sporočila.
- **E-poštni naslov pošiljatelja:** e-poštni naslov enega pošiljatelja.
- **E-poštni naslov** prejemnika: e-poštni naslov enega prejemnika.
- **Zadeva:** uporabite celotno zadevo sporočila. Iskanje ne uporablja velikih in malih črk.

Ko vnesete pogoje iskanja, kliknite Osveži gumb ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Osveži, da** filtrirate rezultate.

Ukazi »cmdlet« za ogled in upravljanje sporočil in datotek v karanteni so:
- [Brisanje-karantenamessage](/powershell/module/exchange/delete-quarantinemessage)
- [Izvoz v karanteno](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Predogled in pošiljanje sporočil v karanteni:](/powershell/module/exchange/preview-quarantinemessage)ta ukaz »cmdlet« je le za sporočila in ne za datoteke z zlonamerno programsko opremo iz programa Microsoft Defender za Office 365 za SharePoint Online, OneDrive za podjetja ali Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)