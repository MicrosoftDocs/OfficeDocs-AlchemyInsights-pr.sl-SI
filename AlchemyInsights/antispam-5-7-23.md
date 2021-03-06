---
title: Antispam - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821427"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Odpravljanje težav za dostavo e-pošte za kodo napake 5.7.23

Preverite zapis DNS SPF za svojo domeno pri javno dostopnem SPF-ju ali v spletnem preverjanje zapisov DNS.

Prepričajte se, da Microsoft ni identificiral odhodnega sporočila kot neželeno pošto in da je bilo preusmerjeno prek skupine dostav [z visokim tveganjem.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages) Sporočila v poolu za dostavo z visokim tveganjem ne bodo uspešno sprejeta preverjanja SPF, zato ciljna e-poštna organizacija ne bo sprejela.

Če težave ne morete odpraviti, se boste morda morali obrnite na skrbnika gostitelja pošte, kateremu poskušate poslati e-pošto. V sporočilu o odklonu si zabeležite podrobno zunanjo napako. Microsoftova podpora morda ne bo mogla dodatno pomagati.
