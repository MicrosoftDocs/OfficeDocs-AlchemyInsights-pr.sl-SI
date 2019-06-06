---
title: Uvod v SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: a44b2c7b26895e09c24df772f1ada9a2e3483747
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735998"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="ebf07-102">Poteke dela v SharePointu</span><span class="sxs-lookup"><span data-stu-id="ebf07-102">Workflows in SharePoint</span></span>

<span data-ttu-id="ebf07-103">Če SharePoint poteki dela ne pošiljate e-pošto, vaše organizacije so se pojavile meje Exchange Online pošiljatelja.</span><span class="sxs-lookup"><span data-stu-id="ebf07-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="ebf07-104">"Potek dela je prekinjena" sporočilo o napaki pride, če imate eno od naslednjih postavk:</span><span class="sxs-lookup"><span data-stu-id="ebf07-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="ebf07-105">Imate potek dela v SharePoint Online, ki uporablja SharePoint 2010 ali tip platforme SharePoint 2013 poteka dela.</span><span class="sxs-lookup"><span data-stu-id="ebf07-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="ebf07-106">Potek dela je nastavljen tako, da po meri email sporočilo poslati več kot 200 uporabnikov naenkrat, več kot 10.000 prejemniki na dan ali več kot 30 sporočil na minuto.</span><span class="sxs-lookup"><span data-stu-id="ebf07-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="ebf07-107">Ko zaženete potek dela, e-poštno sporočilo ni poslano, in boste opazili sporočilo o napaki, notranje stanje nastavljeno na prekinjena ali ne morem poslati prejemniku je prikazana.</span><span class="sxs-lookup"><span data-stu-id="ebf07-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="ebf07-108">Če želite več informacij, si oglejte [članek](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="ebf07-108">For more information, please refer to the following [article](https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

