---
title: Azure PowerShell Az 모듈 소개
description: AzureRM 모듈을 대체하는 새로운 Azure PowerShell 모듈 Az을 소개합니다.
ms.date: 12/13/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 10665a72bc7dcae8ecf36b5ef4e2ab285a0e78b7
ms.sourcegitcommit: 89066b7c4b527357bb2024e1ad708df84c131804
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/09/2019
ms.locfileid: "59364102"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a><span data-ttu-id="7e219-103">새로운 Azure PowerShell Az 모듈 소개</span><span class="sxs-lookup"><span data-stu-id="7e219-103">Introducing the new Azure PowerShell Az module</span></span>

<span data-ttu-id="7e219-104">2018년 12월부터 Azure PowerShell Az 모듈은 일반 릴리스로 출시되며 Azure와 상호 작용하기 위한 PowerShell 모듈입니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-104">Starting in December 2018, the Azure PowerShell Az module is in general release and now the intended PowerShell module for interacting with Azure.</span></span> <span data-ttu-id="7e219-105">Az은 짧아진 명령과 향상된 안정성을 제공하며, 플랫폼 간 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-105">Az offers shorter commands, improved stability, and cross-platform support.</span></span> <span data-ttu-id="7e219-106">Az은 AzureRM의 동일한 기능을 제공하는 동시에 AzureRM에서 쉬운 마이그레이션 경로를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-106">Az also offers feature parity and an easy migration path from AzureRM.</span></span>

<span data-ttu-id="7e219-107">Az는 .NET 표준 라이브러리를 사용합니다. 즉, PowerShell 5 및 PowerShell 6에서 실행됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-107">Az uses the .NET Standard library, which means it runs on PowerShell 5 and PowerShell 6.</span></span>
<span data-ttu-id="7e219-108">PowerShell 6은 Linux, macOS 및 Windows에서 실행할 수 있으므로, Azure PowerShell은 이제 모든 플랫폼에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-108">Since PowerShell 6 can run on Linux, macOS, and Windows, Azure PowerShell is now available for all platforms.</span></span>
<span data-ttu-id="7e219-109">.NET 표준을 사용하면 사용자에게 미치는 영향을 최소화하면서 Azure PowerShell의 코드 기반을 통합할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-109">Using .NET Standard allows us to unify the code base of Azure PowerShell with minimal impact on users.</span></span>

<span data-ttu-id="7e219-110">Az는 새로운 모듈이기 때문에 버전이 1.0.0으로 다시 설정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-110">Az is a new module, so the version has been reset to 1.0.0.</span></span>

## <a name="upgrade-to-az"></a><span data-ttu-id="7e219-111">Az로 업그레이드</span><span class="sxs-lookup"><span data-stu-id="7e219-111">Upgrade to Az</span></span>

<span data-ttu-id="7e219-112">새로운 Az 모듈로 업그레이드하는 것이 권장되며 업그레이드 절차는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-112">It's recommended that all users upgrade to the new Az module.</span></span> <span data-ttu-id="7e219-113">이렇게 하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-113">To do so:</span></span>

* <span data-ttu-id="7e219-114">__권장__: [Azure PowerShell AzureRM 모듈 제거](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)</span><span class="sxs-lookup"><span data-stu-id="7e219-114">__RECOMMENDED__: [Uninstall the Azure PowerShell AzureRM module](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)</span></span>
* [<span data-ttu-id="7e219-115">Azure PowerShell Az 모듈 설치</span><span class="sxs-lookup"><span data-stu-id="7e219-115">Install the Azure PowerShell Az module</span></span>](/powershell/azure/install-az-ps)
* <span data-ttu-id="7e219-116">새 명령 집합에 익숙해지면서 `Enable-AzureRMAlias`로 AzureRM cmdlet을 위한 별칭 추가를 위한 호환 모드를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-116">Enable compatibility mode to add aliases for AzureRM cmdlets with `Enable-AzureRMAlias` while you become familiar with the new command set.</span></span> <span data-ttu-id="7e219-117">AzureRM이 설치되지 않은 경우__만__ 별칭을 사용하도록 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-117">__Only__ enable aliases if you do not have AzureRM installed.</span></span>

## <a name="migrate-existing-scripts-to-az"></a><span data-ttu-id="7e219-118">기존 스크립트를 Az로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="7e219-118">Migrate existing scripts to Az</span></span>

<span data-ttu-id="7e219-119">주요 업데이트가 불편할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-119">Major updates can be inconvenient.</span></span> <span data-ttu-id="7e219-120">그러나 Az 모듈에는 새로운 구문에 대한 업데이트 작업을 하는 동안 기존 스크립트를 사용할 수 있도록 해주는 호환 모드가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-120">However, the Az module has a compatibility mode to help you use existing scripts while you work on updates to the new syntax.</span></span> <span data-ttu-id="7e219-121">`Enable-AzureRmAlias` cmdlet을 사용하여 AzureRM 호환 모드를 활성화합니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-121">Use the `Enable-AzureRmAlias` cmdlet to enable the AzureRM compatibility mode.</span></span> <span data-ttu-id="7e219-122">이 cmdlet은 AzureRM cmdlet 이름을 새 Az cmdlet 이름의 별칭으로 정의합니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-122">This cmdlet defines AzureRM cmdlet names as aliases for the new Az cmdlet names.</span></span>

<span data-ttu-id="7e219-123">새로운 cmdlet 이름은 쉽게 익힐 수 있도록 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-123">The new cmdlet names have been designed to be easy to learn.</span></span> <span data-ttu-id="7e219-124">cmdlet 이름에 `AzureRm` 또는 `Azure`를 사용하는 대신 `Az`를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-124">Instead of using `AzureRm` or `Azure` in cmdlet names, use `Az`.</span></span> <span data-ttu-id="7e219-125">예를 들어, 이전 명령 `New-AzureRMVm`은 `New-AzVm`이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-125">For example, the old command `New-AzureRMVm` has become `New-AzVm`.</span></span>

<span data-ttu-id="7e219-126">마이그레이션 프로세스에 대한 전체 설명은 [AzureRM에서 Az로 마이그레이션](migrate-from-azurerm-to-az.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="7e219-126">For a full description of the migration process, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

## <a name="the-future-of-support-for-azurerm"></a><span data-ttu-id="7e219-127">AzureRM에 대한 향후 지원</span><span class="sxs-lookup"><span data-stu-id="7e219-127">The future of support for AzureRM</span></span>

<span data-ttu-id="7e219-128">기존 AzureRM 모듈은 새 cmdlet 또는 기능을 더 이상 받을 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-128">The existing AzureRM module will no longer receive new cmdlets or features.</span></span> <span data-ttu-id="7e219-129">그러나 AzureRM은 공식적으로 유지되며 2020년 12월까지 버그 수정도 이루어집니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-129">However, AzureRM is still officially maintained and will get bug fixes up through December 2020.</span></span> <span data-ttu-id="7e219-130">최신 Azure 서비스 및 기능을 유지하기 위해서는 Az 모듈로 전환해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="7e219-130">To keep up with the latest Azure services and features, switch to the Az module.</span></span>
