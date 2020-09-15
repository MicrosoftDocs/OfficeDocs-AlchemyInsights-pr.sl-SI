---
title: Pravilo DLP za SSN ne deluje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679385"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="f04b0-102">Težave z DLP s številkami socialnega zavarovanja</span><span class="sxs-lookup"><span data-stu-id="f04b0-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="f04b0-103">**Pomembno**: med temi nepredvidljivimi časi sprejemamo ukrepe, s katerimi skrbimo, da storitvi SharePoint Online in OneDrive ostajata dobro razpoložljivi. Če želite več informacij, si oglejte razdelek [Začasne prilagoditve funkcij storitve SharePoint Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="f04b0-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f04b0-104">**Težave z DLP s številke SSN**</span><span class="sxs-lookup"><span data-stu-id="f04b0-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="f04b0-105">Ali imate težave s **preprečevanjem izgube podatkov (DLP)** ne delate za vsebino, ki vsebuje **številko socialnega zavarovanja (SSN)** , ko uporabljate občutljivo vrsto podatkov v programu Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="f04b0-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="f04b0-106">Če je tako, se prepričajte, da vaša vsebina vsebuje potrebne informacije o tem, kaj išče pravilnik DLP.</span><span class="sxs-lookup"><span data-stu-id="f04b0-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="f04b0-107">Na primer za pravilnik SSN, konfiguriran z ravnjo zaupanja 85%, se ocenijo in jih je treba zaznati, da bo pravilo sprožilo:</span><span class="sxs-lookup"><span data-stu-id="f04b0-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f04b0-108">**[Oblika zapisa:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 številk, ki so lahko v oblikovanem ali neoblikovanem vzorcu</span><span class="sxs-lookup"><span data-stu-id="f04b0-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="f04b0-109">**[Vzorec:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štiri funkcije poiščite številke SSN v štirih različnih vzorcih:</span><span class="sxs-lookup"><span data-stu-id="f04b0-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="f04b0-110">Func_ssn najde številke SSN z močnim oblikovanjem vnaprej 2011, ki so oblikovani s pomišljaji ali presledki (DDD-DD-dddd ali DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="f04b0-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f04b0-111">Func_unformatted_ssn najde številke SSN z močnim oblikovanjem vnaprej 2011, ki niso oblikovani kot devet zaporednih števk (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="f04b0-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="f04b0-112">Func_randomized_formatted_ssn najde številke SSN za 2011, ki so oblikovani s pomišljaji ali presledki (DDD-DD-dddd ali DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="f04b0-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f04b0-113">Func_randomized_unformatted_ssn najde 2011 številke SSN, ki niso oblikovani kot devet zaporednih števk (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="f04b0-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="f04b0-114">**[Preskusna vsota:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, ni checksum</span><span class="sxs-lookup"><span data-stu-id="f04b0-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="f04b0-115">**[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Pravilnik DLP je 85% prepričan, da je zaznal to vrsto občutljivih informacij, če je v bližini 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="f04b0-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f04b0-116">[Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) najde vsebino, ki se ujema z vzorcem.</span><span class="sxs-lookup"><span data-stu-id="f04b0-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f04b0-117">Najde se ključna beseda iz [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="f04b0-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="f04b0-118">Primeri ključnih besed vključujejo:  *socialno varnost, socialno varnost #, SOC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="f04b0-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="f04b0-119">Naslednji vzorec bi na primer sprožil pravilnik DLP: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="f04b0-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="f04b0-120">Če želite več informacij o tem, kaj je potrebno za odkrivanje številke SSN za vašo vsebino, si oglejte ta razdelek v tem članku: [Kaj so občutljive vrste informacij za številke SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="f04b0-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="f04b0-121">Če uporabljate drugačno vgrajeno občutljivo vrsto informacij, si oglejte ta članek za informacije o tem, kaj je zahtevano za druge vrste: [Kaj so videti občutljive vrste informacij](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="f04b0-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  