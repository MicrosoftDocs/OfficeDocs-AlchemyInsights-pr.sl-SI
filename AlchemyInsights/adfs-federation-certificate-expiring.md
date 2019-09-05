---
title: ADFS Federation certifikat poteče
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737205"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="01fde-102">ADFS Federation certifikat poteče</span><span class="sxs-lookup"><span data-stu-id="01fde-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="01fde-103">Če želite odpraviti to težavo, sledite tem korakom:</span><span class="sxs-lookup"><span data-stu-id="01fde-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="01fde-104">Namestite modul Microsoft Azure Active Directory za lupino Windows PowerShell v računalniku (če modul še ni nameščen).</span><span class="sxs-lookup"><span data-stu-id="01fde-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="01fde-105">Če želite to narediti, pojdite na [upravljanje programa AZURE ad z lupino Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="01fde-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="01fde-106">Sledite korakom v razdelku» scenarij 1: potekla je veljavnost potrdila za podpisovanje žetonov AD FS «iz [» prišlo je do napake pri dostopu do mesta «iz AD FS, ko se je Združeno uporabnik prijavil v Office 365, Azure ali InTune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="01fde-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="01fde-107">Sledite korakom v [posodobitvi ali popravite nastavitve federirane domene v Officeu 365, Azure ali InTune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span><span class="sxs-lookup"><span data-stu-id="01fde-107">Follow the steps in [Update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="01fde-108">Če želite izvedeti več o podaljšanju potrdil federacije, glejte [obnovitev potrdil federacije za Office 365 in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="01fde-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
