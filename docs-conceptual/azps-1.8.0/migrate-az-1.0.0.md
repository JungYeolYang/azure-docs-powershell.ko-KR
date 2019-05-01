---
title: Microsoft Azure PowerShell Az 1.0.0의 호환성이 손상되는 변경
description: 이 마이그레이션 가이드에는 Azure PowerShell Az 버전 1 릴리스의 호환성이 손상되는 변경에 대한 목록이 포함되어 있습니다.
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/14/2018
ms.openlocfilehash: be3e19dc4b689adbc63b933dd9f3454122d5344a
ms.sourcegitcommit: 43f4bdf2a59dd82fd881512aa9761bf72eb5703c
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/23/2019
ms.locfileid: "63068849"
---
# <a name="migration-guide-for-az-100"></a><span data-ttu-id="f12e7-103">Az 1.0.0에 대한 마이그레이션 가이드</span><span class="sxs-lookup"><span data-stu-id="f12e7-103">Migration Guide for Az 1.0.0</span></span>

<span data-ttu-id="f12e7-104">이 문서에서는 AzureRM 6.x 버전과 Az 1.0.0 버전 간의 변경 내용을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-104">This document describes the changes between the 6.x versions of AzureRM and Az version 1.0.0.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="f12e7-105">목차</span><span class="sxs-lookup"><span data-stu-id="f12e7-105">Table of Contents</span></span>
- [<span data-ttu-id="f12e7-106">일반적인 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="f12e7-106">General breaking changes</span></span>](#general-breaking-changes)
  - [<span data-ttu-id="f12e7-107">Cmdlet 명사 접두사 변경</span><span class="sxs-lookup"><span data-stu-id="f12e7-107">Cmdlet Noun Prefix Changes</span></span>](#cmdlet-noun-prefix-changes)
  - [<span data-ttu-id="f12e7-108">모듈 이름 변경</span><span class="sxs-lookup"><span data-stu-id="f12e7-108">Module name changes</span></span>](#module-name-changes)
  - [<span data-ttu-id="f12e7-109">제거된 모듈</span><span class="sxs-lookup"><span data-stu-id="f12e7-109">Removed modules</span></span>](#removed-modules)
  - [<span data-ttu-id="f12e7-110">Windows PowerShell 5.1 및 .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="f12e7-110">Windows PowerShell 5.1 and .NET 4.7.2</span></span>](#windows-powershell-51-and-net-472)
  - [<span data-ttu-id="f12e7-111">PSCredential을 사용하여 사용자 로그인 임시 제거</span><span class="sxs-lookup"><span data-stu-id="f12e7-111">Temporary removal of User login using PSCredential</span></span>](#temporary-removal-of-user-login-using-pscredential)
  - [<span data-ttu-id="f12e7-112">웹 브라우저 프롬프트 대신 기본 디바이스 코드 로그인</span><span class="sxs-lookup"><span data-stu-id="f12e7-112">Default Device Code login instead of Web Browser prompt</span></span>](#temporary-default-device-code-login-instead-of-web-browser-prompt)
- [<span data-ttu-id="f12e7-113">모듈의 호환성이 손상되는 변경</span><span class="sxs-lookup"><span data-stu-id="f12e7-113">Module breaking changes</span></span>](#module-breaking-changes)
  - [<span data-ttu-id="f12e7-114">Az.ApiManagement(이전에는 AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="f12e7-114">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>](#azapimanagement-previously-azurermapimanagement)
  - [<span data-ttu-id="f12e7-115">Az.Billing(이전에는 AzureRM.Billing, AzureRM.Consumption, 및 AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="f12e7-115">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [<span data-ttu-id="f12e7-116">Az.CognitiveServices(이전에는 AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="f12e7-116">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>](#azcognitiveservices-previously-azurermcognitiveservices)
  - [<span data-ttu-id="f12e7-117">Az.Compute(이전에는 AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="f12e7-117">Az.Compute (previously AzureRM.Compute)</span></span>](#azcompute-previously-azurermcompute)
  - [<span data-ttu-id="f12e7-118">Az.DataFactory(이전에는 AzureRM.DataFactories 및 AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="f12e7-118">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [<span data-ttu-id="f12e7-119">Az.DataLakeAnalytics(이전에는 AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="f12e7-119">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [<span data-ttu-id="f12e7-120">Az.DataLakeStore(이전에는 AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="f12e7-120">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>](#azdatalakestore-previously-azurermdatalakestore)
  - [<span data-ttu-id="f12e7-121">Az.KeyVault(이전에는 AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="f12e7-121">Az.KeyVault (previously AzureRM.KeyVault)</span></span>](#azkeyvault-previously-azurermkeyvault)
  - [<span data-ttu-id="f12e7-122">Az.Media(이전에는 AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="f12e7-122">Az.Media (previously AzureRM.Media)</span></span>](#azmedia-previously-azurermmedia)
  - [<span data-ttu-id="f12e7-123">Az.Monitor(이전에는 AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="f12e7-123">Az.Monitor (previously AzureRM.Insights)</span></span>](#azmonitor-previously-azurerminsights)
  - [<span data-ttu-id="f12e7-124">Az.Network(이전에는 AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="f12e7-124">Az.Network (previously AzureRM.Network)</span></span>](#aznetwork-previously-azurermnetwork)
  - [<span data-ttu-id="f12e7-125">Az.OperationalInsights(이전에는 AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="f12e7-125">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>](#azoperationalinsights-previously-azurermoperationalinsights)
  - [<span data-ttu-id="f12e7-126">Az.RecoveryServices(이전에는 AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, 및 AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="f12e7-126">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [<span data-ttu-id="f12e7-127">Az.Resources(이전에는 AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="f12e7-127">Az.Resources (previously AzureRM.Resources)</span></span>](#azresources-previously-azurermresources)
  - [<span data-ttu-id="f12e7-128">Az.ServiceFabric(이전에는 AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="f12e7-128">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>](#azservicefabric-previously-azurermservicefabric)
  - [<span data-ttu-id="f12e7-129">Az.Sql(이전에는 AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="f12e7-129">Az.Sql (previously AzureRM.Sql)</span></span>](#azsql-previously-azurermsql)
  - [<span data-ttu-id="f12e7-130">Az.Storage(이전에는 Azure.Storage 및 AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="f12e7-130">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>](#azstorage-previously-azurestorage-and-azurermstorage)
  - [<span data-ttu-id="f12e7-131">Az.Websites(이전에는 AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="f12e7-131">Az.Websites (previously AzureRM.Websites)</span></span>](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a><span data-ttu-id="f12e7-132">일반적인 주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="f12e7-132">General breaking changes</span></span>
### <a name="cmdlet-noun-prefix-changes"></a><span data-ttu-id="f12e7-133">Cmdlet 명사 접두사 변경</span><span class="sxs-lookup"><span data-stu-id="f12e7-133">Cmdlet Noun Prefix Changes</span></span>
<span data-ttu-id="f12e7-134">AzureRM에서는 cmdlet 명사 접두사로 'AzureRM' 또는 'Azure'를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-134">In AzureRM, cmdlets used either 'AzureRM' or 'Azure' as a noun prefix.</span></span>  <span data-ttu-id="f12e7-135">Az는 cmndlet 이름을 단순화하고 정규화하여 모든 cmdlet이 'Az'를 cmdlet 명사 접두사로 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-135">Az simplifies and normalizes cmndlet names, so that all cmdlets use 'Az' as their cmdlet noun prefix.</span></span> <span data-ttu-id="f12e7-136">예: </span><span class="sxs-lookup"><span data-stu-id="f12e7-136">For example:</span></span>
```powershell
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

<span data-ttu-id="f12e7-137">다음으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-137">Have changed to</span></span>
```powershell
Get-AzVM
Get-AzKeyVaultSecret
```

<span data-ttu-id="f12e7-138">이러한 새 cmdlet 이름으로의 전환을 보다 간단하게 만들기 위해 Az는 두 가지 새로운 cmdlet인 ```Enable-AzureRmAlias```와 ```Disable-AzureRmAlias```를 도입했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-138">To make the transition to these new cmdlet names simpler, Az introduces two new cmdlets, ```Enable-AzureRmAlias``` and ```Disable-AzureRmAlias```.</span></span>  <span data-ttu-id="f12e7-139">```Enable-AzureRmAlias```는 AzureRM의 이전 cmdlet 이름에서 최신 Az cmdlet 이름의 별칭을 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-139">```Enable-AzureRmAlias``` creates aliases from the older cmdlet names in AzureRM to the newer Az cmdlet names.</span></span>  <span data-ttu-id="f12e7-140">cmdlet을 사용하면 사용자 또는 컴퓨터 프로필을 변경하여 현재 세션에서 또는 모든 세션에서 별칭을 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-140">The cmdlet allows creating aliases in the current session, or across all sessions by changing your user or machine profile.</span></span> 

<span data-ttu-id="f12e7-141">예를 들어, AzureRM의 다음 스크립트가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-141">For example, the following script in AzureRM:</span></span>
```powershell
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="f12e7-142">```Enable-AzureRmAlias```를 사용하여 최소한의 변경으로 실행할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-142">Could be run with minimal changes using ```Enable-AzureRmAlias```:</span></span>
```powershell
#Requires -Modules Az.Storage
Enable-AzureRmAlias
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="f12e7-143">```Enable-AzureRmAlias -Scope CurrentUser```를 실행하면 열려 있는 모든 powershell 세션의 별칭이 활성화되므로 이 cmdlet을 실행한 후 이와 같은 스크립트를 변경할 필요가 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-143">Running ```Enable-AzureRmAlias -Scope CurrentUser``` will enable the aliases for all powershell sessions you open, so that after executing this cmdlet, a script like this would not need to be changed at all:</span></span>
```powershell
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="f12e7-144">별칭 cmdlet 사용에 대한 자세한 내용은 powershell 프롬프트에서 ```Get-Help -Online Enable-AzureRmAlias```를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-144">For complete details on the usage of the alias cmdlets, execute ```Get-Help -Online Enable-AzureRmAlias``` from the powershell prompt.</span></span>

<span data-ttu-id="f12e7-145">```Disable-AzureRmAlias```는 ```Enable-AzureRmAlias```로 만든 AzureRM cmdlet 별칭을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-145">```Disable-AzureRmAlias``` removes AzureRM cmdlet aliases created by ```Enable-AzureRmAlias```.</span></span>  <span data-ttu-id="f12e7-146">자세한 내용은 powershell 프롬프트에서 ```Get-Help -Online Disable-AzureRmAlias```를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-146">For complete details, execute ```Get-Help -Online Disable-AzureRmAlias``` from the powershell prompt.</span></span>

### <a name="module-name-changes"></a><span data-ttu-id="f12e7-147">모듈 이름 변경</span><span class="sxs-lookup"><span data-stu-id="f12e7-147">Module Name Changes</span></span>
- <span data-ttu-id="f12e7-148">다음 모듈을 제외하고 모듈 이름이 `AzureRM.*`에서 `Az.*`로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-148">The module names have changed from `AzureRM.*` to `Az.*`, except for the following modules:</span></span>
```
AzureRM.Profile                       -> Az.Accounts
Azure.AnalysisServices                -> Az.AnalysisServices
AzureRM.Consumption                   -> Az.Billing
AzureRM.UsageAggregates               -> Az.Billing
AzureRM.DataFactories                 -> Az.DataFactory
AzureRM.DataFactoryV2                 -> Az.DataFactory
AzureRM.MachineLearningCompute        -> Az.MachineLearning
AzureRM.Insights                      -> Az.Monitor
AzureRM.RecoveryServices.Backup       -> Az.RecoveryServices
AzureRM.RecoveryServices.SiteRecovery -> Az.RecoveryServices
AzureRM.Tags                          -> Az.Resources
Azure.Storage                         -> Az.Storage
```

<span data-ttu-id="f12e7-149">모듈 이름이 변경되면 ```#Requires``` 또는 ```Import-Module```을 사용하여 특정 모듈을 로드하는 스크립트는 대신 새 모듈을 사용하도록 변경되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-149">The changes in module names mean that any script that uses ```#Requires``` or ```Import-Module``` to load specific modules will need to be changed to use the new module instead.</span></span>

#### <a name="migrating-requires-statements"></a><span data-ttu-id="f12e7-150">#Requires 문 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="f12e7-150">Migrating #Requires Statements</span></span>
<span data-ttu-id="f12e7-151">#Requires를 사용하여 AzureRM 모듈에 대한 의존성을 선언하는 스크립트는 새 모듈 이름을 사용하도록 업데이트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-151">Scripts that use #Requires to declare a dependency on AzureRM modules should be updated to use the new module names</span></span>
```powershell
#Requires -Module AzureRM.Compute
```

<span data-ttu-id="f12e7-152">다음과 같이 변경되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-152">Should be changed to</span></span>
```powershell
#Requires -Module Az.Compute
```

#### <a name="migrating-import-module-statements"></a><span data-ttu-id="f12e7-153">모듈 가져오기 문 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="f12e7-153">Migrating Import-Module Statements</span></span>
<span data-ttu-id="f12e7-154">```Import-Module```을 사용하여 AzureRM 모듈을 로드하는 스크립트는 새 모듈 이름을 반영하도록 업데이트해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-154">Scripts that use ```Import-Module``` to load AzureRM modules will need to be updated to reflect the new module names.</span></span>
```powershell
Import-Module -Name AzureRM.Compute
```

<span data-ttu-id="f12e7-155">다음과 같이 변경되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-155">Should be changed to</span></span>
```powershell
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a><span data-ttu-id="f12e7-156">Cmdlet 정규화 호출 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="f12e7-156">Migrating Fully-Qualified Cmdlet Invocations</span></span>
<span data-ttu-id="f12e7-157">다음과 같이 모듈 규정 cmdlet 호출을 사용하는 스크립트</span><span class="sxs-lookup"><span data-stu-id="f12e7-157">Scripts that use module-qualified cmdlet invocations, like</span></span>
```powershell
AzureRM.Compute\Get-AzureRmVM
```

<span data-ttu-id="f12e7-158">새 모듈 및 cmdlet 이름을 사용하도록 변경되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-158">Should be changed to use the new module and cmdlet names</span></span>
```powershell
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a><span data-ttu-id="f12e7-159">모듈 매니페스트 종속성 마이그레이션</span><span class="sxs-lookup"><span data-stu-id="f12e7-159">Migrating Module Manifest Dependencies</span></span>
<span data-ttu-id="f12e7-160">모듈 매니페스트(.psd1) 파일을 통해 AzureRM 모듈에 대한 종속성을 나타내는 모듈은 'RequiredModules'섹션에서 모듈 이름을 업데이트해야 합니다</span><span class="sxs-lookup"><span data-stu-id="f12e7-160">Modules that express dependencies on AzureRM modules through a module manifest (.psd1) file will need to updated the module names in their 'RequiredModules' section</span></span>

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

<span data-ttu-id="f12e7-161">다음과 같이 변경되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-161">Should be changed to</span></span>

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a><span data-ttu-id="f12e7-162">제거된 모듈</span><span class="sxs-lookup"><span data-stu-id="f12e7-162">Removed modules</span></span>
- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

<span data-ttu-id="f12e7-163">이러한 서비스에 대한 도구는 더 이상 지원되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-163">The tooling for these services are no longer actively supported.</span></span>  <span data-ttu-id="f12e7-164">편리한 대체 서비스로 이동하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-164">Customers are encouraged to move to alternative services as soon as it is convenient.</span></span>

### <a name="windows-powershell-51-and-net-472"></a><span data-ttu-id="f12e7-165">Windows PowerShell 5.1 및 .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="f12e7-165">Windows PowerShell 5.1 and .NET 4.7.2</span></span>
- <span data-ttu-id="f12e7-166">Az를 사용 하 여 Windows PowerShell 5.1을 사용하려면 .NET 4.7.2를 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-166">Using Az with Windows PowerShell 5.1 requires the installation of .NET 4.7.2.</span></span> <span data-ttu-id="f12e7-167">PowerShell Core를 사용하여 Az를 사용하려면 .NET 4.7.2가 필요하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-167">However, using Az with PowerShell Core does not require .NET 4.7.2.</span></span> 

### <a name="temporary-removal-of-user-login-using-pscredential"></a><span data-ttu-id="f12e7-168">PSCredential을 사용하여 사용자 로그인 임시 제거</span><span class="sxs-lookup"><span data-stu-id="f12e7-168">Temporary removal of User login using PSCredential</span></span>
- <span data-ttu-id="f12e7-169">.NET 표준의 인증 흐름이 변경되어 PSCredential을 통한 사용자 로그인이 일시적으로 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-169">Due to changes in the authentication flow for .NET Standard, we are temporarily removing user login via PSCredential.</span></span> <span data-ttu-id="f12e7-170">이 기능은 Windows PowerShell 5.1용 2019년 1월 15일 릴리스에서 다시 도입됩니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-170">This capability will be re-introduced in the 1/15/2019 release for Windows PowerShell 5.1.</span></span> <span data-ttu-id="f12e7-171">[이 문제](https://github.com/Azure/azure-powershell/issues/7430)는 자세히 다루고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-171">This is duscussed in detail in [this issue.](https://github.com/Azure/azure-powershell/issues/7430)</span></span>

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a><span data-ttu-id="f12e7-172">웹 브라우저 프롬프트 대신 기본 디바이스 코드 로그인</span><span class="sxs-lookup"><span data-stu-id="f12e7-172">Default Device Code login instead of Web Browser prompt</span></span>
- <span data-ttu-id="f12e7-173">.NET 표준의 인증 흐름이 변경되어 대화식 로그인 중에 기본 로그인 흐름으로 디바이스 로그인을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-173">Due to changes in the authentication flow for .NET Standard, we are using device login as the default login flow during interactive login.</span></span> <span data-ttu-id="f12e7-174">웹 브라우저 기반 로그인은 Windows PowerShell 5.1에서 2019년 1월 15일 릴리스의 기본값으로 다시 도입됩니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-174">Web browser based login will be re-introduced for Windows PowerShell 5.1 as the default in the 1/15/2019 release.</span></span> <span data-ttu-id="f12e7-175">이때 사용자는 스위치 매개 변수를 사용하여 디바이스 로그인을 선택할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-175">At that time, users will be able to choose device login using a Switch parameter.</span></span>

## <a name="module-breaking-changes"></a><span data-ttu-id="f12e7-176">모듈의 호환성이 손상되는 변경</span><span class="sxs-lookup"><span data-stu-id="f12e7-176">Module breaking changes</span></span>

### <a name="azapimanagement-previously-azurermapimanagement"></a><span data-ttu-id="f12e7-177">Az.ApiManagement(이전에는 AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="f12e7-177">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>
- <span data-ttu-id="f12e7-178">다음 cmdlet이 제거됩니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-178">Removing the following cmdlets:</span></span>
  - <span data-ttu-id="f12e7-179">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="f12e7-179">New-AzureRmApiManagementHostnameConfiguration</span></span>
  - <span data-ttu-id="f12e7-180">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="f12e7-180">Set-AzureRmApiManagementHostnames</span></span>
  - <span data-ttu-id="f12e7-181">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="f12e7-181">Update-AzureRmApiManagementDeployment</span></span>
  - <span data-ttu-id="f12e7-182">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="f12e7-182">Import-AzureRmApiManagementHostnameCertificate</span></span>
  - <span data-ttu-id="f12e7-183">이러한 속성 설정을 위해 **Set-AzApiManagement**를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-183">Use **Set-AzApiManagement** cmdlet to set these properites instead</span></span>
- <span data-ttu-id="f12e7-184">다음과 같은 속성이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-184">Following properties were removed</span></span>
  - <span data-ttu-id="f12e7-185">`PsApiManagementContext`에서 `PsApiManagementHostnameConfiguration` 형식의 `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration`, `ScmHostnameConfiguration` 속성을 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-185">Removed property `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` and `ScmHostnameConfiguration` of type `PsApiManagementHostnameConfiguration` from `PsApiManagementContext`.</span></span> <span data-ttu-id="f12e7-186">대신 `PsApiManagementCustomHostNameConfiguration` 형식의 `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration`, `ScmCustomHostnameConfiguration`을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-186">Instead use `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` and `ScmCustomHostnameConfiguration` of type `PsApiManagementCustomHostNameConfiguration`.</span></span>
  - <span data-ttu-id="f12e7-187">PsApiManagementContext에서 `StaticIPs`속성을 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-187">Removed property `StaticIPs` from PsApiManagementContext.</span></span> <span data-ttu-id="f12e7-188">해당 속성은 `PublicIPAddresses`, `PrivateIPAddresses`로 분할되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-188">The property has been split into `PublicIPAddresses` and `PrivateIPAddresses`.</span></span>
  - <span data-ttu-id="f12e7-189">필수 속성 `Location`을 New-AzureApiManagementVirtualNetwork cmdlet에서 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-189">Removed required property `Location` from New-AzureApiManagementVirtualNetwork cmdlet.</span></span>

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a><span data-ttu-id="f12e7-190">Az.Billing(이전에는 AzureRM.Billing, AzureRM.Consumption, 및 AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="f12e7-190">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>
- <span data-ttu-id="f12e7-191">`InvoiceName` 매개 변수가 `Get-AzConsumptionUsageDetail` cmdlet에서 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-191">The `InvoiceName` parameter was removed from the `Get-AzConsumptionUsageDetail` cmdlet.</span></span>  <span data-ttu-id="f12e7-192">스크립트는 청구서에 대한 다른 ID 매개 변수를 사용해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-192">Scripts will need to use other identity parameters for the invoice.</span></span>

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a><span data-ttu-id="f12e7-193">Az.CognitiveServices(이전에는 AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="f12e7-193">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>
- <span data-ttu-id="f12e7-194">`Get-AzCognitiveServicesAccountSkus` cmdlet에서 `GetSkusWithAccountParamSetName` 매개 변수 집합을 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-194">Removed `GetSkusWithAccountParamSetName` parameter set from `Get-AzCognitiveServicesAccountSkus` cmdlet.</span></span>  <span data-ttu-id="f12e7-195">ResourceGroupName 및 계정 이름을 사용하는 대신 계정 형식 및 위치별로 SKU를 가져와야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-195">You must get Skus by Account Type and Location, instead of using ResourceGroupName and Account Name.</span></span>

### <a name="azcompute-previously-azurermcompute"></a><span data-ttu-id="f12e7-196">Az.Compute(이전에는 AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="f12e7-196">Az.Compute (previously AzureRM.Compute)</span></span>
- <span data-ttu-id="f12e7-197">`PSVirtualMachine` 및 `PSVirtualMachineScaleSet` 객체의 `Identity` 속성에서 `IdentityIds`가 제거되었습니다. 스크립트는 더 이상 이 필드의 값을 사용하여 처리 결정을 내려서는 안됩니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-197">`IdentityIds` are removed from `Identity` property in `PSVirtualMachine` and `PSVirtualMachineScaleSet` objects Scripts should no longer use the value of this field to make processing decisions.</span></span>
- <span data-ttu-id="f12e7-198">`PSVirtualMachineScaleSetVM` 개체의 `InstanceView` 속성의 형식이 `VirtualMachineInstanceView`에서 `VirtualMachineScaleSetVMInstanceView`로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-198">The type of `InstanceView` property of `PSVirtualMachineScaleSetVM` object is changed from `VirtualMachineInstanceView` to `VirtualMachineScaleSetVMInstanceView`</span></span>
- <span data-ttu-id="f12e7-199">`UpgradePolicy` 속성에서 `AutoOSUpgradePolicy` 및 `AutomaticOSUpgrade` 속성이 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-199">`AutoOSUpgradePolicy` and `AutomaticOSUpgrade` properties are removed from `UpgradePolicy` property</span></span>
- <span data-ttu-id="f12e7-200">`PSSnapshotUpdate` 개체의 `Sku` 속성의 형식이 `DiskSku`에서 `SnapshotSku`로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-200">The type of `Sku` property in `PSSnapshotUpdate` object is changed from `DiskSku` to `SnapshotSku`</span></span>
- <span data-ttu-id="f12e7-201">`VmScaleSetVMParameterSet`이 `Add-AzVMDataDisk` cmdlet에서 제거되면 더 이상 ScaleSet VM에 개별적으로 데이터 디스크를 추가할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-201">`VmScaleSetVMParameterSet` is removed from `Add-AzVMDataDisk` cmdlet, you cna no longer add a data disk individually to a ScaleSet VM.</span></span>

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a><span data-ttu-id="f12e7-202">Az.DataFactory(이전에는 AzureRM.DataFactories 및 AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="f12e7-202">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>
- <span data-ttu-id="f12e7-203">`GatewayName` 매개 변수가 `New-AzDataFactoryEncryptValue` cmdlet에서 필수 항목이 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-203">The `GatewayName` parameter has become mandatory in the `New-AzDataFactoryEncryptValue` cmdlet</span></span>
- <span data-ttu-id="f12e7-204">`New-AzDataFactoryGatewayKey` cmdlet이 제거됨</span><span class="sxs-lookup"><span data-stu-id="f12e7-204">Removed `New-AzDataFactoryGatewayKey` cmdlet</span></span>
- <span data-ttu-id="f12e7-205">`Get-AzDataFactoryV2ActivityRun` cmdlet에서 `LinkedServiceName` 매개 변수가 제거되었습니다. 스크립트는 더 이상 이 필드의 값을 사용하여 처리 결정을 내려서는 안됩니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-205">Removed `LinkedServiceName` parameter from `Get-AzDataFactoryV2ActivityRun` cmdlet Scripts should no longer use the value of this field to make processing decisions.</span></span>

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a><span data-ttu-id="f12e7-206">Az.DataLakeAnalytics(이전에는 AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="f12e7-206">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>
- <span data-ttu-id="f12e7-207">사용되지 않는 cmdlet 제거: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret`, `Set-AzDataLakeAnalyticsCatalogSecret`</span><span class="sxs-lookup"><span data-stu-id="f12e7-207">Removed deprecated cmdlets: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret`, and `Set-AzDataLakeAnalyticsCatalogSecret`</span></span>

### <a name="azdatalakestore-previously-azurermdatalakestore"></a><span data-ttu-id="f12e7-208">Az.DataLakeStore(이전에는 AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="f12e7-208">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>
- <span data-ttu-id="f12e7-209">다음 cmdlet의 `Encoding` 매개 변수는 `FileSystemCmdletProviderEncoding` 형식에서 `System.Text.Encoding` 형식으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-209">The following cmdlets have had the `Encoding` parameter changed from the type `FileSystemCmdletProviderEncoding` to `System.Text.Encoding`.</span></span> <span data-ttu-id="f12e7-210">이 변경은 인코딩 값 `String` 및 `Oem`을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-210">This change removes the encoding values `String` and `Oem`.</span></span> <span data-ttu-id="f12e7-211">다른 모든 이전 인코딩 값은 유지됩니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-211">All the other prior encoding values remain.</span></span>
  - <span data-ttu-id="f12e7-212">New-AzureRmDataLakeStoreItem</span><span class="sxs-lookup"><span data-stu-id="f12e7-212">New-AzureRmDataLakeStoreItem</span></span>
  - <span data-ttu-id="f12e7-213">Add-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="f12e7-213">Add-AzureRmDataLakeStoreItemContent</span></span>
  - <span data-ttu-id="f12e7-214">Get-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="f12e7-214">Get-AzureRmDataLakeStoreItemContent</span></span>
- <span data-ttu-id="f12e7-215">사용되지 않는 `Tags` 속성 별칭을 `New-AzDataLakeStoreAccount` 및 `Set-AzDataLakeStoreAccount` cmdlet에서 제거함</span><span class="sxs-lookup"><span data-stu-id="f12e7-215">Removed deprecated `Tags` property alias from `New-AzDataLakeStoreAccount` and `Set-AzDataLakeStoreAccount` cmdlets</span></span>

  <span data-ttu-id="f12e7-216">다음을 사용하는 스크립트</span><span class="sxs-lookup"><span data-stu-id="f12e7-216">Scripts using</span></span>
  ```powershell
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="f12e7-217">다음과 같이 변경되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-217">Should be changed to</span></span>
  ```powershell
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- <span data-ttu-id="f12e7-218">```PSDataLakeStoreAccountBasic``` 개체에서 사용되지 않는 속성 ```Identity```, ```EncryptionState```, ```EncrypotionProvisioningState```, ```EncryptionConfig```, ```FirewallState```, ```FirewallRules```, ```VirtualNetworkRules```, ```TrustedIdProviderState```, ```TrustedIdProviders```, ```DefaultGroup```, ```NewTier```, ```CurrentTier```, ```FirewallAllowAzureIps```을 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-218">Removed deprecated properties ```Identity```, ```EncryptionState```, ```EncrypotionProvisioningState```, ```EncryptionConfig```, ```FirewallState```, ```FirewallRules```, ```VirtualNetworkRules```, ```TrustedIdProviderState```, ```TrustedIdProviders```, ```DefaultGroup```, ```NewTier```, ```CurrentTier```, ```FirewallAllowAzureIps``` from ```PSDataLakeStoreAccountBasic``` object.</span></span>  <span data-ttu-id="f12e7-219">```Get-AzDataLakeStoreAccount```에서 반환된 ```PSDatalakeStoreAccount```를 사용하는 모든 스크립트는 이러한 속성을 참조하지 않아야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-219">Any script that uses the ```PSDatalakeStoreAccount``` returned from ```Get-AzDataLakeStoreAccount``` should not reference these properties.</span></span>

### <a name="azkeyvault-previously-azurermkeyvault"></a><span data-ttu-id="f12e7-220">Az.KeyVault(이전에는 AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="f12e7-220">Az.KeyVault (previously AzureRM.KeyVault)</span></span>
- <span data-ttu-id="f12e7-221">`PurgeDisabled` 속성이 `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem` 및 `PSKeyVaultSecretAttributes` 개체에서 제거되었습니다. 스크립트는 더 이상 처리 결정을 내리기 위해 ```PurgeDisabled``` 속성을 참조하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-221">The `PurgeDisabled` property was removed from the `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem`, and `PSKeyVaultSecretAttributes` objects Scripts shoudl no longer reference the ```PurgeDisabled``` property to make processing decisions.</span></span>

### <a name="azmedia-previously-azurermmedia"></a><span data-ttu-id="f12e7-222">Az.Media(이전에는 AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="f12e7-222">Az.Media (previously AzureRM.Media)</span></span>
- <span data-ttu-id="f12e7-223">다음을 사용하여 `New-AzMediaService` cmdlet에서 사용되지 않는 `Tags` 속성 별칭을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-223">Remove deprecated `Tags` property alias from `New-AzMediaService` cmdlet Scripts using</span></span>
  ```powershell
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="f12e7-224">다음과 같이 변경되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-224">Should be changed to</span></span>
  ```powershell
  New-AzMMediaService -Tag @{TagName="TagValue"}
  ```
### <a name="azmonitor-previously-azurerminsights"></a><span data-ttu-id="f12e7-225">Az.Monitor(이전에는 AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="f12e7-225">Az.Monitor (previously AzureRM.Insights)</span></span>
- <span data-ttu-id="f12e7-226">`Set-AzDiagnosticSetting` cmdlet 스크립트에서 다음을 사용하여 단일 매개 변수 이름을 위해 복수 이름 `Categories` 및 `Timegrains` 매개 변수를 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-226">Removed plural names `Categories` and `Timegrains` parameter in favor of singular parameter names from `Set-AzDiagnosticSetting` cmdlet Scripts using</span></span>
  ```powershell
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  <span data-ttu-id="f12e7-227">다음과 같이 변경되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-227">Should be changed to</span></span>
  ```powershell
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```
### <a name="aznetwork-previously-azurermnetwork"></a><span data-ttu-id="f12e7-228">Az.Network(이전에는 AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="f12e7-228">Az.Network (previously AzureRM.Network)</span></span>
- <span data-ttu-id="f12e7-229">사용되지 않는 매개 변수 `ResourceId`를 `Get-AzServiceEndpointPolicyDefinition` cmdlet에서 제거</span><span class="sxs-lookup"><span data-stu-id="f12e7-229">Removed deprecated `ResourceId` parameter from `Get-AzServiceEndpointPolicyDefinition` cmdlet</span></span>
- <span data-ttu-id="f12e7-230">`PSVirtualNetwork` 개체에서 사용되지 않는 속성 `EnableVmProtection`을 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-230">Removed deprecated `EnableVmProtection` property from `PSVirtualNetwork` object</span></span>
- <span data-ttu-id="f12e7-231">사용되지 않는 cmdlet 제거: `Set-AzVirtualNetworkGatewayVpnClientConfig`</span><span class="sxs-lookup"><span data-stu-id="f12e7-231">Removed deprecated `Set-AzVirtualNetworkGatewayVpnClientConfig` cmdlet</span></span>
  
<span data-ttu-id="f12e7-232">스크립트는 더 이상이 필드의 값을 기반으로 처리 결정을 내려서는 안됩니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-232">Scripts shoudl no longer make processing decisions based on the values fo these fields.</span></span>

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a><span data-ttu-id="f12e7-233">Az.OperationalInsights(이전에는 AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="f12e7-233">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>
- <span data-ttu-id="f12e7-234">`Get-AzOperationalInsightsDataSource`에 설정된 기본 매개 변수가 제거되고 `ByWorkspaceNameByKind`가 기본 매개 변수 집합이 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-234">Default parameter set for `Get-AzOperationalInsightsDataSource` is removed, and `ByWorkspaceNameByKind` has become the default parameter set</span></span>

  <span data-ttu-id="f12e7-235">다음을 사용하여 데이터 원본을 나열하는 스크립트</span><span class="sxs-lookup"><span data-stu-id="f12e7-235">Scripts that listed data sources using</span></span>
  ```powershell
  Get-AzureRmOperationalInsightsDataSource
  ```

  <span data-ttu-id="f12e7-236">종류를 지정하도록 변경되어야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-236">Should be changed to specify a Kind</span></span>
  ```powershell
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a><span data-ttu-id="f12e7-237">Az.RecoveryServices(이전에는 AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, 및 AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="f12e7-237">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>
- <span data-ttu-id="f12e7-238">`New/Set-AzRecoveryServicesAsrPolicy` cmdlet에서 `Encryption` 매개 변수를 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-238">Removed `Encryption` parameter from `New/Set-AzRecoveryServicesAsrPolicy` cmdlet</span></span>
- <span data-ttu-id="f12e7-239">`TargetStorageAccountName` 매개 변수는 이제 `Restore-AzRecoveryServicesBackupItem` cmdlet의 관리 디스크 복원에 필수 항목입니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-239">`TargetStorageAccountName` parameter is now mandatory for managed disk restores in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="f12e7-240">`Restore-AzRecoveryServicesBackupItem` cmdlet에서 `StorageAccountName`, `StorageAccountResourceGroupName` 매개 변수 제거</span><span class="sxs-lookup"><span data-stu-id="f12e7-240">Removed `StorageAccountName` and `StorageAccountResourceGroupName` parameters in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="f12e7-241">`Get-AzRecoveryServicesBackupContainer` cmdlet에서 `Name` 매개 변수 제거</span><span class="sxs-lookup"><span data-stu-id="f12e7-241">Removed `Name`parameter in `Get-AzRecoveryServicesBackupContainer` cmdlet</span></span>

### <a name="azresources-previously-azurermresources"></a><span data-ttu-id="f12e7-242">Az.Resources(이전에는 AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="f12e7-242">Az.Resources (previously AzureRM.Resources)</span></span>
- <span data-ttu-id="f12e7-243">`New/Set-AzPolicyAssignment` cmdlet에서 `Sku` 매개 변수를 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-243">Removed `Sku` parameter from `New/Set-AzPolicyAssignment` cmdlet</span></span>
- <span data-ttu-id="f12e7-244">`New-AzADServicePrincipal` 및 `New-AzADSpCredential` cmdlet에서 `Password` 매개 변수를 제거했습니다. 암호는 자동으로 생성되며 암호를 제공하는 스크립트는 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-244">Removed `Password` parameter from `New-AzADServicePrincipal` and `New-AzADSpCredential` cmdlet Passwords are automatically generated, scripts that provided the password:</span></span>
  ```powershell
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  <span data-ttu-id="f12e7-245">출력에서 암호를 검색하도록 변경해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-245">Should be changed to retriedve the password from the output:</span></span>
  ```powershell
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a><span data-ttu-id="f12e7-246">Az.ServiceFabric(이전에는 AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="f12e7-246">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>
- <span data-ttu-id="f12e7-247">다음 cmdlet 반환 형식이 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-247">The following cmdlet return types have been changed:</span></span>
  - <span data-ttu-id="f12e7-248">`ApplicationHealthPolicy` 형식의 속성 `SerivceTypeHealthPolicies`가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-248">The property `SerivceTypeHealthPolicies` of type `ApplicationHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="f12e7-249">`ClusterUpgradeDeltaHealthPolicy` 형식의 속성 `ApplicationHealthPolicies`가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-249">The property `ApplicationHealthPolicies` of type `ClusterUpgradeDeltaHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="f12e7-250">`ClusterUpgradePolicy` 형식의 속성 `OverrideUserUpgradePolicy`가 제거되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-250">The property `OverrideUserUpgradePolicy` of type `ClusterUpgradePolicy` has been removed.</span></span>
  - <span data-ttu-id="f12e7-251">이러한 변경 내용은 다음 cmdlet에 영향을 줍니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-251">These changes affect the following cmdlets:</span></span>
    - <span data-ttu-id="f12e7-252">Add-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="f12e7-252">Add-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="f12e7-253">Add-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="f12e7-253">Add-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="f12e7-254">Add-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="f12e7-254">Add-AzServiceFabricNode</span></span>
    - <span data-ttu-id="f12e7-255">Add-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="f12e7-255">Add-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="f12e7-256">Get-AzServiceFabricCluster</span><span class="sxs-lookup"><span data-stu-id="f12e7-256">Get-AzServiceFabricCluster</span></span>
    - <span data-ttu-id="f12e7-257">Remove-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="f12e7-257">Remove-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="f12e7-258">Remove-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="f12e7-258">Remove-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="f12e7-259">Remove-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="f12e7-259">Remove-AzServiceFabricNode</span></span>
    - <span data-ttu-id="f12e7-260">Remove-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="f12e7-260">Remove-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="f12e7-261">Remove-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="f12e7-261">Remove-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="f12e7-262">Set-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="f12e7-262">Set-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="f12e7-263">Set-AzServiceFabricUpgradeType</span><span class="sxs-lookup"><span data-stu-id="f12e7-263">Set-AzServiceFabricUpgradeType</span></span>
    - <span data-ttu-id="f12e7-264">Update-AzServiceFabricDurability</span><span class="sxs-lookup"><span data-stu-id="f12e7-264">Update-AzServiceFabricDurability</span></span>
    - <span data-ttu-id="f12e7-265">Update-AzServiceFabricReliability</span><span class="sxs-lookup"><span data-stu-id="f12e7-265">Update-AzServiceFabricReliability</span></span>

### <a name="azsql-previously-azurermsql"></a><span data-ttu-id="f12e7-266">Az.Sql(이전에는 AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="f12e7-266">Az.Sql (previously AzureRM.Sql)</span></span>
- <span data-ttu-id="f12e7-267">`Set-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet에서 `State`, `ResourceId` 매개 변수 제거</span><span class="sxs-lookup"><span data-stu-id="f12e7-267">Removed `State` and `ResourceId` parameters from `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="f12e7-268">사용되지 않는 cmdlet 제거: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing`, `Remove-AzSqlServerAuditing`</span><span class="sxs-lookup"><span data-stu-id="f12e7-268">Removed deprecated cmdlets: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing`, `Remove-AzSqlServerAuditing`</span></span>
- <span data-ttu-id="f12e7-269">사용되지 않는 매개 변수 `Current`를 `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet에서 제거</span><span class="sxs-lookup"><span data-stu-id="f12e7-269">Removed deprecated parameter `Current` from `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="f12e7-270">사용되지 않는 매개 변수 `DatabaseName`을 `Get-AzSqlServerServiceObjective` cmdlet에서 제거</span><span class="sxs-lookup"><span data-stu-id="f12e7-270">Removed deprecated parameter `DatabaseName` from `Get-AzSqlServerServiceObjective` cmdlet</span></span>
- <span data-ttu-id="f12e7-271">사용되지 않는 매개 변수 `PrivilegedLogin`을 `Set-AzSqlDatabaseDataMaskingPolicy` cmdlet에서 제거</span><span class="sxs-lookup"><span data-stu-id="f12e7-271">Removed deprecated parameter `PrivilegedLogin` from `Set-AzSqlDatabaseDataMaskingPolicy` cmdlet</span></span>

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a><span data-ttu-id="f12e7-272">Az.Storage(이전에는 Azure.Storage 및 AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="f12e7-272">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>
- <span data-ttu-id="f12e7-273">스토리지 계정 이름만 사용하여 Oauth 스토리지 컨텍스트를 만들 수 있도록 기본 매개 변수 집합이 `OAuthParameterSet`으로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-273">To support creating an Oauth storage context with only the storage account name, the default parameter set has been changed to `OAuthParameterSet`</span></span>
  - <span data-ttu-id="f12e7-274">예제: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span><span class="sxs-lookup"><span data-stu-id="f12e7-274">Example: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span></span>
- <span data-ttu-id="f12e7-275">`Location` 매개 변수가 `Get-AzStorageUsage` cmdlet에서 필수 항목이 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-275">The `Location` parameter has become mandatory in the `Get-AzStorageUsage` cmdlet</span></span>
- <span data-ttu-id="f12e7-276">이제 Storage API 메서드는 동기 API 호출 대신 작업 기반 비동기 패턴(TAP)을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-276">The Storage API methods now use the Task-based Asynchronous Pattern (TAP), instead of synchronous API calls.</span></span>
#### <a name="1-blob-snapshot"></a><span data-ttu-id="f12e7-277">1. BLOB 스냅숏</span><span class="sxs-lookup"><span data-stu-id="f12e7-277">1. Blob Snapshot</span></span>
##### <a name="before"></a><span data-ttu-id="f12e7-278">이전:</span><span class="sxs-lookup"><span data-stu-id="f12e7-278">Before:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

##### <a name="after"></a><span data-ttu-id="f12e7-279">이후:</span><span class="sxs-lookup"><span data-stu-id="f12e7-279">After:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="2-share-snapshot"></a><span data-ttu-id="f12e7-280">2. 스냅숏 공유</span><span class="sxs-lookup"><span data-stu-id="f12e7-280">2. Share Snapshot</span></span>
##### <a name="before"></a><span data-ttu-id="f12e7-281">이전:</span><span class="sxs-lookup"><span data-stu-id="f12e7-281">Before:</span></span>
```powershell
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```
#####  <a name="after"></a><span data-ttu-id="f12e7-282">이후:</span><span class="sxs-lookup"><span data-stu-id="f12e7-282">After:</span></span>
```powershell

$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="3-undelete-a-soft-delete-blob"></a><span data-ttu-id="f12e7-283">3. 일시 삭제 BLOB 삭제 취소</span><span class="sxs-lookup"><span data-stu-id="f12e7-283">3. Undelete a soft delete blob</span></span>
##### <a name="before"></a><span data-ttu-id="f12e7-284">이전:</span><span class="sxs-lookup"><span data-stu-id="f12e7-284">Before:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```
##### <a name="after"></a><span data-ttu-id="f12e7-285">이후:</span><span class="sxs-lookup"><span data-stu-id="f12e7-285">After:</span></span>
```powershell
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="4-set-blob-tier"></a><span data-ttu-id="f12e7-286">4. BLOB 계층 설정</span><span class="sxs-lookup"><span data-stu-id="f12e7-286">4. Set Blob Tier</span></span>
##### <a name="before"></a><span data-ttu-id="f12e7-287">이전:</span><span class="sxs-lookup"><span data-stu-id="f12e7-287">Before:</span></span>
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

##### <a name="after"></a><span data-ttu-id="f12e7-288">이후:</span><span class="sxs-lookup"><span data-stu-id="f12e7-288">After:</span></span>
```powershell
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a><span data-ttu-id="f12e7-289">Az.Websites(이전에는 AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="f12e7-289">Az.Websites (previously AzureRM.Websites)</span></span>
- <span data-ttu-id="f12e7-290">사용되지 않는 속성을 `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo`, `PSSite` 개체에서 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="f12e7-290">Removed deprecated properties from the `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo`, and `PSSite` objects</span></span>