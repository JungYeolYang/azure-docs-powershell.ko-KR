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
ms.openlocfilehash: 6568dc4e6c51e8f250aad2c4dd765c065fe6a8bf
ms.sourcegitcommit: ae4540a90508db73335a54408dfd6cdf3712a1e9
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/18/2019
ms.locfileid: "58808063"
---
# <a name="azure-stack-module-171"></a><span data-ttu-id="b66ad-103">Azure Stack 모듈 1.7.1</span><span class="sxs-lookup"><span data-stu-id="b66ad-103">Azure Stack Module 1.7.1</span></span>

## <a name="requirements"></a><span data-ttu-id="b66ad-104">Requirements:</span><span class="sxs-lookup"><span data-stu-id="b66ad-104">Requirements:</span></span>

<span data-ttu-id="b66ad-105">최소 지원 Azure Stack 버전은 1901입니다.</span><span class="sxs-lookup"><span data-stu-id="b66ad-105">Minimum supported Azure Stack version is 1901.</span></span>

<span data-ttu-id="b66ad-106">참고: 이전 버전의 Azure Stack인 경우 [Azure Stack Powershell 설치](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)를 확인하세요.</span><span class="sxs-lookup"><span data-stu-id="b66ad-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="b66ad-107">설치</span><span class="sxs-lookup"><span data-stu-id="b66ad-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.4.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.1
```

## <a name="release-notes"></a><span data-ttu-id="b66ad-108">릴리스 정보</span><span class="sxs-lookup"><span data-stu-id="b66ad-108">Release Notes</span></span>

* <span data-ttu-id="b66ad-109">1901 업데이트 지원</span><span class="sxs-lookup"><span data-stu-id="b66ad-109">Supported with 1901 update</span></span>
* <span data-ttu-id="b66ad-110">이는 호환성이 손상되는 변경 릴리스입니다.</span><span class="sxs-lookup"><span data-stu-id="b66ad-110">This a breaking change release.</span></span> <span data-ttu-id="b66ad-111">호환성이 손상되는 변경에 대한 자세한 내용은 <https://aka.ms/azspshmigration170>를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="b66ad-111">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="b66ad-112">Azs.Backup.Admin 모듈 \* 호환성이 손상되는 변경: Backup이 인증서 기반 암호화 모드로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="b66ad-112">Azs.Backup.Admin Module \* Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="b66ad-113">대칭 키에 대한 지원은 사용되지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="b66ad-113">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="b66ad-114">Azs.Fabric.Admin 모듈 \* 사용 중단 \* Get-AzsInfrastructureVolume은 더 이상 사용되지 않으며, 새 cmdlet Get-AzsVolume이 제공됩니다. \* Get-AzsStorageSystem은 더 이상 사용되지 않으며, 새 cmdlet Get-AzsStorageSubSystem이 제공됩니다. \* Get-AzsStoragePool은 더 이상 사용되지 않으며, StorageSubSystem 개체가 용량 속성을 갖습니다.</span><span class="sxs-lookup"><span data-stu-id="b66ad-114">Azs.Fabric.Admin Module       \* Deprecation           \* Get-AzsInfrastructureVolume has been deprecated, we provide new cmdlet Get-AzsVolume           \* Get-AzsStorageSystem has been deprecated, we provide new cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool has been deprecated, the StorageSubSystem object has the capacity property</span></span>
* <span data-ttu-id="b66ad-115">Azs.Compute.Admin 모듈           \* 버그 수정: Add-AzsPlatformImage, Get-AzsPlatformImage: 성공 경로에서만 ConvertTo-PlatformImageObject 호출           \* 버그 수정: Add-AzsVmExtension, Get-AzsVmExtension: 성공 경로에서만 ConvertTo-VmExtensionObject 호출</span><span class="sxs-lookup"><span data-stu-id="b66ad-115">Azs.Compute.Admin Module           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Calling ConvertTo-PlatformImageObject only in the success path           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Calling ConvertTo-VmExtensionObject only in the success path</span></span>
* <span data-ttu-id="b66ad-116">Azs.Storage.Admin 모듈 \* 버그 수정 - 새 스토리지 할당량이 제공되지 않을 경우 기본값을 사용합니다.'</span><span class="sxs-lookup"><span data-stu-id="b66ad-116">Azs.Storage.Admin Module           \* Bug fix - New Storage Quota uses defaults if none provided.'</span></span>
