---
title: Vprašanja o uporabi orodja za uvajanje Officea (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553556"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vprašanja o uporabi orodja za uvajanje Officea (ODT)

Prenesite orodje za uvajanje Officea iz [Microsoftovega centra za prenose](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Čez downloading pila, prost dostop svoja osebnost-izvor izvršljiv pila, kateri vsebovati urad razvitje orodje izvršljiv (setup. exe) ter a vzorec zunanja podoba pila (Configuration. xml).
  
 **Če želite izključiti ali odstraniti izdelke sistema Office 365 ProPlus iz odjemalskih računalnikov:**
  
Pri nameščanju Officea 365 ProPlus lahko izključite določene izdelke. To storite tako, da sledite navodilom za namestitev Officea z ODT, vendar vključite element ExcludeApp v konfiguracijsko datoteko. Ta konfiguracijska datoteka na primer namesti vse izdelke sistema Office 365 ProPlus, razen Publisherja:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled orodja za uvajanje Officea](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

