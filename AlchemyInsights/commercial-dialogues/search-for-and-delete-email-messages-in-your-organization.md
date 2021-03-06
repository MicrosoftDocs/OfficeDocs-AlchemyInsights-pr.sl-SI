---
title: Iskanje in brisanje e-poštnih sporočil v organizaciji
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750017"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>Iskanje in brisanje e-poštnih sporočil v organizaciji

Upoštevajte te korake:

1. Če niste globalni skrbnik, morate poiskati sporočila, ki jih mora vaš račun dodati v **skupino vlog E-odkrivanje Manager** ali **upravljanje iskanja skladnosti**. Če želite izbrisati sporočila, se morate vključiti v **skupino vlog za upravljanje organizacije** ali **vlogo za upravljanje iskanja in čiščenja**. Dovoljenja za te vloge so dodeljena v [središču za skladnost varnostnega &.](https://protection.office.com)
2. [Ustvarite iskanje vsebine](https://docs.microsoft.com/office365/securitycompliance/content-search) , da poiščete sporočilo, ki ga želite izbrisati.
3. [Vzpostavi povezavo z varnostnim središčem v središču za skladnost z varnostjo &](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). Če uporabljate MFA, si oglejte ta navodila: [Povežite se s središčem za varnost & skladnost z uporabo multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
4. Izbrišite sporočilo: zaženite `New-ComplianceSearchAction` ukaz» cmdlet «, da izbrišete sporočilo. Izbrisana sporočila so premaknjena v mapo» nadomestljive elemente uporabnika «. Če želite ukaz» primer «, glejte [3. korak: izbrišite sporočilo.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
