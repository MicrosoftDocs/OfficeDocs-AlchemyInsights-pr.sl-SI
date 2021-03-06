---
title: Micro zamude ali omejevanje storitve PowerShell v storitvi Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702142"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Micro zamude ali omejevanje storitve PowerShell v storitvi Exchange Online

Ko zaženete skripte in ukaze »cmdlet« v storitvi Exchange Online, boste morda opazili opozorila »Micro delay applied«. Tukaj je nekaj predlogov, kako odpraviti to težavo:

- Zaženite diagnostiko, da sprostite najemnika pravilnike o zmogljivosti zmogljivosti PowerShell. S to rešitvijo boste težavo večino rešili.
- Če težave še vedno ne odpravite, uporabite modul [Exchange Online v2 PowerShell,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)ki vključuje ukaze CMDlet, ki temeljijo na vmesniku API REST in so znatno bolj učinkovitejši. To je lahko odlična rešitev za veliko število ukazov» dobi «, ki se pogosto uporabljajo.
- Če morate uporabiti ukaze CMDlet, ki niso zajeti v modulu v2, glejte Zagon ukazov [»cmdlet«](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)lupine PowerShell za večje število uporabnikov v programu Office 365, ki govori o tem, kako se lahko v modulu PowerShell omejijo omejevanje zmogljivosti v Exchange Online.
