---
title: Dovoljenja za koledar
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
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819924"
---
# <a name="calendar-permissions"></a>Dovoljenja za koledar

Uporabniki lahko spremenijo svoja dovoljenja za koledar z Outlookom v spletu ali z drugimi odjemalci, vendar boste kot skrbnik morda morali raziskati tudi sami.  
Z ukazom »cmdlet« lupine Exchange PowerShell boste videli dovoljenje za uporabnikov koledar:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Če želite več informacij, glejte:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Dovoljenja za koledar so uporabljena za skupno rabo koledarjev, za več informacij o skupni rabi Outlookovega koledarja pa si oglejte te članke:

- [Skupna raba koledarja programa Outlook z drugimi osebami](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Skupna raba koledarja v Outlooku v spletu za podjetja](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Če želite odpraviti težave z dovoljenjem koledarja, lahko uporabite [orodje Pomočnik za podporo in obnovitev.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)