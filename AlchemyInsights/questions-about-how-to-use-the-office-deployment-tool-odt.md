---
title: Vprašanja o tem, kako uporabljati orodje za uvajanje Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29490141"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Vprašanja o tem, kako uporabljati orodje za uvajanje Office (ODT)

Urad razvitje orodje prenesete iz [Microsoftovega centra za prenose](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Po prenosu datoteke, zaženite samo pridobivanja izvedljivo datoteko, ki vsebuje Office razvitje orodje izvršljiv (setup.exe) in vzorec konfiguracijske datoteke (configuration.xml).
  
 **Izključiti ali odstraniti Office 365 ProPlus izdelkov iz odjemalske računalnike:**
  
Ko namestite Office 365 ProPlus, izključite lahko določene izdelke. To storite tako, sledite korakom za namestitev Office z na ODT, vendar vsebuje ExcludeApp elementa v konfiguracijski datoteki. Na primer, te konfiguracijske datoteke namesti vse Office 365 ProPlus proizvodov razen založnik:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled orodja za uvajanje urad](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

