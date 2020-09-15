---
title: Težave pri vpisu v programe Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695195"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="9ea6d-102">Popravljanje aplikacije Microsoft 365 apps» modul zaupanja vredne platforme računalnika ni pravilno delujoč «</span><span class="sxs-lookup"><span data-stu-id="9ea6d-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="9ea6d-103">Če želite to napako odpraviti, poskusite to:</span><span class="sxs-lookup"><span data-stu-id="9ea6d-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="9ea6d-104">Namestite najnovejše posodobitve za [Windows](https://support.microsoft.com/help/4027667/windows-10-update) in [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="9ea6d-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="9ea6d-105">[Počistite Officeove poverilnice](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic sistema Windows.</span><span class="sxs-lookup"><span data-stu-id="9ea6d-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9ea6d-106">**Opomba:** Poti registra za Office 2016 so se spremenile v 16,0.</span><span class="sxs-lookup"><span data-stu-id="9ea6d-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9ea6d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9ea6d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="9ea6d-108">Preskusite [postopek za obnovitev uporabnika](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , da odpravite napake modula zaupanja TPM.</span><span class="sxs-lookup"><span data-stu-id="9ea6d-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="9ea6d-109">Nastavite EnableADAL = 0 s temi koraki:</span><span class="sxs-lookup"><span data-stu-id="9ea6d-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="9ea6d-110">Z desno tipko miške kliknite gumb Start sistema Windows, izberite **Zaženi**, vnesite **regedit**in nato izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="9ea6d-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="9ea6d-111">Izberite **da** , da omogočite urejevalnik registra, da spremenite vašo napravo.</span><span class="sxs-lookup"><span data-stu-id="9ea6d-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="9ea6d-112">V urejevalniku registra dodajte vrednost DWORD **EnableADAL** z nastavitvami **0** v razdelku HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="9ea6d-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="9ea6d-113">Če želite več informacij, glejte [težave s povezavo v vpisu po posodobitvi na Office 2016 Build 16.0.7967 v sistemu Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="9ea6d-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>