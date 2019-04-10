---
title: E-poštnih sporočil premakniti arhivskega nabiralnika
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747219"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premakniti email arhivskega nabiralnika
 
1. Potrditev, da je bila omogočena **Arhiv nabiralnik** . V nasprotnem primeru, sledite korakom v [tem članku](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) za omogočanje arhivskega nabiralnika.

2. V arhiv sporočil samodejno arhivskega nabiralnika, oznako za hranjenje z dejanjem **Premakni v Arhiv** mora biti nastavljena na **samodejno dodati oznako celoten predal (privzeto)**. Sledite korakom tukaj ustvariti oznako: [Arhiv privzeto oznako](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).
    
3. Nato dodajte oznako **Arhiv** pravilnik o hranjenju. V skrbniškem središču za izmenjavo, izberite **Zadrževanja** > dodati, **premakniti za oznako Arhiv** politike >, **shranite**. 
    
4. Zdaj [dodelite pravilnik o hranjenju](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) posebne uporabnikovega nabiralnika. Istega pravilnika veljajo na **primarnega** in **arhivskega** nabiralnika. 
    
Je potrebno za vsiljevanje uspelo mapo pomočnika (MFA) teči ter uveljavil nove nastavitve uporabnikovega nabiralnika. Zaženite ta ukaz, medtem ko [povezati EKSO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) začeti pomočnik za upravljane mape za določen nabiralnik: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

Če želite več informacij o nastavljanju pravilnik arhiviranja, glejte [Nastavitev Arhiv in izbris pravilnika za nabiralnike](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  

