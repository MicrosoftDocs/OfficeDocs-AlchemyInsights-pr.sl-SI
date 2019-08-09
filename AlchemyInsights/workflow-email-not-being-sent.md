---
title: Potek dela email ni poslan
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270688"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="3003d-102">Potek dela email ni poslan</span><span class="sxs-lookup"><span data-stu-id="3003d-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="3003d-103">Email s poteki dela se ne pošljejo vse uporabnike ali samo določenim uporabnikom, ali vidite napake **e-poštnega sporočila ni mogoče poslati. Preverite, ali je e-mail veljaven prejemnik**.</span><span class="sxs-lookup"><span data-stu-id="3003d-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="3003d-104">Preverite, če uporabnik obstaja v skupini **Vse ljudi** dovoljenja (seznam informacij uporabnik) za to zbirko mest.</span><span class="sxs-lookup"><span data-stu-id="3003d-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="3003d-105">Vzorec neposredno URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="3003d-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="3003d-106">Če uporabnik ne obstaja, se prepričajte, uporabnik je podpisal stran.</span><span class="sxs-lookup"><span data-stu-id="3003d-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="3003d-107">Če gre za zunanjega uporabnika, se prepričajte, da njihovo povabilo sprejme.</span><span class="sxs-lookup"><span data-stu-id="3003d-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="3003d-108">Če uporabnik obstaja v skupini dovoljenja, poskrbite, da naslov ni pravilen.</span><span class="sxs-lookup"><span data-stu-id="3003d-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="3003d-109">Če uporabniki e-poštni naslov ni nastavljena tukaj, ustvarite vzorec Opozorilo za tega uporabnika, ki sili sinhronizacijo uporabniški račun od uporabnikov profil SharePoint v tej zbirki mest.</span><span class="sxs-lookup"><span data-stu-id="3003d-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="3003d-110">Email s poteki dela pošiljajo skrbniki zbirke ne pa drugim uporabnikom in vidim napako \*\*HTTP prepovedano za <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="3003d-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="3003d-111">Glej [Dostop zavrnjen, ko sent email v skupine](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="3003d-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="3003d-112">Prav tako, preverite, ali funkcija zbirke mest **dostop omejen uporabnik dovoljenje lockdown način** ni aktivna.</span><span class="sxs-lookup"><span data-stu-id="3003d-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="3003d-113">Sorodne teme</span><span class="sxs-lookup"><span data-stu-id="3003d-113">Related topics</span></span>
<span data-ttu-id="3003d-114">Želite poskusiti Microsoft Flow v SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="3003d-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="3003d-115">Ustvari tok</span><span class="sxs-lookup"><span data-stu-id="3003d-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="3003d-116">SharePoint in pretok</span><span class="sxs-lookup"><span data-stu-id="3003d-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


