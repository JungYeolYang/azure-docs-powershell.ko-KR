---
title: AzureRM에서 Az로 Azure PowerShell 스크립트 마이그레이션
description: AzureRM 모듈에서 새 Az 모듈로 스크립트를 마이그레이션하는 단계와 도구에 대해 알아보세요.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 28122ca953d62b405f19effbbc680f2dc6202cca
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/16/2019
ms.locfileid: "54341989"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a><span data-ttu-id="2ea97-103">AzureRM에서 Azure PowerShell Az로 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="2ea97-103">Migrate from AzureRM to Azure PowerShell Az</span></span>

<span data-ttu-id="2ea97-104">Az 모듈은 AzureRM과 기능 패리티를 가지고 있지만 더 짧고 일관된 cmdlet 이름을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-104">The Az module has feature parity with AzureRM, but uses shorter and more consistent cmdlet names.</span></span>
<span data-ttu-id="2ea97-105">AzureRM cmdlet용으로 작성된 스크립트는 새 모듈과 자동으로 작동하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-105">Scripts written for the AzureRM cmdlets won't automatically work with the new module.</span></span> <span data-ttu-id="2ea97-106">쉽게 전환하기 위해 Az는 AzureRM을 사용하여 기존 스크립트를 실행할 수 있는 도구를 제공합니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-106">To make the transition easier, Az offers tools to allow you to run your existing scripts using AzureRM.</span></span> <span data-ttu-id="2ea97-107">새 명령 집합으로 마이그레이션은 편리하지 않지만 이 문서는 새로운 모듈로 전환을 시작하는 데 도움이 됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-107">No migration to a new command set is ever convenient, but this article will help you get started on transitioning to the new module.</span></span>

