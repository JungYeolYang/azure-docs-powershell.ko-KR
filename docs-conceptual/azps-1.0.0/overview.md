---
title: Azure PowerShell 개요
description: 설치 방법 및 시작 방법에 대한 정보가 담긴 Azure PowerShell Az 모듈의 개요입니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 10/29/2018
ms.openlocfilehash: 7982e122d49db4d558648231d1ab8bfeed80be2d
ms.sourcegitcommit: 4acddc7026522c4fe39de2c4424917d88ee01b7e
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 12/21/2018
ms.locfileid: "53736463"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="65eda-103">Azure PowerShell 개요</span><span class="sxs-lookup"><span data-stu-id="65eda-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="65eda-104">Azure PowerShell은 Azure 리소스를 관리하기 위해 [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) 모델을 사용하는 cmdlet 집합을 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="65eda-105">Azure PowerShell은.NET 표준을 사용하여 Windows, macOS 및 Linux에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-105">Azure PowerShell uses .NET Standard, making it available for Windows, macOS, and Linux.</span></span>
<span data-ttu-id="65eda-106">Azure PowerShell은 Azure Cloud Shell에서도 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-106">Azure PowerShell is also available from Azure Cloud Shell.</span></span>

<span data-ttu-id="65eda-107">[Azure Cloud Shell](/azure/cloud-shell/overview)을 사용하여 브라우저에서 Azure PowerShell을 실행하거나 [자신의 컴퓨터에 설치](install-az-ps.md)합니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-107">Use [Azure Cloud Shell](/azure/cloud-shell/overview) to run Azure PowerShell in your browser, or [install locally](install-az-ps.md).</span></span> <span data-ttu-id="65eda-108">[시작하기](get-started-azureps.md) 아티클에서 Azure PowerShell 기본 사항을 배우고 Azure를 시작해 보세요.</span><span class="sxs-lookup"><span data-stu-id="65eda-108">Check out the [Get Started](get-started-azureps.md) article to learn the Azure PowerShell basics and get started with Azure.</span></span>

<span data-ttu-id="65eda-109">Azure PowerShell 최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azureps.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="65eda-109">For information about the latest Azure PowerShell release, see the [release notes](release-notes-azureps.md).</span></span>

## <a name="about-the-new-az-module"></a><span data-ttu-id="65eda-110">새 Az 모듈 정보</span><span class="sxs-lookup"><span data-stu-id="65eda-110">About the new Az module</span></span>

<span data-ttu-id="65eda-111">이 설명서에서는 Azure PowerShell을 위한 새 Az 모듈을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-111">This documentation describes the new Az module for Azure PowerShell.</span></span> <span data-ttu-id="65eda-112">이 새 모듈은.NET 표준으로 처음부터 작성됩니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-112">This new module is written from the ground up in .NET Standard.</span></span> <span data-ttu-id="65eda-113">.NET 표준을 사용하면 Azure PowerShell을 Windows의 PowerShell 5.x 또는 모든 플랫폼의 PowerShell 6에서 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-113">Using .NET Standard allows Azure PowerShell to run under PowerShell 5.x on Windows or PowerShell 6 on any platform.</span></span> <span data-ttu-id="65eda-114">Az 모듈은 이제 PowerShell을 통해 Azure와 상호 작용하도록 의도된 방법입니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-114">The Az module is now the intended way to interact with Azure through PowerShell.</span></span>
<span data-ttu-id="65eda-115">AzureRM의 버그 수정은 계속되지만, 새로운 기능은 더 이상 받지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-115">AzureRM will continue to get bug fixes, but no longer receive new features.</span></span>

<span data-ttu-id="65eda-116">[Azure PowerShell Az 모듈 소개](new-azureps-module-az.md)에서 명령의 이름이 변경된 내용과 AzureRM의 유지 관리 계획을 포함하여 새 모듈에 대한 자세한 내용을 확인할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-116">Learn the full details about the new module, including how commands have been renamed and the maintenance plans for AzureRM, in the [Introducing the Azure PowerShell Az module](new-azureps-module-az.md).</span></span> <span data-ttu-id="65eda-117">지금 바로 새 모듈을 사용하여 시작하려는 경우 [AzureRM에서 Az로 마이그레이션](migrate-from-azurerm-to-az.md)을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-117">If you want to get started with using the new module right away, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

