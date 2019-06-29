---
title: Pravilniki o hranjenju v Exchange Admin Center ne deluje
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 9f4a175239bc20aaf489615da63ef35002030a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35369681"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="73807-102">Pravilniki o hranjenju v skrbniškem središču za izmenjavo</span><span class="sxs-lookup"><span data-stu-id="73807-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="73807-103">**Izdaje:** Na novo ustvarjeno ali posodobljeno zadrževanja v skrbniškem središču za izmenjavo ne veljajo za nabiralnike ali artikli ne premesti arhivskega nabiralnika ali izbrisati.</span><span class="sxs-lookup"><span data-stu-id="73807-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="73807-104">**Vzrokov:**</span><span class="sxs-lookup"><span data-stu-id="73807-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="73807-105">To se lahko ker je **Pomočnik upravljane mape** ni predelana uporabnikovega nabiralnika.</span><span class="sxs-lookup"><span data-stu-id="73807-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="73807-106">Pomočnik za upravljane mape Windows poskusi obdelati vse nabiralnike v organizaciji oblaku enkrat vsakih sedem dni.</span><span class="sxs-lookup"><span data-stu-id="73807-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="73807-107">Če spremenite oznako za hranjenje ali uporabljajo pravilnik z nabiralnikom, lahko počakate, dokler uspelo mape pomagajo obdela nabiralnik, ali lahko zaženete ukaz cmdlet Start-ManagedFolderAssistant začeti pomočnik za upravljane mape za obdelavo določenega nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="73807-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="73807-108">Teče ta ukaz »cmdlet« je namenjen preskušanju ali odpravljanju pravilnika o hranjenju ali tag nastavitve hranjenja.</span><span class="sxs-lookup"><span data-stu-id="73807-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="73807-109">Če želite več informacij, obiščite [prost dostop pomočnik za upravljane mape](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="73807-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="73807-110">**Raztopina:** Prost dostop sledeč zapoved v začetek pomočnik za upravljane mape za določen nabiralnik:</span><span class="sxs-lookup"><span data-stu-id="73807-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="73807-111">Pojavi se to lahko tudi, če **RetentionHold** je bila **omogočena** v nabiralniku.</span><span class="sxs-lookup"><span data-stu-id="73807-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="73807-112">Če nabiralnik je postavljena na RetentionHold, s pravilnikom o hranjenju, v nabiralniku ne bo obdelan v tem času.</span><span class="sxs-lookup"><span data-stu-id="73807-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="73807-113">Za več informacije na RetentionHold nastavitev glej: [Nabiralnik hranjenja čakanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="73807-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="73807-114">**Rešitev:**</span><span class="sxs-lookup"><span data-stu-id="73807-114">**Solution:**</span></span>
    
  - <span data-ttu-id="73807-115">Preverite stanje RetentionHold nastavitev na določen nabiralnik v [EKSO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="73807-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="73807-116">Prost dostop sledeč zapoved v **onesposobiti** RetentionHold na določen naslov:</span><span class="sxs-lookup"><span data-stu-id="73807-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="73807-117">Zdaj, znova zaženite upravljane mape pomočnik:</span><span class="sxs-lookup"><span data-stu-id="73807-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="73807-118">**Opomba:** Če nabiralnik je manjši od 10 MB, pomočnik za upravljane mape bo samodejno obdela nabiralnik.</span><span class="sxs-lookup"><span data-stu-id="73807-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
  