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
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010774"
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

[Pregled orodja za uvajanje Officea](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

