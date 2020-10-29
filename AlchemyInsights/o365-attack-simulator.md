---
title: 2681 simulator napada v Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801567"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="179e4-102">Simulator napada v programu Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="179e4-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="179e4-103">Ali zamujate simulator napada?</span><span class="sxs-lookup"><span data-stu-id="179e4-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="179e4-104">Simulator napada zahteva **Microsoft Defender za office 365 (paket ATP 2)** ali **Office 365 Enterprise E5** .</span><span class="sxs-lookup"><span data-stu-id="179e4-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5** .</span></span> <span data-ttu-id="179e4-105">Simulator napada ni **vključen v** Microsoft Defender za Office 365 (paket ATP 1), Office 365 Enterprise E3 ali kateri koli Microsoft 365 apps za naročnine na podjetja.</span><span class="sxs-lookup"><span data-stu-id="179e4-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="179e4-106">Z računom, ki ga uporabljate za zagon simuliranih napadov, potrebujete dovoljenja globalnega skrbnika ali varnostnega skrbnika in multi-Factor Authentication (MFA).</span><span class="sxs-lookup"><span data-stu-id="179e4-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="179e4-107">Če želite več informacij o zahtevah simulatorja napada, si oglejte [to temo](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="179e4-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="179e4-108">Pomembne stvari, ki jih morate vedeti o simulacijah **nasilnih napadov gesel** :</span><span class="sxs-lookup"><span data-stu-id="179e4-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="179e4-109">Če je v ciljnem računu omogočena funkcija MFA in je bilo geslo pravilno uganil, račun ne bo prikazan kot ogrožen (drugi faktor preverjanja pristnosti bo nepopoln).</span><span class="sxs-lookup"><span data-stu-id="179e4-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="179e4-110">Datoteka gesel ne more biti večja od 10 MB.</span><span class="sxs-lookup"><span data-stu-id="179e4-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="179e4-111">Uporabite eno geslo na vrstico in vključite prazno vrstico (vračanje) po zadnjem geslu na seznamu.</span><span class="sxs-lookup"><span data-stu-id="179e4-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="179e4-112">Pomembne stvari, ki jih morate vedeti o prilaganju simulacij s **kopjem** :</span><span class="sxs-lookup"><span data-stu-id="179e4-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="179e4-113">Po načrtu ne morete ponuditi vrednosti po meri za **spletni naslov strežnika za prijavo lažnega predstavljanja** .</span><span class="sxs-lookup"><span data-stu-id="179e4-113">By design, you can't provide a custom value for **Phishing login server URL** .</span></span>

  - <span data-ttu-id="179e4-114">Če prejemnik uporabi [dodatek» omogoči sporočilo za poročilo](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) «, da sporoči sporočilo kot lažno predstavljanje, morda ne boste prejeli opozoril za sporočilo (ker je to simulirani napad).</span><span class="sxs-lookup"><span data-stu-id="179e4-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="179e4-115">Poročila: ko je simulirani napad končan, lahko kliknete **podrobnosti napada** , da si ogledate poročilo.</span><span class="sxs-lookup"><span data-stu-id="179e4-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="179e4-116">Če želite podrobna navodila in nove funkcije v simulatorju napada, glejte [simulator napada v programu Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="179e4-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
