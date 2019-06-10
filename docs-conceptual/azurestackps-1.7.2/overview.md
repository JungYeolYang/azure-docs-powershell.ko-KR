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
# <a name="azure-stack-module-172"></a>Azure Stack 모듈 1.7.2

## <a name="requirements"></a>Requirements:

지원되는 최소 Azure Stack 버전은 1904입니다.

참고: 이전 버전의 Azure Stack인 경우 [Azure Stack Powershell 설치](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)를 확인하세요.

## <a name="install-powershell-for-azure-stack"></a>Azure Stack용 PowerShell 설치

설치에는 다음 세 가지 단계가 있습니다.

1. Azure Stack 버전에 따라 Azure Stack PowerShell 설치
2. 추가 스토리지 기능을 사용하도록 설정
3. PowerShell 설치 확인

### <a name="install-azure-stack-powershell"></a>Azure Stack PowerShell 설치

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

### <a name="enable-additional-storage-features"></a>추가 스토리지 기능을 사용하도록 설정

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

## <a name="release-notes"></a>릴리스 정보

* 1904 업데이트 지원
* 이는 호환성이 손상되는 변경 릴리스입니다. 호환성이 손상되는 변경에 대한 자세한 내용은 <https://aka.ms/azspshmigration170>를 참조하세요.
* Azs.Backup.Admin 모듈 * 호환성이 손상되는 변경: Backup이 인증서 기반 암호화 모드로 변경됩니다. 대칭 키에 대한 지원은 사용되지 않습니다.
* Azs.Fabric.Admin 모듈 * 사용 중단 * Get-AzsInfrastructureVolume은 더 이상 사용되지 않으며, 새 cmdlet Get-AzsVolume이 제공됩니다. * Get-AzsStorageSystem은 더 이상 사용되지 않으며, 새 cmdlet Get-AzsStorageSubSystem이 제공됩니다. * Get-AzsStoragePool은 더 이상 사용되지 않으며, StorageSubSystem 개체가 용량 속성을 갖습니다.
* Azs.Compute.Admin 모듈           * 버그 수정: Add-AzsPlatformImage, Get-AzsPlatformImage: 성공 경로에서만 ConvertTo-PlatformImageObject 호출           * 버그 수정: Add-AzsVmExtension, Get-AzsVmExtension: 성공 경로에서만 ConvertTo-VmExtensionObject 호출
* Azs.Storage.Admin 모듈 * 버그 수정 - 새 스토리지 할당량이 제공되지 않을 경우 기본값을 사용합니다.'
