---
title: Samodejno šifriranje e-poštnih sporočil v storitvi Office 365, poslanih določenim domenam
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749300"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="b3ffa-102">Samodejno šifriranje e-poštnih sporočil v storitvi Office 365, poslanih določenim domenam</span><span class="sxs-lookup"><span data-stu-id="b3ffa-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="b3ffa-103">V [skrbniškem središču za Exchange](https://outlook.office365.com/ecp/)izberite **pravila toka pošte >**.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="b3ffa-104">Kliknite ikono **novo (+)** , nato pa kliknite **uporabi šifriranje sporočil sistema Office 365 in zaščito pravic za sporočila**.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="b3ffa-105">V polje **ime** vnesite ime za pravilo, na primer *šifriranje sporočil, poslanih v contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="b3ffa-106">**Če želite uporabiti to pravilo, če** izberite **domeno prejemnika >**.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="b3ffa-107">Vnesite ime domene, na primer **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="b3ffa-108">Kliknite ikono **Dodaj (+)** in nato kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="b3ffa-109">Poleg polja **naredi to** kliknite **Izberi eno**.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="b3ffa-110">V spustnem meniju **predloga RMS** izberite **Šifriraj** in nato kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="b3ffa-111">(Če ne vidite te možnosti, to pomeni, da vaš paket ne vključuje samodejnega šifriranja.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="b3ffa-112">Vendar ga lahko dodate!)</span><span class="sxs-lookup"><span data-stu-id="b3ffa-112">But you can add it!)</span></span>
9. <span data-ttu-id="b3ffa-113">Izberite poljuben izbirni izbor (na seznamu izbirnih izbir, ki jih lahko naredite na tej strani, od katerih jih je mogoče preprostiti s privzeto nastavitev za enostavnost).</span><span class="sxs-lookup"><span data-stu-id="b3ffa-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="b3ffa-114">Kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b3ffa-115">Pozneje se lahko vrnete in uredite to pravilo.</span><span class="sxs-lookup"><span data-stu-id="b3ffa-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="b3ffa-116">Če želite več informacij o ustvarjanju pravil za šifriranje, glejte [določanje pravil pretoka pošte za šifriranje e-poštnih sporočil v storitvi Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="b3ffa-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>