---
title: Vprašanja o uporabi orodja za uvajanje Officea (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698074"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vprašanja o uporabi orodja za uvajanje Officea (ODT)

Prenesite orodje za uvajanje Officea iz [Microsoftovega centra za prenose](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Čez downloading pila, prost dostop svoja osebnost-izvor izvršljiv pila, kateri vsebovati urad razvitje orodje izvršljiv (setup. exe) ter a vzorec zunanja podoba pila (Configuration. xml).
  
 **Če želite izključiti ali odstraniti Microsoftove 365 aplikacije za izdelke podjetja iz odjemalskih računalnikov:**
  
Ko nameščate Microsoft 365 apps za podjetje, lahko izključite določene izdelke. To storite tako, da sledite navodilom za namestitev Officea z ODT, vendar vključite element ExcludeApp v konfiguracijsko datoteko. Ta konfiguracijska datoteka na primer namesti vse Microsoftove 365 aplikacije za izdelke podjetja, razen Publisherja:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled orodja za uvajanje Officea](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

