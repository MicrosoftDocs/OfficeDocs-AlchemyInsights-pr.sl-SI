---
title: Popravljanje Officeovih aplikacij vaš račun je v slabem stanju sporočilo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969803"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="0fd07-102">Popravljanje Officeovih aplikacij» vaš račun je v slabem stanju «</span><span class="sxs-lookup"><span data-stu-id="0fd07-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="0fd07-103">Če želite odpraviti to napako, poskusite naslednje možnosti v prizadetem računalniku:</span><span class="sxs-lookup"><span data-stu-id="0fd07-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="0fd07-104">Odprite Officeovo aplikacijo, izberite račun **datotečnega** > **računa** > **iz vseh računov**.</span><span class="sxs-lookup"><span data-stu-id="0fd07-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="0fd07-105">Znova se vpišite z uporabniškim računom z veljavno licenco.</span><span class="sxs-lookup"><span data-stu-id="0fd07-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="0fd07-106">Za podrobnejše informacije glejte [računi v Officeu](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="0fd07-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="0fd07-107">[Počistite Officeove poverilnice](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) z upraviteljem poverilnic Windows.</span><span class="sxs-lookup"><span data-stu-id="0fd07-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="0fd07-108">**Opomba:** Registrske poti za Office 2016 so se spremenile v 16,0.</span><span class="sxs-lookup"><span data-stu-id="0fd07-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="0fd07-109">Na primer \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="0fd07-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="0fd07-110">V prizadetem računalniku nastavite EnableADAL = 0 z naslednjimi koraki:</span><span class="sxs-lookup"><span data-stu-id="0fd07-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="0fd07-111">Z desno tipko miške kliknite gumb Windows in izberite **Zaženi**.</span><span class="sxs-lookup"><span data-stu-id="0fd07-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="0fd07-112">V polje **Odpri** vnesite **regedit**in nato izberite **v redu**.</span><span class="sxs-lookup"><span data-stu-id="0fd07-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="0fd07-113">Izberite **da** , ko se prikaže poziv, da urejevalnik registra omogoča spreminjanje vaše naprave.</span><span class="sxs-lookup"><span data-stu-id="0fd07-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="0fd07-114">V urejevalniku registra dodajte vrednost DWORD EnableADAL z nastavitvijo 0 pod HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="0fd07-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="0fd07-115">Če pride do napake med povezovanjem z Officeom 365 z Officeom 2013, [omogočite sodobno preverjanje pristnosti](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) za odjemalca Office.</span><span class="sxs-lookup"><span data-stu-id="0fd07-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="0fd07-116">Če želite več informacij, glejte [Odpravljanje težav z aplikacijami brez brskalnika, ki se ne morejo prijaviti v Office 365, Azure ali InTune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="0fd07-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

