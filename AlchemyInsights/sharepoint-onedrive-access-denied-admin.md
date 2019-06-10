---
title: Odpravljanje težav s postranski tajivec vest
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760356"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="962a6-102">Odpravljanje težav s postranski tajivec sporočil v skrbniškem središču za Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="962a6-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="962a6-103">Če prejmete sporočilo o zavrnjenem ko poskušate brskati za Sharepoint/OneDrive Admin Center dostopu, prepričajte se, da vam [dodeli dovoljenje za uporabnika](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="962a6-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="962a6-104">Če ima uporabnik dovoljenje, prav tako se prepričajte, so [dodeljena skrbniška vloga](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) ki lahko dostop do admin centri.</span><span class="sxs-lookup"><span data-stu-id="962a6-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="962a6-105">Ta težava se lahko pojavi tudi, ko uporabnik izbriše in ponovno ustvari z enakim glavnim imenom uporabnika (UPN).</span><span class="sxs-lookup"><span data-stu-id="962a6-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="962a6-106">Novi račun je ustvarjen z uporabo različnih PUID (Passport Enolični ID) vrednost.</span><span class="sxs-lookup"><span data-stu-id="962a6-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="962a6-107">Ko uporabnik poskuša za dostop do zbirke mest ali njihovih OneDrive, uporabnik je napačno PUID.</span><span class="sxs-lookup"><span data-stu-id="962a6-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="962a6-108">Drugi scenarij vključuje sinhronizacija imenika z Active Directory organizacijska enota (OU).</span><span class="sxs-lookup"><span data-stu-id="962a6-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="962a6-109">Če uporabniki so že vpisani v SharePoint, in nato preselil v različnih OU in resynced s SharePointom, da lahko pride do te težave.</span><span class="sxs-lookup"><span data-stu-id="962a6-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="962a6-110">Če želite težavo odpraviti, obnovite izvirno UPN s korakom v članku, [obnoviti uporabnik v Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="962a6-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="962a6-111">Opomba: Če je OneDrive ali SharePoint Admin center ni na voljo za več uporabnikov, ki so prej imeli dostopa, lahko pride začasno storitev vprašanje.</span><span class="sxs-lookup"><span data-stu-id="962a6-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="962a6-112">[Preverite zdravje Nadzorna plošča storitev](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="962a6-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

