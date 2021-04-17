---
title: Spreminjanje zahteve za krepka gesla
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818484"
---
# <a name="change-strong-password-requirement"></a>Spreminjanje zahteve za krepka gesla

Microsoft privzeto zahteva močna gesla.

S storitvijo PowerShell lahko onemogočite močna gesla za določene uporabnike s temi ukazi:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Če želite onemogočiti močna gesla za vse uporabnike, uporabite:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Več informacij o pravilniku za gesla](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Vzpostavljanje povezave s storitvijo Microsoft 365 z lupino PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Več informacij o ukazih MsolUser v lupini PowerShell](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
