---
title: Samodejno šifriranje določenih e-poštnih sporočil v storitvi Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526764"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="56992-102">Samodejno šifriranje določenih e-poštnih sporočil v storitvi Office 365</span><span class="sxs-lookup"><span data-stu-id="56992-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="56992-103">V [skrbniškem središču za Exchange](https://outlook.office365.com/ecp/)izberite **pravila toka pošte >**.</span><span class="sxs-lookup"><span data-stu-id="56992-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="56992-104">Kliknite ikono **novo (+)** , nato pa kliknite **uporabi šifriranje sporočil sistema Office 365 in zaščito pravic za sporočila**.</span><span class="sxs-lookup"><span data-stu-id="56992-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="56992-105">V polje **ime** vnesite ime za pravilo, na primer *Šifriraj vsa sporočila*.</span><span class="sxs-lookup"><span data-stu-id="56992-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="56992-106">**Če želite uporabiti to pravilo**, izberite **[uporabi za vsa sporočila]**.</span><span class="sxs-lookup"><span data-stu-id="56992-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="56992-107">Poleg polja **naredi to** kliknite **Izberi eno**.</span><span class="sxs-lookup"><span data-stu-id="56992-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="56992-108">V spustnem meniju **predloga RMS** izberite **Šifriraj** in nato kliknite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="56992-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="56992-109">(Če ne vidite te možnosti, to pomeni, da vaš paket ne vključuje samodejnega šifriranja.</span><span class="sxs-lookup"><span data-stu-id="56992-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="56992-110">Vendar ga lahko dodate!)</span><span class="sxs-lookup"><span data-stu-id="56992-110">But you can add it!)</span></span>
7. <span data-ttu-id="56992-111">Potrdite potrditveno polje **Nadziraj to pravilo z ravnjo resnosti** in nato izberite želeno raven.</span><span class="sxs-lookup"><span data-stu-id="56992-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="56992-112">Če ima vaše podjetje pogodbene obveznosti, da pošljejo vsa šifrirana e-poštna sporočila, vam priporočam, da nastavite raven na **visoko**.</span><span class="sxs-lookup"><span data-stu-id="56992-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="56992-113">V razdelku **Izberite model za to pravilo** kliknite **Uveljavi**.</span><span class="sxs-lookup"><span data-stu-id="56992-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="56992-114">Izberite poljuben izbirni izbor (na seznamu izbirnih izbir, ki jih lahko naredite na tej strani, od katerih jih je mogoče preprostiti s privzeto nastavitev za enostavnost).</span><span class="sxs-lookup"><span data-stu-id="56992-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="56992-115">Kliknite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="56992-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="56992-116">Pozneje se lahko vrnete in uredite to pravilo.</span><span class="sxs-lookup"><span data-stu-id="56992-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="56992-117">Če želite več informacij o ustvarjanju pravil za šifriranje, glejte [določanje pravil pretoka pošte za šifriranje e-poštnih sporočil v storitvi Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="56992-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