<span data-ttu-id="65eda-118">[AzureRM 설명서](/powershell/azure/azurerm)도 제공됩니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-118">The [AzureRM documentation](/powershell/azure/azurerm) is also available.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="65eda-119">Azure 설명서가 새로운 모듈 cmdlet 이름을 반영하도록 업데이트되는 동안 아티클은 여전히 AzureRM 명령을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-119">While the Azure documentation is being updated to reflect the new module cmdlet names, articles may still use the AzureRM commands.</span></span> <span data-ttu-id="65eda-120">Az 모듈을 설치한 후 `Enable-AzureRmAlias`를 사용하여 AzureRM cmdlet 별칭을 사용하도록 하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-120">After installing the Az module, it's recommended that you enable the AzureRM cmdlet aliases with `Enable-AzureRmAlias`.</span></span> <span data-ttu-id="65eda-121">자세한 내용은 [AzureRM에서 Az로 마이그레이션](migrate-from-azurerm-to-az.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="65eda-121">See the [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md) article for more details.</span></span>

## <a name="common-scenarios"></a><span data-ttu-id="65eda-122">일반적인 시나리오</span><span class="sxs-lookup"><span data-stu-id="65eda-122">Common scenarios</span></span>

<span data-ttu-id="65eda-123">다음 샘플을 통해 Azure PowerShell로 일반 시나리오를 수행하는 방법을 배울 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-123">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="65eda-124">Linux Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="65eda-124">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="65eda-125">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="65eda-125">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="65eda-126">Web Apps</span><span class="sxs-lookup"><span data-stu-id="65eda-126">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="65eda-127">SQL Databases</span><span class="sxs-lookup"><span data-stu-id="65eda-127">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a><span data-ttu-id="65eda-128">PowerShell 기본 사항 알아보기</span><span class="sxs-lookup"><span data-stu-id="65eda-128">Learn PowerShell basics</span></span>

<span data-ttu-id="65eda-129">PowerShell에 대해 익숙하지 않으면 소개가 도움이 될 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-129">If you're unfamiliar with PowerShell, an introduction may be helpful.</span></span>

* [<span data-ttu-id="65eda-130">PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="65eda-130">Installing PowerShell</span></span>](/powershell/scripting/setup/installing-windows-powershell)
* [<span data-ttu-id="65eda-131">PowerShell 스크립팅</span><span class="sxs-lookup"><span data-stu-id="65eda-131">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)

<span data-ttu-id="65eda-132">이 비디오를 시청할 수도 있습니다. [PowerShell 기본 사항: (파트 1)PowerShell 시작](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)</span><span class="sxs-lookup"><span data-stu-id="65eda-132">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

<span data-ttu-id="65eda-133">또는 Microsoft Virtual Academy의 [PowerShell 시작](https://mva.microsoft.com/liveevents/powershell-jumpstart)에 참석합니다.</span><span class="sxs-lookup"><span data-stu-id="65eda-133">Or attend the Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart).</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="65eda-134">Microsoft Learn을 통해 기술 쌓기</span><span class="sxs-lookup"><span data-stu-id="65eda-134">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="65eda-135">PowerShell을 사용하여 스크립트로 Azure 작업 자동화</span><span class="sxs-lookup"><span data-stu-id="65eda-135">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="65eda-136">더 많은 대화형 학습 보기...</span><span class="sxs-lookup"><span data-stu-id="65eda-136">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="65eda-137">다른 Azure PowerShell 모듈</span><span class="sxs-lookup"><span data-stu-id="65eda-137">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="65eda-138">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="65eda-138">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="65eda-139">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="65eda-139">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="65eda-140">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="65eda-140">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="65eda-141">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="65eda-141">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
