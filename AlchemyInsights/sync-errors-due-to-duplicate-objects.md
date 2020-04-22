---
title: 902 (sinhronizacija napak zaradi podvojenih predmetov)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767151"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="86caa-102">Sinhronizacija napak zaradi podvojenih predmetov</span><span class="sxs-lookup"><span data-stu-id="86caa-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="86caa-103">Ko se sinhronizacija imenika dokonča v Microsoft 365, se lahko prikaže eno od teh sporočil o napaki:</span><span class="sxs-lookup"><span data-stu-id="86caa-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="86caa-104">Tega predmeta ni mogoče posodobiti v storitvah Microsoft Online Services, ker imajo naslednji atributi, povezani s tem predmetom, vrednosti, ki so morda že povezane z drugim predmetom v lokalnem imeniku.</span><span class="sxs-lookup"><span data-stu-id="86caa-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="86caa-105">Sinhroniziran predmet z istim naslovom proxy že obstaja v imeniku Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="86caa-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="86caa-106">Tega predmeta ni mogoče posodobiti, ker imajo naslednji atributi, povezani s tem predmetom, vrednosti, ki so morda že povezane z drugim predmetom v lokalnih imeniških storitvah: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="86caa-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="86caa-107">V odkriti ter pritrditi izdaja, travnato gričevje ter prost dostop [Idfix DirSync zmota sanacija orodje](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="86caa-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="86caa-108">Če želite več informacij, glejte [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="86caa-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
