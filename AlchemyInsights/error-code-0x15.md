---
title: Koda napake 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Če prejmete napako, medtem ko aktivirate Office 2013 na uvajanje storitev oddaljenega namizja (RDS), razmislite o omogočanju ADAL z urejanjem registra.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sl-SI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703154"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="849c2-103">Zmota prebiti activation urad 2013 naprej zakoten pult usluga</span><span class="sxs-lookup"><span data-stu-id="849c2-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="849c2-104">Če prejmete napako, medtem ko aktivirate Office 2013 na uvajanje storitev oddaljenega namizja (RDS), razmislite o omogočanju ADAL z urejanjem registra.</span><span class="sxs-lookup"><span data-stu-id="849c2-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="849c2-105">**Registrski ključ**</span><span class="sxs-lookup"><span data-stu-id="849c2-105">**Registry key**</span></span>|<span data-ttu-id="849c2-106">**Vrsta**</span><span class="sxs-lookup"><span data-stu-id="849c2-106">**Type**</span></span>|<span data-ttu-id="849c2-107">**Vrednost**</span><span class="sxs-lookup"><span data-stu-id="849c2-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="849c2-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="849c2-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="849c2-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="849c2-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="849c2-110">1</span><span class="sxs-lookup"><span data-stu-id="849c2-110">1</span></span>  <br/> |

<span data-ttu-id="849c2-111">Če želite več informacij, glejte [Omogočanje modernega preverjanja pristnosti za Office 2013 v napravah s sistemom Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="849c2-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="849c2-112">ADAL je privzeto omogočen v Microsoft 365 apps za podjetja in Office 2016.</span><span class="sxs-lookup"><span data-stu-id="849c2-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="849c2-113">Storitve oddaljenega namizja (RDS) so bile prej imenovane terminalske storitve.</span><span class="sxs-lookup"><span data-stu-id="849c2-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  