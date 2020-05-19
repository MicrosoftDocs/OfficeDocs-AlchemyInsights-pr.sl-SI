---
title: Spreminjanje e-poštnega naslova skupine Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283261"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Spreminjanje e-poštnega naslova skupine Microsoft 365

E-poštni naslov skupine Microsoft 365 lahko spremenite s skrbniškim središčem. Samo izberite skupino in izberite @edit e-poštni naslov.

Če želite spremeniti primarni naslov SMTP skupine Microsoft 365, lahko uporabite tudi naslednje ukaze EXO PowerShell:

Set-UnifiedGroup <Group Name> -PrimarySMTPAddress<new SMTP Address>

Primer:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
