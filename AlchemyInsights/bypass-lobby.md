---
title: Obvozna avla
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684966"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="367bd-102">Nadzor nastavitev lobija in raven sodelovanja v aplikaciji Teams</span><span class="sxs-lookup"><span data-stu-id="367bd-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="367bd-103">Če želite vsem, vključno s klici, zunanjimi in anonimnimi Uporabniki, omogočiti, da **zaobidejo preddverje**, uporabite PowerShell za izpolnitev tega opravila.</span><span class="sxs-lookup"><span data-stu-id="367bd-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="367bd-104">Tukaj je primer spreminjanja globalnega pravilnika za srečanje za vašo organizacijo.</span><span class="sxs-lookup"><span data-stu-id="367bd-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="367bd-105">Ta ukaz» cmdlet «trenutno zahteva uporabo modula za Skype za podjetja PowerShell.</span><span class="sxs-lookup"><span data-stu-id="367bd-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="367bd-106">Če želite nastaviti nastavitev za uporabo tega ukaza» cmdlet «, si oglejte [upravljanje pravilnikov prek lupine PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="367bd-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="367bd-107">Ko nastavite pravilnik, ga morate uporabiti za uporabnike; Če pa ste spremenili globalni pravilnik, bo ta samodejno veljal za uporabnike.</span><span class="sxs-lookup"><span data-stu-id="367bd-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="367bd-108">Za vsako spremembo pravilnika morate počakati vsaj **4 ure do 24 ur** , da bodo pravilniki lahko uveljavljeni.</span><span class="sxs-lookup"><span data-stu-id="367bd-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="367bd-109">Če želite, da bodo te spremembe natančno razumele, kaj to omogoča, si oglejte dokumentacijo, ki je spodaj.</span><span class="sxs-lookup"><span data-stu-id="367bd-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="367bd-110">Razumevanje kontrolnikov pravilnika lobiranja za Teams</span><span class="sxs-lookup"><span data-stu-id="367bd-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="367bd-111">Te nastavitve nadzirajo, kateri udeleženci srečanja čakajo v preddverju, preden so sprejeti v srečanje, in raven udeležbe, ki jim je dovoljen v srečanju.</span><span class="sxs-lookup"><span data-stu-id="367bd-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="367bd-112">S funkcijo PowerShell lahko posodobite nastavitve pravilnika srečanja, ki še niso bile uveljavljene (z oznako» kmalu na voljo «) v skrbniškem središču za ekipe.</span><span class="sxs-lookup"><span data-stu-id="367bd-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="367bd-113">Glejte spodaj za primer» cmdlet «lupine PowerShell, ki vsem uporabnikom omogoča, da zaobidejo preddverje.</span><span class="sxs-lookup"><span data-stu-id="367bd-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="367bd-114">[Samodejno priznavanje oseb](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) je pravilnik per organizatorja, ki nadzoruje, ali se ljudje neposredno pridruževanjo srečanju ali počakajo v čakalnici, dokler jih ne sprejme uporabnik s preverjeno pristnostjo.</span><span class="sxs-lookup"><span data-stu-id="367bd-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="367bd-115">[Dovolite anonimnim osebam, da začnejo srečanje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) , je pravilnik na organizatorju, ki nadzoruje, ali se lahko anonimni ljudje, vključno z uporabniki B2B in Združenega uporabnika, pridružite srečanju uporabnikov brez preverjanja pristnosti v organizaciji.</span><span class="sxs-lookup"><span data-stu-id="367bd-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="367bd-116">[Dovoli klicnim uporabnikom, da zaobidejo preddverje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**kmalu**na voljo) je pravilnik na organizatorju, ki nadzoruje, ali osebe, ki kličejo s telefonom, neposredno pridružijo srečanju ali pa počakajo v preddverju, ne glede na nastavitev **samodejno priznavanje oseb** .</span><span class="sxs-lookup"><span data-stu-id="367bd-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="367bd-117">[Dovoli organizatorjem, da preglasijo nastavitve lobija](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**kmalu**na voljo) je pravilnik per organizatorja, ki nadzoruje, ali lahko organizator srečanja preglasi nastavitve lobija, ki jih skrbnik **samodejno prizna osebam** in **Dovoli klicne uporabnike, da zaobidejo preddverje** , ko načrtujejo novo srečanje.</span><span class="sxs-lookup"><span data-stu-id="367bd-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="367bd-118">**Opomba:** Preberite [upravljanje pravilnikov za srečanje v aplikaciji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za popoln pregled pravilnikov za srečanje Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="367bd-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
