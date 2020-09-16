---
title: Ustvarjanje mesta v storitvi SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732256"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="c9e90-102">Ustvarjanje SharePointovih mest s predlogami</span><span class="sxs-lookup"><span data-stu-id="c9e90-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="c9e90-103">Možnost shranjevanja mesta kot predloge ni podprta s sodobnimi komunikacijskimi ali spletnimi mesti skupine.</span><span class="sxs-lookup"><span data-stu-id="c9e90-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="c9e90-104">Če želite več informacij o uporabi predlog [, glejte shranjevanje, prenos in prenos SharePointovega mesta kot predloge](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="c9e90-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="c9e90-105">Tukaj je nekaj pogostih težav/rešitev glede shranjevanja mesta ali seznama kot predloge v SharePoint Onlineu.</span><span class="sxs-lookup"><span data-stu-id="c9e90-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="c9e90-106">**Gumb» Shrani spletno mesto/seznam «ni na voljo ali manjka**</span><span class="sxs-lookup"><span data-stu-id="c9e90-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="c9e90-107">Skrbniki bodo morali omogočiti skript po meri, če želite omogočiti funkcije predloge.</span><span class="sxs-lookup"><span data-stu-id="c9e90-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="c9e90-108">Za podrobne korake, primere in premisleke glejte</span><span class="sxs-lookup"><span data-stu-id="c9e90-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="c9e90-109">Omogočanje ali preprečevanje skripta po meri</span><span class="sxs-lookup"><span data-stu-id="c9e90-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="c9e90-110">Ukaz» Shrani mesto kot predlogo «ni podprt in lahko povzroči težave na mestih, ki uporabljajo SharePoint Server Publishing Infrastructure.</span><span class="sxs-lookup"><span data-stu-id="c9e90-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="c9e90-111">**Predloge mesta ni mogoče ustvariti ali pa ne deluje pravilno**</span><span class="sxs-lookup"><span data-stu-id="c9e90-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="c9e90-112">Predloga morda manjka [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) in ne bo aktivirana.</span><span class="sxs-lookup"><span data-stu-id="c9e90-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="c9e90-113">Če funkcija ni na voljo za aktiviranje v trenutni zbirki mest, ne morete uporabiti predloge mesta za ustvarjanje spletnega mesta.</span><span class="sxs-lookup"><span data-stu-id="c9e90-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="c9e90-114">Preverite, ali kateri koli seznami ali knjižnice presegajo [mejni prag pogleda seznama](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) v 5000 elementih, saj lahko to blokira ustvarjanje predloge mesta.</span><span class="sxs-lookup"><span data-stu-id="c9e90-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="c9e90-115">Mesto lahko uporablja preveč virov in zato predloga mesta presega omejitev 50 MB.</span><span class="sxs-lookup"><span data-stu-id="c9e90-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="c9e90-116">Na voljo so težave s prikazom podatkov s seznama, ki uporablja stolpec za iskanje.</span><span class="sxs-lookup"><span data-stu-id="c9e90-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="c9e90-117">Če želite več informacij, glejte [seznam ustvarjenih predlog ne prikazuje podatkov s pravilnega seznama za iskanje v storitvi SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="c9e90-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="c9e90-118">Če želite podrobnejše informacije o pogostih težavah in rešitvah, glejte [Ustvarjanje in uporaba predlog spletnega mesta](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="c9e90-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



