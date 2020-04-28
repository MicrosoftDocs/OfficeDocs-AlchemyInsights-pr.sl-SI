---
title: Šifriranje s pravili prenosa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915289"
---
# <a name="encryption-with-transport-rules"></a>Šifriranje s pravili prenosa

V [skrbniškem središču za Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) lahko uporabite zmogljivosti šifriranja sporočil v Officeu (OME) v pravilih o toku pošte za proženje šifriranja sporočil. V pogoju pravila prenosa izberite možnost **Uporabite šifriranje sporočil v storitvi Office 365 in zaščito pravic**.

- Več informacij najdete v razdelku [Določite pravilo toka pošte za šifriranje](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- V storitvi Powershell uporabite pripomoček »cmdlet« [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) in vrednost parametra *ApplyOME* nastavite na $true.
