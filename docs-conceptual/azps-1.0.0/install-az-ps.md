---
title: PowerShellGet으로 Azure PowerShell 설치
description: PowerShellGet으로 Azure PowerShell을 설치 하는 방법
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 828fa8cb2aabac893c566fb146d00af04b16b479
ms.sourcegitcommit: 6685809f054203bd733c84f68acc69e53e5cca8c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/02/2019
ms.locfileid: "53982929"
---
# <a name="install-the-azure-powershell-module"></a><span data-ttu-id="d6580-103">Azure PowerShell 모듈 설치</span><span class="sxs-lookup"><span data-stu-id="d6580-103">Install the Azure PowerShell module</span></span>

<span data-ttu-id="d6580-104">이 문서에서는 PowerShellGet을 사용하여 Azure PowerShell 모듈을 설치하는 방법을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="d6580-105">이러한 지침은 Windows, macOS 및 Linux 플랫폼에서 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="d6580-106">Az 모듈에 대해 현재 다른 설치 방법은 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-106">For the Az module, currently no other installation methods are supported.</span></span>

## <a name="requirements"></a><span data-ttu-id="d6580-107">요구 사항</span><span class="sxs-lookup"><span data-stu-id="d6580-107">Requirements</span></span>

<span data-ttu-id="d6580-108">Azure PowerShell은 Windows 7 이상의 PowerShell 5.x 또는 모든 플랫폼의 PowerShell 6.x에서 작동합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-108">Azure PowerShell works with PowerShell 5.x on Windows 7 or higher, or PowerShell 6.x on any platform.</span></span>
<span data-ttu-id="d6580-109">PowerShell 버전을 확인하려면 다음 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-109">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="d6580-110">오래된 버전이 있거나 PowerShell을 설치해야 하는 경우 [다양한 버전의 PowerShell 설치](/powershell/scripting/setup/installing-powershell)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d6580-110">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](/powershell/scripting/setup/installing-powershell).</span></span> <span data-ttu-id="d6580-111">플랫폼에 대한 설치 정보는 해당 페이지에 링크되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-111">Install information for your platform is linked from that page.</span></span>

