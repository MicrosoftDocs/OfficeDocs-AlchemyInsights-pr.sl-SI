---
title: Ustvarite in uporabljate nabiralnik v skupni rabi
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762416"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="bcc2f-102">Odpravljanje težave - uporabnika ni mogoče najti v imeniku</span><span class="sxs-lookup"><span data-stu-id="bcc2f-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="bcc2f-103">Če uporabniki prejemajo napake sporočilo "uporabnika ni mogoče najti" v imeniku.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="bcc2f-104">Prosimo, poskusite znova kjer vrsto izdaje je uporabnik ni v imeniku.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="bcc2f-105">Takole je treba izpolniti za pri odpravljanju težav.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="bcc2f-106">Zagotovitev račun, ki je sprejel povabilo email je isti račun, ki se uporablja za vpis v kasneje.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="bcc2f-107">Preverite, ali uporabnik uporablja isti račun sprejmite povabilo, in sicer v mestu.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="bcc2f-108">Za več informacij, glejte [kako upravljati vzdevki za račun Microsoft</a> za upravljanje Office 365 prijava](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="bcc2f-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="bcc2f-109">Prebrskajte do vsakega območja(-ij), v katerem uporabnik prejema napako.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="bcc2f-110">Dodaj "/ _layouts/15/people.aspx/membershipgroupid=0" (znotraj dvojnih narekovajev) v prenehati od URL mesta.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="bcc2f-111">Primer: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="bcc2f-112">Na seznamu izberite uporabnika.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-112">Select the user from the list.</span></span>

- <span data-ttu-id="bcc2f-113">Kliknite **Odstrani uporabniška dovoljenja** na traku.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="bcc2f-114">Dodajte nazaj uporabnika in znova pošljite prositi da uporabnik.</span><span class="sxs-lookup"><span data-stu-id="bcc2f-114">Add back the User and Resend the invite to the user.</span></span>
