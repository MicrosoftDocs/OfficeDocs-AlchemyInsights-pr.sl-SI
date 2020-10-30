---
title: Spreminjanje zahteve za zapleteno geslo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804439"
---
# <a name="change-strong-password-requirement"></a>Spreminjanje zahteve za zapleteno geslo

Microsoft privzeto zahteva zapletena gesla.

Z uporabo lupine PowerShell lahko onemogočite močna gesla za določene uporabnike s temi ukazi:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Če želite onemogočiti močna gesla za vse uporabnike, uporabite:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Več informacij o pravilniku za gesla](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Vzpostavljanje povezave s storitvijo Microsoft 365 z lupino PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Več informacij o ukazih lupine PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
