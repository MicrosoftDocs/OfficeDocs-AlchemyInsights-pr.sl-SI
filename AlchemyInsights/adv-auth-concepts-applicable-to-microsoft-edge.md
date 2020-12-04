---
title: Dodatni koncepti preverjanja pristnosti, ki veljajo za Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573777"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="0f1ac-102">Dodatni koncepti preverjanja pristnosti, ki veljajo za Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="0f1ac-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="0f1ac-103">V nadaljevanju so opisani napredni koncepti preverjanja pristnosti, ki veljajo za Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="0f1ac-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="0f1ac-104">**Proaktivno preverjanje pristnosti**</span><span class="sxs-lookup"><span data-stu-id="0f1ac-104">**Proactive Authentication**</span></span>

<span data-ttu-id="0f1ac-105">Ko omogočite pravilnik o [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , bo Microsoft Edge poskušal proaktivno preveriti pristnost prijavljenih uporabnikov prek Microsoftovih storitev.</span><span class="sxs-lookup"><span data-stu-id="0f1ac-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="0f1ac-106">V rednih časovnih presledkih bo uporaba spletne storitve za preverjanje posodobljenega manifesta, ki vsebuje konfiguracijo, ki ureja proaktivno preverjanje pristnosti.</span><span class="sxs-lookup"><span data-stu-id="0f1ac-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="0f1ac-107">Prednosti: proaktivno preverjanje pristnosti omogoča preverjanje pristnosti za ključne storitve, kot je na primer stran» Office New zavihek «.</span><span class="sxs-lookup"><span data-stu-id="0f1ac-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="0f1ac-108">Če se Bing uporablja kot iskalnik, proaktivno preverjanje pristnosti izboljša učinkovitost naslovne vrstice in pomaga pri ustvarjanju rezultatov iskanja prilagojenih potrebam vašega podjetja.</span><span class="sxs-lookup"><span data-stu-id="0f1ac-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="0f1ac-109">**Windows hello CredUI za preverjanje pristnosti NTLM**</span><span class="sxs-lookup"><span data-stu-id="0f1ac-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="0f1ac-110">Če Enotna prijava (SSO) ni na voljo, ko spletno mesto poskuša podpisati uporabnika prek mehanizma NTLM ali pogajanja, bo ta funkcija uporabniku omogočila skupno rabo poverilnic OS s spletnim mestom in za zadovoljevanje preverjanja pristnosti z uporabniškim vmesnikom Windows hello verodostojnost.</span><span class="sxs-lookup"><span data-stu-id="0f1ac-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="0f1ac-111">Ta tok za vpis bo prikazan le v sistemu Windows 10 in le za uporabnike, ki ne prejmejo SSO med NTLM ali pogajalskim izzivom.</span><span class="sxs-lookup"><span data-stu-id="0f1ac-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="0f1ac-112">**Uporaba shranjenih gesel za samodejno vpis**</span><span class="sxs-lookup"><span data-stu-id="0f1ac-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="0f1ac-113">Uporabniki, ki shranjujejo gesla v brskalniku Microsoft Edge, lahko omogočijo samodejno prijavo na spletna mesta, kjer imajo shranjene poverilnice.</span><span class="sxs-lookup"><span data-stu-id="0f1ac-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="0f1ac-114">Uporabniki lahko to funkcijo vklopijo ali izklopijo v edge://settings/passwords, vi pa jo lahko konfigurirate v pravilnikih [upravitelja gesel](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="0f1ac-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
