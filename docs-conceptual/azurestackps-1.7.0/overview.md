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
ms.openlocfilehash: af34497f243ce8f4f718e88312f6ad54eb6ad848
ms.sourcegitcommit: 993db64e68b222acbcfdeef2e81eb3316b160858
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 02/14/2019
ms.locfileid: "56240534"
---
# <a name="azure-stack-module-170"></a>Azure Stack 모듈 1.7.0

## <a name="requirements"></a>Requirements:
최소 지원 Azure Stack 버전은 1901입니다.

참고: 이전 버전을 사용하는 경우 1.7.0 버전을 설치하세요.

## <a name="install"></a>설치
```
# Remove previous versions of AzureStack and AzureRM modules
Uninstall-Module -Name AzureRM -Force
Uninstall-Module -Name Azure.Storage -Force
Uninstall-Module -Name AzureStack -Force
Get-Module -Name "Azs*" -ListAvailable | Uninstall-Module  -Force 
Get-Module -Name "AzureRm*" -ListAvailable | Uninstall-Module  -Force

# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module AzureRM -RequiredVersion 2.4.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.0
```
## <a name="release-notes"></a>릴리스 정보
* 1901 업데이트 지원
* 이는 호환성이 손상되는 변경 릴리스입니다. 호환성이 손상되는 변경에 대한 자세한 내용은 https://aka.ms/azspshmigration170를 참조하세요.
* Azs.Backup.Admin 모듈 * 호환성이 손상되는 변경: Backup이 인증서 기반 암호화 모드로 변경됩니다. 대칭 키에 대한 지원은 사용되지 않습니다.
* Azs.Fabric.Admin 모듈 * 사용 중단 * Get-AzsInfrastructureVolume은 더 이상 사용되지 않으며, 새 cmdlet Get-AzsVolume이 제공됩니다. * Get-AzsStorageSystem은 더 이상 사용되지 않으며, 새 cmdlet Get-AzsStorageSubSystem이 제공됩니다. * Get-AzsStoragePool은 더 이상 사용되지 않으며, StorageSubSystem 개체가 용량 속성을 갖습니다.
* Azs.Compute.Admin 모듈           * 버그 수정: Add-AzsPlatformImage, Get-AzsPlatformImage: 성공 경로에서만 ConvertTo-PlatformImageObject 호출           * 버그 수정: Add-AzsVmExtension, Get-AzsVmExtension: 성공 경로에서만 ConvertTo-VmExtensionObject 호출
* Azs.Storage.Admin 모듈 * 버그 수정 - 새 스토리지 할당량이 제공되지 않을 경우 기본값을 사용합니다.'

