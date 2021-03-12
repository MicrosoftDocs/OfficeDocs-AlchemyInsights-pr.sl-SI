---
title: Primer Microsoftovega pravilnika za varno Prilogo sistema Microsoft Defender za Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749196"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="7cebf-102">Primer Microsoftovega pravilnika za varno Prilogo sistema Microsoft Defender za Office 365</span><span class="sxs-lookup"><span data-stu-id="7cebf-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="7cebf-103">Te nastavitve omogočajo pravilnik, imenovan *brez zakasnitve* , ki dostavlja sporočila takoj in nato znova pripne Priloge po skeniranju:</span><span class="sxs-lookup"><span data-stu-id="7cebf-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="7cebf-104">**Ime**: brez zamud</span><span class="sxs-lookup"><span data-stu-id="7cebf-104">**Name**: No delays</span></span>
- <span data-ttu-id="7cebf-105">**Opis**: takoj dostavlja sporočila in znova pripne Priloge po skeniranju.</span><span class="sxs-lookup"><span data-stu-id="7cebf-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="7cebf-106">**Odgovor**: izberite možnost **dinamične dostave** .</span><span class="sxs-lookup"><span data-stu-id="7cebf-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="7cebf-107">Če želite več informacij, glejte [dinamično dostavo v pravilnikih varnih prilog](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="7cebf-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="7cebf-108">Razdelek **preusmeritev Priloge** : izberite možnost, če želite **omogočiti preusmeritev**, nato pa vnesite e-poštni naslov globalnega skrbnika za Microsoft 365, varnostnega skrbnika ali varnostnega analitika, ki bo preiskal zlonamerne Priloge.</span><span class="sxs-lookup"><span data-stu-id="7cebf-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="7cebf-109">**Uporabljeno za** odsek: izberite **domeno prejemnika** in nato izberite domeno.</span><span class="sxs-lookup"><span data-stu-id="7cebf-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="7cebf-110">Izberite **Dodaj**, nato pa izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="7cebf-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="7cebf-111">Ko končate, izberite **Shrani**.</span><span class="sxs-lookup"><span data-stu-id="7cebf-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="7cebf-112">Če želite izvedeti več, glejte [varne Priloge v storitvi Microsoft Defender za Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="7cebf-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