<span data-ttu-id="d6580-112">Windows에서 PowerShell 5.x를 사용하는 경우 .NET Framework 4.7.2도 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-112">If you are using PowerShell 5.x on Windows, you also need .NET Framework 4.7.2 installed.</span></span> <span data-ttu-id="d6580-113">새 버전의 .NET Framework를 업데이트 또는 설치하는 방법은 [.NET Framework 설치 설명서](/dotnet/framework/install)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-113">For instructions on updating or installing a new version of .NET Framework, see the [.NET Framework installation guide](/dotnet/framework/install).</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="d6580-114">Azure PowerShell 모듈 설치</span><span class="sxs-lookup"><span data-stu-id="d6580-114">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="d6580-115">AzureRM 및 Az 모듈을 동시에 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-115">You can have both the AzureRM and Az modules installed at the same time.</span></span> <span data-ttu-id="d6580-116">모듈을 모두 설치한 후 __별칭을 사용 않 함으로 설정__합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-116">If you have both modules installed, __don't enable aliases__.</span></span>
> <span data-ttu-id="d6580-117">별칭을 사용하도록 설정하면 AzureRM cmdlet 및 Az 명령 별칭 간의 충돌이 발생하여 예기치 않은 동작이 발생할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-117">Enabling aliases will cause conflicts between AzureRM cmdlets and Az command aliases, and could cause unexpected behavior.</span></span>
> <span data-ttu-id="d6580-118">Az 모듈을 설치하기 전에 AzureRM을 제거하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-118">It's recommended that before installing the Az module, you uninstall AzureRM.</span></span> <span data-ttu-id="d6580-119">항상 AzureRM을 제거할 수 있으며 또는 언제든지 별칭을 사용하도록 설정할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-119">You can always uninstall AzureRM or enable aliases at any time.</span></span> <span data-ttu-id="d6580-120">AzureRM 명령 별칭을 알아보려면 [AzureRM에서 Az로 마이그레이션](migrate-from-azurerm-to-az.md)을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-120">To learn about the AzureRM command aliases, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
> <span data-ttu-id="d6580-121">제거 방법은 [AzureRM 모듈 제거](uninstall-az-ps.md#uninstall-the-azurerm-module)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d6580-121">For uninstall instructions, see [Uninstall the AzureRM module](uninstall-az-ps.md#uninstall-the-azurerm-module).</span></span> 

<span data-ttu-id="d6580-122">모듈을 전역 범위에 설치하려면 상승된 권한으로 PowerShell 갤러리에서 모듈을 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-122">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="d6580-123">Azure PowerShell을 설치하려면 상승된 세션에서 다음 명령을 실행합니다(Windows에서는 "관리자 권한으로 실행", macOS 또는 Linux에서는 슈퍼 사용자 권한으로 실행).</span><span class="sxs-lookup"><span data-stu-id="d6580-123">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="d6580-124">관리자 권한에 대한 액세스 권한이 없으면 `-Scope` 인수를 추가하여 현재 사용자를 위해 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-124">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="d6580-125">기본적으로 PowerShell 갤러리는 PowerShellGet에 대한 신뢰할 수 있는 리포지토리로 구성되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-125">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="d6580-126">PSGallery를 처음 사용할 때는 다음과 같은 메시지가 표시됩니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-126">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="d6580-127">설치를 계속하려면 `Yes` 또는 `Yes to All`로 답변합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-127">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="d6580-128">Az 모듈은 Azure PowerShell cmdlet의 롤업 모듈입니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-128">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="d6580-129">설치하면 사용 가능한 모든 Azure Resource Manager 모듈이 다운로드되고 cmdlet을 사용할 수 있게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-129">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="d6580-130">로그인</span><span class="sxs-lookup"><span data-stu-id="d6580-130">Sign in</span></span>

<span data-ttu-id="d6580-131">Azure PowerShell을 사용하여 작업을 시작하려면 Azure 자격 증명으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-131">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="d6580-132">모듈 자동 로딩을 비활성화한 경우 `Import-Module Az`을 사용하여 모듈을 수동으로 가져와야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-132">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="d6580-133">모듈 구조화 방식으로 인해 몇 초 정도 걸릴 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-133">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="d6580-134">모든 새 PowerShell 세션에 대해 이러한 단계를 반복해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-134">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="d6580-135">PowerShell 세션 간에 Azure 로그인을 유지하는 방법을 보려면 [PowerShell 세션간에 사용자 자격 증명 유지](context-persistence.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d6580-135">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="d6580-136">Azure PowerShell 모듈 업데이트</span><span class="sxs-lookup"><span data-stu-id="d6580-136">Update the Azure PowerShell module</span></span>

<span data-ttu-id="d6580-137">[Update-Module](/powershell/module/powershellget/update-module)을 실행하여 Azure PowerShell 설치를 업데이트할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-137">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="d6580-138">이 명령은 이전 버전을 제거하지 __않습니다__.</span><span class="sxs-lookup"><span data-stu-id="d6580-138">This command does __not__ uninstall older versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="d6580-139">Azure PowerShell의 이전 버전을 시스템에서 제거하는 방법을 알아보려면, [Azure PowerShell 모듈 제거](uninstall-az-ps.md)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-139">To learn how to remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="d6580-140">여러 버전의 Azure PowerShell 사용</span><span class="sxs-lookup"><span data-stu-id="d6580-140">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="d6580-141">Azure PowerShell은 버전을 2개 이상 설치할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-141">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="d6580-142">여러 버전의 Azure PowerShell이 설치되어 있는지 확인하려면 다음 명령을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-142">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

<span data-ttu-id="d6580-143">Azure PowerShell의 버전을 제거하려면 [Azure PowerShell 모듈 제거](uninstall-az-ps.md)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-143">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="d6580-144">`-RequiredVersion` 인수를 사용하여 `Az` 모듈의 특정 버전을 설치하거나 로드할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-144">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` argument:</span></span>

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

<span data-ttu-id="d6580-145">모듈 버전이 두 개 이상인 경우 모듈 자동 로드 및 `Import-Module`이 기본적으로 최신 버전을 로드합니다.</span><span class="sxs-lookup"><span data-stu-id="d6580-145">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="d6580-146">피드백 제공</span><span class="sxs-lookup"><span data-stu-id="d6580-146">Provide feedback</span></span>

<span data-ttu-id="d6580-147">Azure Powershell에서 버그 발생 시, [ GitHub에서 문제를 제출](https://github.com/Azure/azure-powershell/issues)하세요.</span><span class="sxs-lookup"><span data-stu-id="d6580-147">If you find a bug in Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="d6580-148">명령줄에서 피드백을 제공하려면 [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="d6580-148">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d6580-149">다음 단계</span><span class="sxs-lookup"><span data-stu-id="d6580-149">Next Steps</span></span>

<span data-ttu-id="d6580-150">Azure PowerShell 모듈 및 모듈의 기능에 대해 자세히 알아보려면, [Azure PowerShell 시작](get-started-azureps.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d6580-150">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>
<span data-ttu-id="d6580-151">Azure PowerShell에 익숙하고 AzureRM에서 마이그레이션해야 하는 경우 [AzureRM에서 Az로 마이그레이션](migrate-from-azurerm-to-az.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="d6580-151">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
