---
title: Azure Stack Admin PowerShell 개요 | Microsoft Docs
description: 설치 및 구성에 대한 설명을 포함한 Azure Stack Admin PowerShell 개요입니다.
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 02/06/2019
ms.openlocfilehash: af0343e5ad92fa7f2b5c10e3e67cb7e10feb81c6
ms.sourcegitcommit: 0fdccb57a356b6e7c35a77b1f76e01fb96ef582b
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/17/2019
ms.locfileid: "65855791"
---
# <a name="azure-stack-module-172"></a><span data-ttu-id="8044c-103">Azure Stack 모듈 1.7.2</span><span class="sxs-lookup"><span data-stu-id="8044c-103">Azure Stack Module 1.7.2</span></span>

## <a name="requirements"></a><span data-ttu-id="8044c-104">Requirements:</span><span class="sxs-lookup"><span data-stu-id="8044c-104">Requirements:</span></span>

<span data-ttu-id="8044c-105">지원되는 최소 Azure Stack 버전은 1904입니다.</span><span class="sxs-lookup"><span data-stu-id="8044c-105">Minimum supported Azure Stack version is 1904.</span></span>

<span data-ttu-id="8044c-106">참고: 이전 버전의 Azure Stack인 경우 [Azure Stack Powershell 설치](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="8044c-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install-powershell-for-azure-stack"></a><span data-ttu-id="8044c-107">Azure Stack용 PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="8044c-107">Install PowerShell for Azure Stack</span></span>

<span data-ttu-id="8044c-108">설치에는 다음 세 가지 단계가 있습니다.</span><span class="sxs-lookup"><span data-stu-id="8044c-108">Installation has three steps:</span></span>

1. <span data-ttu-id="8044c-109">Azure Stack 버전에 따라 Azure Stack PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="8044c-109">Install Azure Stack PowerShell depending on your version of Azure Stack</span></span>
2. <span data-ttu-id="8044c-110">추가 스토리지 기능을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="8044c-110">Enable additional storage features</span></span>
3. <span data-ttu-id="8044c-111">PowerShell 설치 확인</span><span class="sxs-lookup"><span data-stu-id="8044c-111">Confirm the installation of PowerShell</span></span>

### <a name="install-azure-stack-powershell"></a><span data-ttu-id="8044c-112">Azure Stack PowerShell 설치</span><span class="sxs-lookup"><span data-stu-id="8044c-112">Install Azure Stack PowerShell</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install the AzureRM.BootStrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRM.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Get-AzureRmProfile -Update
Use-AzureRmProfile -Profile 2019-03-01-hybrid -Force
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

### <a name="enable-additional-storage-features"></a><span data-ttu-id="8044c-113">추가 스토리지 기능을 사용하도록 설정</span><span class="sxs-lookup"><span data-stu-id="8044c-113">Enable additional storage features</span></span>

```
# Install the Azure.Storage module version 4.5.0
Install-Module -Name Azure.Storage -RequiredVersion 4.5.0 -Force -AllowClobber

# Install the AzureRm.Storage module version 5.0.4
Install-Module -Name AzureRM.Storage -RequiredVersion 5.0.4 -Force -AllowClobber

# Remove incompatible storage module installed by AzureRM.Storage
Uninstall-Module Azure.Storage -RequiredVersion 4.6.1 -Force

# Load the modules explicitly specifying the versions
Import-Module -Name Azure.Storage -RequiredVersion 4.5.0
Import-Module -Name AzureRM.Storage -RequiredVersion 5.0.4
```

## <a name="release-notes"></a><span data-ttu-id="8044c-114">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="8044c-114">Release Notes</span></span>

* <span data-ttu-id="8044c-115">1904 업데이트 지원</span><span class="sxs-lookup"><span data-stu-id="8044c-115">Supported with 1904 update</span></span>
* <span data-ttu-id="8044c-116">이는 호환성이 손상되는 변경 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="8044c-116">This a breaking change release.</span></span> <span data-ttu-id="8044c-117">호환성이 손상되는 변경에 대한 자세한 내용은 <https://aka.ms/azspshmigration170>를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="8044c-117">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="8044c-118">Azs.Backup.Admin 모듈 \* 호환성이 손상되는 변경: Backup이 인증서 기반 암호화 모드로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="8044c-118">Azs.Backup.Admin Module \* Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="8044c-119">대칭 키에 대한 지원은 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="8044c-119">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="8044c-120">Azs.Fabric.Admin 모듈 \* 사용 중단 \* Get-AzsInfrastructureVolume은 더 이상 사용되지 않으며, 새 cmdlet Get-AzsVolume이 제공됩니다. \* Get-AzsStorageSystem은 더 이상 사용되지 않으며, 새 cmdlet Get-AzsStorageSubSystem이 제공됩니다. \* Get-AzsStoragePool은 더 이상 사용되지 않으며, StorageSubSystem 개체가 용량 속성을 갖습니다.</span><span class="sxs-lookup"><span data-stu-id="8044c-120">Azs.Fabric.Admin Module       \* Deprecation           \* Get-AzsInfrastructureVolume has been deprecated, we provide new cmdlet Get-AzsVolume           \* Get-AzsStorageSystem has been deprecated, we provide new cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool has been deprecated, the StorageSubSystem object has the capacity property</span></span>
* <span data-ttu-id="8044c-121">Azs.Compute.Admin 모듈           \* 버그 수정: Add-AzsPlatformImage, Get-AzsPlatformImage: 성공 경로에서만 ConvertTo-PlatformImageObject 호출           \* 버그 수정: Add-AzsVmExtension, Get-AzsVmExtension: 성공 경로에서만 ConvertTo-VmExtensionObject 호출</span><span class="sxs-lookup"><span data-stu-id="8044c-121">Azs.Compute.Admin Module           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Calling ConvertTo-PlatformImageObject only in the success path           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Calling ConvertTo-VmExtensionObject only in the success path</span></span>
* <span data-ttu-id="8044c-122">Azs.Storage.Admin 모듈 \* 버그 수정 - 새 스토리지 할당량이 제공되지 않을 경우 기본값을 사용합니다.'</span><span class="sxs-lookup"><span data-stu-id="8044c-122">Azs.Storage.Admin Module           \* Bug fix - New Storage Quota uses defaults if none provided.'</span></span>