<span data-ttu-id="2ea97-108">AzureRM과 Az 간의 호환성이 손상되는 전체 변경 목록을 보려면 [Az 1.0.0 마이그레이션 가이드](migrate-az-1.0.0.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2ea97-108">To see the full list of breaking changes between AzureRM and Az, see the [Migration guide for Az 1.0.0](migrate-az-1.0.0.md)</span></span>

## <a name="check-for-installed-versions-of-azurerm"></a><span data-ttu-id="2ea97-109">설치된 AzureRM 버전 확인</span><span class="sxs-lookup"><span data-stu-id="2ea97-109">Check for installed versions of AzureRM</span></span>

<span data-ttu-id="2ea97-110">Az 모듈은 AzureRM 모듈과 나란히 설치할 수 있지만 권장하지는 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-110">The Az module can be installed side-by-side with the AzureRM module, but this is not recommended.</span></span> <span data-ttu-id="2ea97-111">모든 마이그레이션 단계를 수행하기 전에 시스템에 설치된 AzureRM의 버전을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-111">Before taking any migration steps, check which versions of AzureRM are installed on your system.</span></span> <span data-ttu-id="2ea97-112">이렇게 하면 스크립트가 최신 릴리스에서 이미 실행되고 있는지 확인하고 AzureRM을 제거하지 않고 명령 별칭을 사용할 수 있는지 여부를 알려줍니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-112">Doing so allows you to make sure scripts are already running on the latest release, and let you know if you can enable command aliases without uninstalling AzureRM.</span></span>

<span data-ttu-id="2ea97-113">설치한 AzureRM의 버전을 확인하려면 다음 명령을 입력합니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-113">To check which version(s) of AzureRM you have installed, run the command:</span></span>

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a><span data-ttu-id="2ea97-114">기존 스크립트가 최신 AzureRM 릴리스와 함께 작동하는지 확인하세요</span><span class="sxs-lookup"><span data-stu-id="2ea97-114">Ensure your existing scripts work with the latest AzureRM release</span></span>

<span data-ttu-id="2ea97-115">가장 중요한 단계입니다!</span><span class="sxs-lookup"><span data-stu-id="2ea97-115">This is the most important step!</span></span> <span data-ttu-id="2ea97-116">기존 스크립트를 실행하고 AzureRM(__6.13.1__)의 _최신_ 릴리스와 함께 작동하는지 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="2ea97-116">Run your existing scripts, and make sure that they work with the _latest_ release of AzureRM (__6.13.1__).</span></span> <span data-ttu-id="2ea97-117">스크립트가 작동하지 않으면 [AzureRM 마이그레이션 가이드](/powershell/azure/azurerm/migration-guide.6.0.0)를 읽으세요.</span><span class="sxs-lookup"><span data-stu-id="2ea97-117">If your scripts don't work, make sure to read the [AzureRM migration guide](/powershell/azure/azurerm/migration-guide.6.0.0).</span></span>

## <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="2ea97-118">Azure PowerShell Az 모듈 설치</span><span class="sxs-lookup"><span data-stu-id="2ea97-118">Install the Azure PowerShell Az module</span></span>

<span data-ttu-id="2ea97-119">첫 번째 단계는 플랫폼에 Az 모듈을 설치하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-119">The first step is to install the Az module on your platform.</span></span> <span data-ttu-id="2ea97-120">Az를 설치할 때는 AzureRM을 제거하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-120">When you install Az, it's recommended that you uninstall AzureRM.</span></span> <span data-ttu-id="2ea97-121">다음 단계에서는 기존 스크립트를 계속 실행하고 이전 cmdlet 이름과의 호환성을 유지하는 방법을 알아보겠습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-121">In the following steps, you'll learn how to keep running your existing scripts and enable compatibility for old cmdlet names.</span></span>

<span data-ttu-id="2ea97-122">Azure PowerShell Az 모듈을 설치하려면 다음 단계를 수행하십시오.</span><span class="sxs-lookup"><span data-stu-id="2ea97-122">To install the Azure PowerShell Az module, follow these steps:</span></span>

* <span data-ttu-id="2ea97-123">__권장__: [AzureRM 모듈을 제거합니다](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module).</span><span class="sxs-lookup"><span data-stu-id="2ea97-123">__RECOMMENDED__: [Uninstall the AzureRM module](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module).</span></span>
  <span data-ttu-id="2ea97-124">가장 최신 버전뿐만 아니라 설치된 _모든_ AzureRM 버전을 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-124">Make sure that you remove _all_ installed versions of AzureRM, not just the most recent version.</span></span>
* [<span data-ttu-id="2ea97-125">Az 모듈 설치</span><span class="sxs-lookup"><span data-stu-id="2ea97-125">Install the Az module</span></span>](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-compatibility-aliases"></a><span data-ttu-id="2ea97-126"><a name="aliases"/>AzureRM 호환성 별칭을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="2ea97-126"><a name="aliases"/>Enable AzureRM compatibility aliases</span></span> 

> [!IMPORTANT]
>
> <span data-ttu-id="2ea97-127">_모든_ 버전의 AzureRM을 제거한 경우에만 호환성 모드를 활성화하세요.</span><span class="sxs-lookup"><span data-stu-id="2ea97-127">Only enable compatibility mode if you've uninstalled _all_ versions of AzureRM.</span></span> <span data-ttu-id="2ea97-128">AzureRM cmdlet과의 호환 모드를 계속 사용하도록 설정하면 예기치 않은 동작이 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-128">Enabling compatibility mode with AzureRM cmdlets still available may result in unpredictable behavior.</span></span> <span data-ttu-id="2ea97-129">AzureRM을 설치하기로 결정한 경우 이 단계를 건너뛰세요. 그러나 AzureRM cmdlet은 이전 모듈을 사용하고 Az cmdlet은 호출하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-129">Skip this step if you decided to keep AzureRM installed, but be aware that any AzureRM cmdlets will use the older modules and not call any Az cmdlets.</span></span>

<span data-ttu-id="2ea97-130">AzureRM을 제거하고 최신 AzureRM 버전과 함께 스크립트가 작동하면 이제 Az 모듈에 대한 호환 모드를 사용할 때입니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-130">With AzureRM uninstalled and your scripts working with the latest AzureRM version, the next step is to enable the compatibility mode for the Az module.</span></span> <span data-ttu-id="2ea97-131">호환성은 다음 명령으로 사용됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-131">Compatibility is enabled with the command:</span></span>

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="2ea97-132">별칭을 사용하면 Az 모듈이 설치된 이전 cmdlet 이름을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-132">Aliases enable the ability to use old cmdlet names with the Az module installed.</span></span> <span data-ttu-id="2ea97-133">이러한 별칭은 선택한 범위에 대한 사용자 프로필에 기록됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-133">These aliases are written to the user profile for the selected scope.</span></span> <span data-ttu-id="2ea97-134">사용자 프로필이 없으면 프로일 하나가 만들어집니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-134">If no user profile exists, one is created.</span></span>

> [!WARNING]
>
> <span data-ttu-id="2ea97-135">이 명령에 대해 다른 `-Scope`를 사용할 수 있지만 권장되지는 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-135">You can use a different `-Scope` for this command, but it's not recommended.</span></span> <span data-ttu-id="2ea97-136">별칭은 선택된 범위에 대한 사용자 프로필에 기록되므로 가능한 한 범위를 제한적으로 유지합니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-136">Aliases are written to the user profile for the selected scope, so keep enabling them to as limited a scope as possible.</span></span> <span data-ttu-id="2ea97-137">별칭을 시스템 전체에서 사용하도록 설정하면 AzureRM을 로컬 범위에 설치한 다른 사용자에게 문제가 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-137">Enabling aliases system-wide could also cause issues for other users which have AzureRM installed in their local scope.</span></span>

<span data-ttu-id="2ea97-138">별칭 모드가 활성화되면 스크립트를 다시 실행하여 스크립트가 여전히 예상대로 작동하는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-138">Once the alias mode is enabled, run your scripts again to confirm that they still function as expected.</span></span> 

## <a name="change-module-imports-and-cmdlet-names"></a><span data-ttu-id="2ea97-139">모듈 가져오기 및 cmdlet 이름 변경</span><span class="sxs-lookup"><span data-stu-id="2ea97-139">Change module imports and cmdlet names</span></span>

<span data-ttu-id="2ea97-140">일반적으로 모듈 이름은 `AzureRM` 및 `Azure`가 `Az`가 되도록 변경되었으며 cmdlet에도 동일하게 적용됩니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-140">In general, the module names have been changed so that `AzureRM` and `Azure` become `Az`, and the same for cmdlets.</span></span>
<span data-ttu-id="2ea97-141">예를 들어, `AzureRM.Compute` 모듈의 이름이 `Az.Compute`로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-141">For example, the `AzureRM.Compute` module has been renamed to `Az.Compute`.</span></span> <span data-ttu-id="2ea97-142">`New-AzureRMVM`은 `New-AzVM`이 되고 `Get-AzureStorageBlob`은 이제 `Get-AzStorageBlob`입니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-142">`New-AzureRMVM` has become `New-AzVM`, and `Get-AzureStorageBlob` is now `Get-AzStorageBlob`.</span></span>

<span data-ttu-id="2ea97-143">이 이름 변경에는 알아야 할 예외 사항이 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-143">There are exceptions to this naming change that you should be aware of.</span></span> <span data-ttu-id="2ea97-144">`AzureRM` 또는 `Azure`를 `Az`로 변경하는 것 이외에 일부 cmdlet의 접미사에 영향을 주지 않고 일부 모듈의 이름을 바꾸거나 기존 모듈에 병합했습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-144">Some modules were renamed or merged into existing modules without this affecting the suffix of their cmdlets, other than changing `AzureRM` or `Azure` to `Az`.</span></span> <span data-ttu-id="2ea97-145">또는 전체 cmdlet 접미사가 새로운 모듈 이름을 반영하도록 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-145">Otherwise, the full cmdlet suffix was changed to reflect the new module name.</span></span>

| <span data-ttu-id="2ea97-146">AzureRM 모듈</span><span class="sxs-lookup"><span data-stu-id="2ea97-146">AzureRM module</span></span> | <span data-ttu-id="2ea97-147">Az 모듈</span><span class="sxs-lookup"><span data-stu-id="2ea97-147">Az module</span></span> | <span data-ttu-id="2ea97-148">Cmdlet 접미사가 변경되었습니까?</span><span class="sxs-lookup"><span data-stu-id="2ea97-148">Cmdlet suffix changed?</span></span> |
|----------------|-----------|------------------------|
| <span data-ttu-id="2ea97-149">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2ea97-149">AzureRM.Profile</span></span> | <span data-ttu-id="2ea97-150">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2ea97-150">Az.Accounts</span></span> | <span data-ttu-id="2ea97-151">예</span><span class="sxs-lookup"><span data-stu-id="2ea97-151">Yes</span></span> |
| <span data-ttu-id="2ea97-152">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="2ea97-152">AzureRM.Insights</span></span> | <span data-ttu-id="2ea97-153">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2ea97-153">Az.Monitor</span></span> | <span data-ttu-id="2ea97-154">예</span><span class="sxs-lookup"><span data-stu-id="2ea97-154">Yes</span></span> |
| <span data-ttu-id="2ea97-155">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="2ea97-155">AzureRM.DataFactories</span></span> | <span data-ttu-id="2ea97-156">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2ea97-156">Az.DataFactory</span></span> | <span data-ttu-id="2ea97-157">예</span><span class="sxs-lookup"><span data-stu-id="2ea97-157">Yes</span></span> |
| <span data-ttu-id="2ea97-158">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="2ea97-158">AzureRM.DataFactoryV2</span></span> | <span data-ttu-id="2ea97-159">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2ea97-159">Az.DataFactory</span></span> | <span data-ttu-id="2ea97-160">예</span><span class="sxs-lookup"><span data-stu-id="2ea97-160">Yes</span></span> |
| <span data-ttu-id="2ea97-161">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="2ea97-161">AzureRM.RecoveryServices.Backup</span></span> | <span data-ttu-id="2ea97-162">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2ea97-162">Az.RecoveryServices</span></span> | <span data-ttu-id="2ea97-163">아니요</span><span class="sxs-lookup"><span data-stu-id="2ea97-163">No</span></span> |
| <span data-ttu-id="2ea97-164">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="2ea97-164">AzureRM.RecoveryServices.SiteRecovery</span></span> | <span data-ttu-id="2ea97-165">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2ea97-165">Az.RecoveryServices</span></span> | <span data-ttu-id="2ea97-166">아니요</span><span class="sxs-lookup"><span data-stu-id="2ea97-166">No</span></span> |
| <span data-ttu-id="2ea97-167">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="2ea97-167">AzureRM.Tags</span></span> | <span data-ttu-id="2ea97-168">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2ea97-168">Az.Resources</span></span> | <span data-ttu-id="2ea97-169">아니요</span><span class="sxs-lookup"><span data-stu-id="2ea97-169">No</span></span> |
| <span data-ttu-id="2ea97-170">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="2ea97-170">AzureRM.MachineLearningCompute</span></span> | <span data-ttu-id="2ea97-171">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="2ea97-171">Az.MachineLearning</span></span> | <span data-ttu-id="2ea97-172">아니요</span><span class="sxs-lookup"><span data-stu-id="2ea97-172">No</span></span> |
| <span data-ttu-id="2ea97-173">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="2ea97-173">AzureRM.UsageAggregates</span></span> | <span data-ttu-id="2ea97-174">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="2ea97-174">Az.Billing</span></span> | <span data-ttu-id="2ea97-175">아니요</span><span class="sxs-lookup"><span data-stu-id="2ea97-175">No</span></span> |
| <span data-ttu-id="2ea97-176">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="2ea97-176">AzureRM.Consumption</span></span> | <span data-ttu-id="2ea97-177">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="2ea97-177">Az.Billing</span></span> | <span data-ttu-id="2ea97-178">아니요</span><span class="sxs-lookup"><span data-stu-id="2ea97-178">No</span></span> |

## <a name="summary"></a><span data-ttu-id="2ea97-179">요약</span><span class="sxs-lookup"><span data-stu-id="2ea97-179">Summary</span></span>

<span data-ttu-id="2ea97-180">이 단계를 따르면 기존 스크립트를 모두 업데이트하여 새 모듈을 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2ea97-180">By following these steps, you can update all of your existing scripts to use the new module.</span></span> <span data-ttu-id="2ea97-181">마이그레이션을 어렵게 하는 이들 단계에 대해 질문이나 문제가 있는 경우 지침을 개선할 수 있도록 이 문서에 의견을 남겨주세요.</span><span class="sxs-lookup"><span data-stu-id="2ea97-181">If you have any questions or problems with these steps that made your migration difficult, please comment on this article so that we can improve the instructions.</span></span>
