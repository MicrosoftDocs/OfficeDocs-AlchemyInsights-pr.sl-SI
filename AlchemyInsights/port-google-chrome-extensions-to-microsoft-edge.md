---
title: Vrata brskalnika Google Chrome na Microsoft Edge (krom)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678981"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>Vrata brskalnika Google Chrome na Microsoft Edge (krom)

[Do razširitve brskalnika Google Chrome lahko preprosto poženete v Microsoft Edge (krom)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension). V večini primerov so potrebni le najnujnejše spremembe za zagon teh razširitev na spletnem mestu Microsoft Edge.

Pripone API-jev in Manifestne tipke, ki jih podpira Google Chrome, so združljive s kodo Microsoft Edge. Vendar pa Microsoft Edge ne podpira razširitve API-jev Chrome. gcm, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken in Chrome. instanceID.