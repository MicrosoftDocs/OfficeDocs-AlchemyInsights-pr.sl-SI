---
title: Konsistenciin GUID/sourceAnchor obnašanje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705749"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="ff485-102">Konsistenciin GUID/sourceAnchor obnašanje</span><span class="sxs-lookup"><span data-stu-id="ff485-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="ff485-103">Azure AD Connect (različica 1.1.524.0 in pozneje) zdaj olajšuje uporabo msDS-doslednosti GUID kot atribut sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="ff485-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="ff485-104">Ko uporabljate to funkcijo, Azure AD Connect samodejno konfigurira pravila sinhronizacije tako, da:</span><span class="sxs-lookup"><span data-stu-id="ff485-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="ff485-105">Uporabite msDS-Konsistenciuuguid kot atribut sourceAnchor za uporabniške predmete.</span><span class="sxs-lookup"><span data-stu-id="ff485-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="ff485-106">ObjectGUID se uporablja za druge vrste predmetov.</span><span class="sxs-lookup"><span data-stu-id="ff485-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="ff485-107">V katerem koli danem krajevnem uporabniškem predmetu AD, katerega atribut msDS-Konsistencyguid ni poseljen, Azure AD Connect zapiše svojo vrednost objectGUID nazaj v atribut msDS-Konsistencyguid v krajevnem imeniku Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ff485-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="ff485-108">Ko je atribut msDS-Konsistencyguid naseljen, Azure AD Connect nato izvozi predmet v Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ff485-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="ff485-109">**Opomba:** Ko se krajevni predmet oglasa uvozi v Azure AD Connect (to je uvoženo v prostor AD Connector in napovedano v metaverse), ne morete več spreminjati vrednosti sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="ff485-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="ff485-110">Če želite določiti vrednost sourceAnchor za dani krajevni predmet oglasa, konfigurirajte atribut msDS-Konsistencyguid, preden ga uvozite v Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="ff485-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="ff485-111">Če želite več informacij o SourceAnchor in doslednosti GUID-a, glejte naslednje: [AZURE ad Connect: oblikovalni koncepti](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="ff485-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

