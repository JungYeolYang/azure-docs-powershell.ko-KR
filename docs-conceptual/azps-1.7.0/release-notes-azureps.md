---
ms.openlocfilehash: 54d7a9da878e085e90479fb229876c9be6dafd74
ms.sourcegitcommit: 89066b7c4b527357bb2024e1ad708df84c131804
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 04/09/2019
ms.locfileid: "59364137"
---
## <a name="170---april-2019"></a><span data-ttu-id="cd4ef-101">1.7.0 - 2019년 4월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-101">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="cd4ef-102">마지막 주 릴리스 이후의 주요 사항</span><span class="sxs-lookup"><span data-stu-id="cd4ef-102">Highlights since the last major release</span></span>
* <span data-ttu-id="cd4ef-103">`Az` 모듈 일반 공급</span><span class="sxs-lookup"><span data-stu-id="cd4ef-103">General availability of `Az` module</span></span>
* <span data-ttu-id="cd4ef-104">`Az` 모듈에 대한 자세한 내용은 https://aka.ms/azps-announce를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-104">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="cd4ef-105">Location, ResourceGroup 및 ResourceName 완성자가 추가되었습니다(https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/).</span><span class="sxs-lookup"><span data-stu-id="cd4ef-105">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="cd4ef-106">와일드카드 지원이 Az.Compute 및 Az.Network에 대한 Get cmdlet에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-106">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="cd4ef-107">Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-107">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cd4ef-108">Python 2 Runbook 지원이 Az.Automation에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-108">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="cd4ef-109">Az.LogicApp: 통합 계정 어셈블리 및 일괄 처리 구성을 위한 새로운 cmdlet입니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-109">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="cd4ef-110">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cd4ef-110">Az.Accounts</span></span>
* <span data-ttu-id="cd4ef-111">매개 변수 AzureAnalysisServicesEndpointResourceId를 허용하도록 Add-AzEnvironment 및 Set-AzEnvironment 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-111">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cd4ef-112">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-112">Az.AnalysisServices</span></span>
* <span data-ttu-id="cd4ef-113">데이터 평면 cmdlet에서 ServiceClient 사용 및 원본 인증 논리 제거</span><span class="sxs-lookup"><span data-stu-id="cd4ef-113">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="cd4ef-114">호환성이 손상되는 변경을 방지하기 위해 Add-AzureASAccount를 Connect-AzAccount의 래퍼로 만듦</span><span class="sxs-lookup"><span data-stu-id="cd4ef-114">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cd4ef-115">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cd4ef-115">Az.Automation</span></span>
* <span data-ttu-id="cd4ef-116">포함에 대한 New-AzAutomationSoftwareUpdateConfiguration cmdlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-116">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="cd4ef-117">이제 매개 변수 IncludedKbNumber 및 IncludedPackageNameMask가 작동함</span><span class="sxs-lookup"><span data-stu-id="cd4ef-117">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="cd4ef-118">Azure 자동화 업데이트 관리 동적 그룹에 대한 버그 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-118">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cd4ef-119">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-119">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-120">New-AzDiskConfig 및 New-AzSnapshotConfig에 HyperVGeneration 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-120">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="cd4ef-121">다른 테넌트의 갤러리 이미지를 사용하여 VM을 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="cd4ef-121">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="cd4ef-122">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cd4ef-122">Az.ContainerInstance</span></span>
* <span data-ttu-id="cd4ef-123">후행 빈 인수를 추가한 New-AzContainerGroup의 -Command 매개 변수의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-123">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cd4ef-124">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cd4ef-124">Az.DataFactory</span></span>
* <span data-ttu-id="cd4ef-125">ADF .Net SDK 버전을 3.0.2로 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-125">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="cd4ef-126">RepoConfiguration 관련 설정에 대한 추가 매개 변수로 Set-AzDataFactoryV2 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-126">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cd4ef-127">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-127">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-128">'-ResourceId' 또는 '-ResourceGroupName', '-Name' 및 '-ResourceType' 매개 변수를 제공할 때 'Get-AzResource'에 대한 공급자 처리 개선</span><span class="sxs-lookup"><span data-stu-id="cd4ef-128">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="cd4ef-129">'Test-AzDeployment' 및 'Test-AzResourceGroupDeployment'에 대한 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="cd4ef-129">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="cd4ef-130">배포 유효성 검사 외부에서 발생한 오류를 처리하고 그 대신 명령의 출력에 포함</span><span class="sxs-lookup"><span data-stu-id="cd4ef-130">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="cd4ef-131">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/6856를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-131">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="cd4ef-132">배포 cmdlet 세트에 스크립트 및 작업 시나리오에서 프롬프트를 건너뛰는 '-IgnoreDynamicParameters' 스위치 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-132">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="cd4ef-133">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/6856를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-133">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="cd4ef-134">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-134">Az.Sql</span></span>
* <span data-ttu-id="cd4ef-135">데이터베이스 데이터 분류 지원</span><span class="sxs-lookup"><span data-stu-id="cd4ef-135">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cd4ef-136">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cd4ef-136">Az.Storage</span></span>
* <span data-ttu-id="cd4ef-137">매개 변수 -UseConnectedAccount를 사용하여 스토리지 컨텍스트를 만들 때 자세한 오류 보고(단, 로그인 Azure 계정 없이)</span><span class="sxs-lookup"><span data-stu-id="cd4ef-137">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="cd4ef-138">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="cd4ef-138">New-AzStorageContext</span></span>
* <span data-ttu-id="cd4ef-139">관리 평면 API를 사용하여 지정한 스토리지 계정의 BLOB 서비스 속성 관리 지원</span><span class="sxs-lookup"><span data-stu-id="cd4ef-139">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="cd4ef-140">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="cd4ef-140">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="cd4ef-141">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="cd4ef-141">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="cd4ef-142">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="cd4ef-142">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="cd4ef-143">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="cd4ef-143">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="cd4ef-144">BLOB 및 파일 업로드/다운로드 cmdlet에 대한 -AsJob 지원</span><span class="sxs-lookup"><span data-stu-id="cd4ef-144">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="cd4ef-145">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="cd4ef-145">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="cd4ef-146">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="cd4ef-146">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="cd4ef-147">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="cd4ef-147">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="cd4ef-148">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="cd4ef-148">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="cd4ef-149">1.6.0 - 2019년 3월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-149">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="cd4ef-150">마지막 주 릴리스 이후의 주요 사항</span><span class="sxs-lookup"><span data-stu-id="cd4ef-150">Highlights since the last major release</span></span>
* <span data-ttu-id="cd4ef-151">`Az` 모듈 일반 공급</span><span class="sxs-lookup"><span data-stu-id="cd4ef-151">General availability of `Az` module</span></span>
* <span data-ttu-id="cd4ef-152">`Az` 모듈에 대한 자세한 내용은 https://aka.ms/azps-announce를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-152">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="cd4ef-153">Location, ResourceGroup 및 ResourceName 완성자가 추가되었습니다(https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/).</span><span class="sxs-lookup"><span data-stu-id="cd4ef-153">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="cd4ef-154">와일드카드 지원이 Az.Compute 및 Az.Network에 대한 Get cmdlet에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-154">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="cd4ef-155">Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-155">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cd4ef-156">Python 2 Runbook 지원이 Az.Automation에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-156">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="cd4ef-157">Az.LogicApp: 통합 계정 어셈블리 및 일괄 처리 구성을 위한 새로운 cmdlet입니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-157">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cd4ef-158">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cd4ef-158">Az.Automation</span></span>
* <span data-ttu-id="cd4ef-159">Azure 자동화 업데이트 관리에서 변경된 지원 기능은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-159">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="cd4ef-160">동적 그룹화</span><span class="sxs-lookup"><span data-stu-id="cd4ef-160">Dynamic grouping</span></span>
    * <span data-ttu-id="cd4ef-161">사전 스크립트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-161">Pre-Post script</span></span>
    * <span data-ttu-id="cd4ef-162">다시 부팅 설정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-162">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cd4ef-163">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-163">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-164">Get-AzVmBootDiagnosticsData의 경로 확인 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-164">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="cd4ef-165">Compute 클라이언트 라이브러리가 25.0.0으로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-165">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cd4ef-166">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cd4ef-166">Az.KeyVault</span></span>
* <span data-ttu-id="cd4ef-167">와일드카드 지원이 KeyVault cmdlet에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-167">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cd4ef-168">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cd4ef-168">Az.Network</span></span>
* <span data-ttu-id="cd4ef-169">Azure Firewall에 대한 위협 인텔리전스 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-169">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="cd4ef-170">Application Gateway 방화벽 정책의 최상위 수준 리소스 및 사용자 지정 규칙이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-170">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cd4ef-171">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-171">Az.RecoveryServices</span></span>
* <span data-ttu-id="cd4ef-172">인스턴트 RP를 지원하기 위해 SnapshotRetentionInDays가 Azure VM 정책에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-172">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="cd4ef-173">컨테이너 등록을 취소하는 파이프 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-173">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="cd4ef-174">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-174">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-175">Get-AzResource 및 Get-AzResourceGroup에 대한 와일드카드 지원을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-175">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="cd4ef-176">ARM에 대한 일반 호출을 수행할 때 사용되는 자격 증명을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-176">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="cd4ef-177">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-177">Az.Sql</span></span>
* <span data-ttu-id="cd4ef-178">위협 탐지의 cmdlet 매개 변수(ExcludeDetectionType)가 DetectionType에서 string[]으로 변경되어 새 DetectionType이 추가되면 이후의 증명이 되고 자동 완성도 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-178">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cd4ef-179">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cd4ef-179">Az.Storage</span></span>
* <span data-ttu-id="cd4ef-180">스토리지 계정에 대한 관리 정책 가져오기/설정/제거를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-180">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="cd4ef-181">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="cd4ef-181">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="cd4ef-182">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="cd4ef-182">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="cd4ef-183">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="cd4ef-183">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="cd4ef-184">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="cd4ef-184">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="cd4ef-185">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="cd4ef-185">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="cd4ef-186">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="cd4ef-186">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cd4ef-187">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cd4ef-187">Az.Websites</span></span>
* <span data-ttu-id="cd4ef-188">'New-AzWebApp -IncludeSourceWebAppSlots'를 사용하여 모든 슬롯의 복제를 중단하는 ARM 템플릿 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-188">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="cd4ef-189">1.5.0 - 2019년 3월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-189">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cd4ef-190">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cd4ef-190">Az.Accounts</span></span>
* <span data-ttu-id="cd4ef-191">'Register-AzModule' 명령을 추가하여 AutoRest 생성 cmdlet을 지원</span><span class="sxs-lookup"><span data-stu-id="cd4ef-191">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="cd4ef-192">Connect-AzAccount 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-192">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cd4ef-193">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cd4ef-193">Az.Automation</span></span>
* <span data-ttu-id="cd4ef-194">몇몇 Azure Automation cmdlet에서 특정 월별 일정을 검색할 때 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-194">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="cd4ef-195">상위 20개 노드를 반환하도록 Get-AzAutomationDscNode를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-195">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="cd4ef-196">이제 모든 노드 반환</span><span class="sxs-lookup"><span data-stu-id="cd4ef-196">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cd4ef-197">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cd4ef-197">Az.Cdn</span></span>
* <span data-ttu-id="cd4ef-198">사용자 지정 도메인 Https 사용/사용 안 함에 대한 새 Powershell cmdlet이 추가되었으며 기존의 것은 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-198">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cd4ef-199">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-199">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-200">Get cmdlet에 와일드 카드 지원 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-200">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cd4ef-201">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cd4ef-201">Az.DataFactory</span></span>
* <span data-ttu-id="cd4ef-202">ADF.Net SDK 버전이 3.0.1로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-202">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cd4ef-203">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cd4ef-203">Az.LogicApp</span></span>
* <span data-ttu-id="cd4ef-204">첫 결과 페이지 검색 시에만 ListWorkflows 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-204">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cd4ef-205">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cd4ef-205">Az.Network</span></span>
* <span data-ttu-id="cd4ef-206">Network cmdlet에 와일드 카드 지원 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-206">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cd4ef-207">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-207">Az.RecoveryServices</span></span>
* <span data-ttu-id="cd4ef-208">Azure VM 지원에 SQL 서버가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-208">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="cd4ef-209">SDK 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-209">SDK Update</span></span>
* <span data-ttu-id="cd4ef-210">VMappContainer 체크 인 Get-ProtectableItem 제거</span><span class="sxs-lookup"><span data-stu-id="cd4ef-210">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="cd4ef-211">Get ProtectableItem의 매개 변수로 Name과 ServerName이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-211">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="cd4ef-212">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-212">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-213">`-TemplateObject` 매개 변수를 추가하여 cmdlet을 배포</span><span class="sxs-lookup"><span data-stu-id="cd4ef-213">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="cd4ef-214">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/2933를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-214">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="cd4ef-215">`Get-AzResource`의 결과를 ??(으)로 파이프할 때 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-215">Fix issue when piping the result of `Get-AzResource` to</span></span> `Set-AzResource`
    - <span data-ttu-id="cd4ef-216">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8240를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-216">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="cd4ef-217">실행 시 JSON 데이터 형식 변경 문제 해결</span><span class="sxs-lookup"><span data-stu-id="cd4ef-217">Fix issue with JSON data type change when running</span></span> `Set-AzResource`
    - <span data-ttu-id="cd4ef-218">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7930를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-218">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="cd4ef-219">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-219">Az.Sql</span></span>
* <span data-ttu-id="cd4ef-220">AuditingEndpointsCommunicator를 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-220">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="cd4ef-221">새 진단 설정을 생성할 때 에지 사례의 동작을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-221">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cd4ef-222">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cd4ef-222">Az.Storage</span></span>
* <span data-ttu-id="cd4ef-223">스토리지 계정      - New-AzStorageAccount를 생성할 때 종류 BlockBlobStorage를 지원</span><span class="sxs-lookup"><span data-stu-id="cd4ef-223">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="cd4ef-224">1.4.0 - 2019년 2월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-224">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="cd4ef-225">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-225">Az.AnalysisServices</span></span>
* <span data-ttu-id="cd4ef-226">사용되지 않는 AddAzureASAccount cmdlet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-226">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cd4ef-227">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cd4ef-227">Az.Automation</span></span>
* <span data-ttu-id="cd4ef-228">Import-AzAutomationDscNodeConfiguration 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-228">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="cd4ef-229">Import-AzAutomationDscConfiguration cmdlet 구성 이름 유효성 검사 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-229">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="cd4ef-230">Import-AzAutomationDscConfiguration cmdlet 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="cd4ef-230">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="cd4ef-231">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-231">Az.CognitiveServices</span></span>
* <span data-ttu-id="cd4ef-232">리소스의 하위 도메인을 지정하는 데 사용되는 New-AzCognitiveServicesAccount에 대한 새 선택적 매개 변수로 CustomSubdomainName이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-232">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cd4ef-233">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-233">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-234">ID 매개 변수 집합 문제 해결</span><span class="sxs-lookup"><span data-stu-id="cd4ef-234">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="cd4ef-235">Name 매개 변수를 제공하지 않으면 Get-AzVMExtension이 설치된 모든 확장을 열거하도록 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-235">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="cd4ef-236">Update-AzImage cmdlet에 태그 및 ResourceId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-236">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="cd4ef-237">인스턴스 ID가 없는 Get-AzVmssVM과 InstanceView를 사용하면 인스턴스 보기가 있는 VMSS VM을 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-237">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cd4ef-238">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cd4ef-238">Az.DataLakeStore</span></span>
* <span data-ttu-id="cd4ef-239">ADL 삭제된 항목 열거 및 복원에 대한 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-239">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cd4ef-240">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cd4ef-240">Az.EventHub</span></span>
* <span data-ttu-id="cd4ef-241">Eventhub의 CaptureDescription 클래스에서 빈 보관을 건너뛰는 새 부울 속성 SkipEmptyArchives가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-241">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="cd4ef-242">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cd4ef-242">Az.KeyVault</span></span>
* <span data-ttu-id="cd4ef-243">Set-AzKeyVaultSecret 태그 지정 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-243">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cd4ef-244">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cd4ef-244">Az.LogicApp</span></span>
* <span data-ttu-id="cd4ef-245">통합 계정에 대한 기본 sku 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-245">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="cd4ef-246">XSLT 2.0, XSLT 3.0, Liquid 맵 형식 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-246">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="cd4ef-247">통합 계정 어셈블리에 대한 새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-247">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="cd4ef-248">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cd4ef-248">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cd4ef-249">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cd4ef-249">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cd4ef-250">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cd4ef-250">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cd4ef-251">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cd4ef-251">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="cd4ef-252">통합 계정 일괄 처리 구성에 대한 새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-252">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="cd4ef-253">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd4ef-253">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cd4ef-254">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd4ef-254">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cd4ef-255">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd4ef-255">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cd4ef-256">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd4ef-256">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="cd4ef-257">논리 앱 SDK를 버전 4.1.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-257">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cd4ef-258">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cd4ef-258">Az.Monitor</span></span>
* <span data-ttu-id="cd4ef-259">Get-AzMetric에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-259">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cd4ef-260">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cd4ef-260">Az.Network</span></span>
* <span data-ttu-id="cd4ef-261">Add-AzApplicationGatewayCustomError에 대한 도움말 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-261">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="cd4ef-262">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cd4ef-262">Az.OperationalInsights</span></span>
* <span data-ttu-id="cd4ef-263">New 및 Get ApplicationInsights 데이터 소스에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-263">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="cd4ef-264">지정된 작업 영역에 대한 특정 또는 전체 ApplicationInsights 데이터 원본 가져오기를 지원하기 위한 새로운 'ApplicationInsights' 종류가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-264">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="cd4ef-265">지정된 Application-Insights 리소스 매개 변수(구독 ID, resourceGroupName 및 이름)별로 데이터 원본을 만들기 위한 New-AzOperationalInsightsApplicationInsightsDataSource cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-265">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="cd4ef-266">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-266">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-267">문제 https://github.com/Azure/azure-powershell/issues/8166 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-267">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="cd4ef-268">문제 https://github.com/Azure/azure-powershell/issues/8235 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-268">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="cd4ef-269">문제 https://github.com/Azure/azure-powershell/issues/6219 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-269">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="cd4ef-270">KeyCredentials 반복 만들기를 방지하기 위해 버그 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-270">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="cd4ef-271">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-271">Az.Sql</span></span>
* <span data-ttu-id="cd4ef-272">SQL DB 하이퍼스케일에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-272">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="cd4ef-273">복원 요청에서 불필요한 속성을 설정하여 복원이 실패할 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-273">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cd4ef-274">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cd4ef-274">Az.Websites</span></span>
* <span data-ttu-id="cd4ef-275">Get-AzWebAppSlotMetrics 내 올바른 예제</span><span class="sxs-lookup"><span data-stu-id="cd4ef-275">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="cd4ef-276">1.3.0 - 2019년 2월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-276">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cd4ef-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cd4ef-277">Az.Accounts</span></span>
* <span data-ttu-id="cd4ef-278">ClientRuntime 최신 버전 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-278">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cd4ef-279">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-279">Az.AnalysisServices</span></span>
<span data-ttu-id="cd4ef-280">Az.AnalysisServices 모듈의 전반적인 가용성.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-280">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cd4ef-281">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-281">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-282">AEM 확장: UltraSSD 및 P60, P70, P80 디스크에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-282">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="cd4ef-283">Set-AzVMBootDiagnostics에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-283">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="cd4ef-284">Update-AzImage에 대한 도움말 및 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-284">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cd4ef-285">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-285">Az.RecoveryServices</span></span>
<span data-ttu-id="cd4ef-286">Az.RecoveryServices 모듈의 전반적인 가용성.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-286">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cd4ef-287">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-287">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-288">리소스 그룹 관련 태그 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-288">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="cd4ef-289">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8166를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-289">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="cd4ef-290">`Get-AzureRmRoleAssignment`이(가) -ErrorAction을 준수하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-290">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="cd4ef-291">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8235를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-291">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="cd4ef-292">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-292">Az.Sql</span></span>
* <span data-ttu-id="cd4ef-293">AzSqlDatabaseBackupShortTermRetentionPolicy 가져오기/설정하기 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-293">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="cd4ef-294">SQL cmdlet을 실행할 경우 Azure 계정에 로그인되어 있지 않은 것이 nullref 예외를 초래하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-294">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="cd4ef-295">Get-AzSqlCapability의 nullref 예외 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-295">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="cd4ef-296">1.2.1 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-296">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cd4ef-297">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cd4ef-297">Az.Accounts</span></span>
* <span data-ttu-id="cd4ef-298">올바른 인증 버전을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="cd4ef-298">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cd4ef-299">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-299">Az.AnalysisServices</span></span>
* <span data-ttu-id="cd4ef-300">업데이트된 인증 종속성을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="cd4ef-300">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cd4ef-301">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-301">Az.RecoveryServices</span></span>
* <span data-ttu-id="cd4ef-302">업데이트된 인증 종속성을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="cd4ef-302">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="cd4ef-303">1.2.0 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-303">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cd4ef-304">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cd4ef-304">Az.Accounts</span></span>
* <span data-ttu-id="cd4ef-305">Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-305">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cd4ef-306">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-306">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cd4ef-307">Uninstall-AzureRm 관련 PS Core에 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-307">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="cd4ef-308">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="cd4ef-308">Az.Aks</span></span>
* <span data-ttu-id="cd4ef-309">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-309">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cd4ef-310">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cd4ef-310">Az.Automation</span></span>
* <span data-ttu-id="cd4ef-311">Python 2 Runbook에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-311">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="cd4ef-312">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-312">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cd4ef-313">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cd4ef-313">Az.Cdn</span></span>
* <span data-ttu-id="cd4ef-314">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-314">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cd4ef-315">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-315">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-316">Invoke-AzVMReimage cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-316">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="cd4ef-317">Set-AzVmss에 TempDisk 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-317">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="cd4ef-318">New-AzVM 경고 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-318">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="cd4ef-319">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="cd4ef-319">Az.ContainerRegistry</span></span>
* <span data-ttu-id="cd4ef-320">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-320">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cd4ef-321">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cd4ef-321">Az.DataFactory</span></span>
* <span data-ttu-id="cd4ef-322">ADF.Net SDK 버전이 3.0.0으로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-322">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cd4ef-323">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cd4ef-323">Az.DataLakeStore</span></span>
* <span data-ttu-id="cd4ef-324">MSI를 사용할 때 ADLS 엔드포인트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-324">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="cd4ef-325">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7462를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-325">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="cd4ef-326">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-326">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cd4ef-327">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cd4ef-327">Az.IotHub</span></span>
* <span data-ttu-id="cd4ef-328">Add-IotHubRoutingEndpoint cmdlet에 인코딩 형식을 추가하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-328">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cd4ef-329">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cd4ef-329">Az.KeyVault</span></span>
* <span data-ttu-id="cd4ef-330">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-330">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cd4ef-331">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cd4ef-331">Az.Network</span></span>
* <span data-ttu-id="cd4ef-332">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-332">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="cd4ef-333">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-333">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-334">'New-AzADAppCredential' 및 'New-AzADSpCredential' 참조 설명서의 잘못된 예제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-334">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="cd4ef-335">리소스 그룹 배포 cmdlet 실행 전 '-TemplateFile' 매개 변수 경로가 확인되지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-335">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="cd4ef-336">Az.Resources: New-AzureRmPolicyDefinition -Mode 기본값에 대한 올바른 설명서</span><span class="sxs-lookup"><span data-stu-id="cd4ef-336">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="cd4ef-337">Az.Resources: 문제 https://github.com/Azure/azure-powershell/issues/7522 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-337">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="cd4ef-338">Az.Resources: 문제 https://github.com/Azure/azure-powershell/issues/5747 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-338">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="cd4ef-339">'PSResourceGroupDeployment' 개체의 서식 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-339">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="cd4ef-340">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/2123를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-340">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cd4ef-341">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cd4ef-341">Az.ServiceFabric</span></span>
* <span data-ttu-id="cd4ef-342">인증서가 VMSS 모델에 추가되었는데도 예외가 발생할 경우 롤백합니다. 이는 버그 https://github.com/Azure/service-fabric-issues/issues/932를 수정하기 위함입니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-342">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="cd4ef-343">일부 오류 메시지를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-343">Fix some error messages.</span></span>
* <span data-ttu-id="cd4ef-344">Az로의 마이그레이션을 통해서는 작동하지 않는 New-AzServiceFabriCluster를 위해 기본값 ARM 템플릿을 가진 클러스터 만들기를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-344">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="cd4ef-345">확장에서 클러스터 id를 확인하여 클러스터에 해당하는 VMSS에만 추가되도록 클러스터/애플리케이션 인증서 추가를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-345">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="cd4ef-346">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="cd4ef-346">Az.SignalR</span></span>
* <span data-ttu-id="cd4ef-347">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-347">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="cd4ef-348">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-348">Az.Sql</span></span>
* <span data-ttu-id="cd4ef-349">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-349">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cd4ef-350">가능한 값을 가진 LicenseType 매개 변수에 대한 매개 변수 설명이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-350">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="cd4ef-351">유일하게 업데이트된 속성인데 작동하지 않는 관리되는 인스턴스 ID의 업데이트 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-351">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="cd4ef-352">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="cd4ef-352">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cd4ef-353">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cd4ef-353">Az.Storage</span></span>
* <span data-ttu-id="cd4ef-354">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-354">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cd4ef-355">Premium Storage 계정이 클래식 로깅/메트릭을 지원하지 않기 때문에, Premium Storage 계정의 클래식 로깅/메트릭을 가져올/설정할 때 상세한 오류 메시지를 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-355">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="cd4ef-356">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="cd4ef-356">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="cd4ef-357">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="cd4ef-357">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="cd4ef-358">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="cd4ef-358">Az.TrafficManager</span></span>
* <span data-ttu-id="cd4ef-359">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-359">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cd4ef-360">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cd4ef-360">Az.Websites</span></span>
* <span data-ttu-id="cd4ef-361">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-361">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cd4ef-362">앱이 ASE에 호스팅되면 'New-AzWebAppSSLBinding'을 수정하여 올바른 resourcegroup+location에 인증서를 업로드합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-362">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="cd4ef-363">'New-AzWebAppSSLBinding'을 수정하여 SSL 인증서를 앱에 바인딩하는 데 붙는 태그를 덮어쓰지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-363">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="cd4ef-364">1.1.0 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-364">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cd4ef-365">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cd4ef-365">Az.Accounts</span></span>
* <span data-ttu-id="cd4ef-366">Enable-AzureRmAlias에 'Local' 범위 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-366">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cd4ef-367">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-367">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-368">이름이 Restart/Start/Stop/Remove/Set-AzVM과 Save-AzVMImage에 설정된 ID 매개 변수에서 선택 사항이 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-368">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="cd4ef-369">도움말 파일의 ID에 대한 설명이 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-369">Updated the description of ID in help files</span></span>
* <span data-ttu-id="cd4ef-370">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-370">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cd4ef-371">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cd4ef-371">Az.DataLakeStore</span></span>
* <span data-ttu-id="cd4ef-372">SDK 수정을 위해 데이터 평면의 SDK 버전을 1.1.14로 업데이트하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-372">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="cd4ef-373">getfilestatus 및 liststatus에 대한 음수 acesstime 및 modificationtime 수정, 비동기 취소 토큰 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-373">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="cd4ef-374">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="cd4ef-374">Az.EventGrid</span></span>
* <span data-ttu-id="cd4ef-375">2019-01-01 API 버전을 사용하도록 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-375">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="cd4ef-376">2019-01-01 API 버전에서 새 시나리오를 지원하도록 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-376">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="cd4ef-377">New-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-377">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="cd4ef-378">이벤트 Time-to-Live</span><span class="sxs-lookup"><span data-stu-id="cd4ef-378">Event Time-To-Live,</span></span>
        - <span data-ttu-id="cd4ef-379">이벤트에 대한 최대 배달 시도</span><span class="sxs-lookup"><span data-stu-id="cd4ef-379">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="cd4ef-380">배달 못한 편지의 엔드포인트입니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-380">Dead letter endpoint.</span></span>
    - <span data-ttu-id="cd4ef-381">Update-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-381">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="cd4ef-382">이벤트 Time-to-Live</span><span class="sxs-lookup"><span data-stu-id="cd4ef-382">Event Time-To-Live,</span></span>
        - <span data-ttu-id="cd4ef-383">이벤트에 대한 최대 배달 시도</span><span class="sxs-lookup"><span data-stu-id="cd4ef-383">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="cd4ef-384">배달 못한 편지의 엔드포인트입니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-384">Dead letter endpoint.</span></span>
* <span data-ttu-id="cd4ef-385">New-AzureRmEventGridSubscription 및 Update-AzureRmEventGridSubscription cmdlet의 EndpointType 옵션에 새 열거형 값(즉, storageQueue 및 hybridConnection)을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-385">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="cd4ef-386">이벤트 구독을 생성 또는 업데이트할 때 사용자가 직접 조치를 취해야 할 경우 경고 메시지를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-386">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cd4ef-387">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cd4ef-387">Az.IotHub</span></span>
* <span data-ttu-id="cd4ef-388">최신 버전의 Azure IotHub SDK로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="cd4ef-388">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cd4ef-389">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cd4ef-389">Az.LogicApp</span></span>
* <span data-ttu-id="cd4ef-390">지정된 이름이 없는 모든 Get-AzLogicApp 목록</span><span class="sxs-lookup"><span data-stu-id="cd4ef-390">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="cd4ef-391">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-391">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-392">'Get-AzResource'에 '-ODataQuery'및 '-ResourceId' 매개 변수를 제공할 때 매개 변수 집합 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-392">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="cd4ef-393">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7875를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-393">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="cd4ef-394">New/Set-AzPolicyDefinition에서 -Custom 매개 변수 처리 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-394">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="cd4ef-395">New-AzDeployment 설명서에서 오타 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-395">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="cd4ef-396">'New-AzADUser'에 '-MailNickname'매개 변수가 필수 항목으로 지정됨</span><span class="sxs-lookup"><span data-stu-id="cd4ef-396">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="cd4ef-397">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8220를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-397">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="cd4ef-398">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="cd4ef-398">Az.SignalR</span></span>
* <span data-ttu-id="cd4ef-399">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-399">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="cd4ef-400">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-400">Az.Sql</span></span>
* <span data-ttu-id="cd4ef-401">Storage 관리 클라이언트 종속성을 일반적인 SDK 구현으로 변환했습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-401">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cd4ef-402">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cd4ef-402">Az.Storage</span></span>
* <span data-ttu-id="cd4ef-403">Sas Token, OAuth 또는 Anonymous를 사용하여 스토리지 컨텍스트의 StorageAccountName을 실제 스토리지 계정 이름으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-403">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="cd4ef-404">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="cd4ef-404">New-AzStorageContext</span></span>
* <span data-ttu-id="cd4ef-405">'-FullUri' 매개 변수를 사용하여 BLOB 스냅숏 개체의 Sas Token을 생성하고 반환된 Uri를 스냅숏 Uri로 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-405">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="cd4ef-406">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="cd4ef-406">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cd4ef-407">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cd4ef-407">Az.Websites</span></span>
* <span data-ttu-id="cd4ef-408">'Get-AzDeletedWebApp'의 날짜 구문 분석 버그를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-408">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="cd4ef-409">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-409">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="cd4ef-410">1.0.0 - 2018년 12월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-410">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="cd4ef-411">일반</span><span class="sxs-lookup"><span data-stu-id="cd4ef-411">General</span></span>

- <span data-ttu-id="cd4ef-412">Az 모듈 일반 공급</span><span class="sxs-lookup"><span data-stu-id="cd4ef-412">General Availability of Az Module</span></span>
- <span data-ttu-id="cd4ef-413">각 모듈에 대 한 온라인 도움말</span><span class="sxs-lookup"><span data-stu-id="cd4ef-413">Online help for each module</span></span>
- <span data-ttu-id="cd4ef-414">자세한 내용과 로드맵은 [Az 알림 페이지](https://aka.ms/azps-announce)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-414">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="cd4ef-415">AzureRM에서 마이그레이션하는 것에 대한 정보는 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-415">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="cd4ef-416">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cd4ef-416">Az.Accounts</span></span>
- <span data-ttu-id="cd4ef-417">Az.Profile에서 변경</span><span class="sxs-lookup"><span data-stu-id="cd4ef-417">Changed from Az.Profile</span></span>
- <span data-ttu-id="cd4ef-418">프로필 및 컨텍스트 형식에 대한 표 형식 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-418">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="cd4ef-419">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cd4ef-419">Az.ApiManagement</span></span>
- <span data-ttu-id="cd4ef-420">#7002에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-420">Fixes for #7002</span></span>
- <span data-ttu-id="cd4ef-421">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-421">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="cd4ef-422">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="cd4ef-422">Az.Batch</span></span>
- <span data-ttu-id="cd4ef-423">`PSComputeNode`의 새로운 `NodeAgentInformation` 속성을 통해 풀의 각 VM에서 실행 중인 Azure Batch 노드 에이전트의 버전을 확인하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-423">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="cd4ef-424">`PSDataDisk`에 대한 `Caching` 기본 값은 이제 `None` 대신 `ReadWrite`입니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-424">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="cd4ef-425">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-425">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="cd4ef-426">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="cd4ef-426">Az.Billing</span></span>
- <span data-ttu-id="cd4ef-427">청구, 소비 및 UsageAggregates cmdlet 결합 cmdlet에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-427">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="cd4ef-428">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-428">Az.CognitivServices</span></span>
- <span data-ttu-id="cd4ef-429">New-AzureRmCognitiveServicesAccount 작업에서 사용 가능한 SkuName 및 Typem에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-429">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="cd4ef-430">Get-AzCognitiveServicesAccountSkus에서 GetSkusWithAccountParamSetName 매개 변수 집합을 제거</span><span class="sxs-lookup"><span data-stu-id="cd4ef-430">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="cd4ef-431">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cd4ef-431">Az.ContainerInstance</span></span>
- <span data-ttu-id="cd4ef-432">ManagedIdentity 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="cd4ef-432">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="cd4ef-433">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="cd4ef-433">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="cd4ef-434">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-434">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="cd4ef-435">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cd4ef-435">Az.DataLakeStore</span></span>
- <span data-ttu-id="cd4ef-436">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-436">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="cd4ef-437">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cd4ef-437">Az.Monitor</span></span>
- <span data-ttu-id="cd4ef-438">Az.Monitor 이름 변경 및 기타 사소한 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-438">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="cd4ef-439">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cd4ef-439">Az.KeyVault</span></span>
- <span data-ttu-id="cd4ef-440">출력 형식에서 사용되지 않는 'PurgeDisabled' 속성 제거</span><span class="sxs-lookup"><span data-stu-id="cd4ef-440">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="cd4ef-441">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="cd4ef-441">Az.MachineLearning</span></span>
- <span data-ttu-id="cd4ef-442">Az.MachineLearningCompute 모듈의 cmdlet 포함</span><span class="sxs-lookup"><span data-stu-id="cd4ef-442">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="cd4ef-443">Az.Media</span><span class="sxs-lookup"><span data-stu-id="cd4ef-443">Az.Media</span></span>
- <span data-ttu-id="cd4ef-444">New-AzMediaService에서 사용되지 않는 -Tags 별칭이 제거됨</span><span class="sxs-lookup"><span data-stu-id="cd4ef-444">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="cd4ef-445">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cd4ef-445">Az.Network</span></span>
<span data-ttu-id="cd4ef-446">Application Gateway에서 RewriteRuleSets를 구성하는 것에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="cd4ef-446">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="cd4ef-447">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-447">New cmdlets added:</span></span>
        - <span data-ttu-id="cd4ef-448">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-448">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cd4ef-449">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-449">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cd4ef-450">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-450">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cd4ef-451">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-451">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cd4ef-452">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-452">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cd4ef-453">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="cd4ef-453">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="cd4ef-454">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-454">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="cd4ef-455">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd4ef-455">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="cd4ef-456">선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-456">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="cd4ef-457">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="cd4ef-457">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="cd4ef-458">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="cd4ef-458">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="cd4ef-459">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="cd4ef-459">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="cd4ef-460">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="cd4ef-460">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="cd4ef-461">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="cd4ef-461">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="cd4ef-462">New-AzureRmApplicationGatewayUrlPathMapConfig로 ID를 사용하여 Application Gateway에 KeyVault 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-462">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="cd4ef-463">선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="cd4ef-463">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="cd4ef-464">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cd4ef-464">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="cd4ef-465">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cd4ef-465">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="cd4ef-466">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cd4ef-466">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="cd4ef-467">New-AzApplicationGateway cmdlet이 선택적 매개 변수를 사용하도록 업데이트됨 -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="cd4ef-467">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="cd4ef-468">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-468">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="cd4ef-469">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cd4ef-469">Az.OperationalInsights</span></span>
- <span data-ttu-id="cd4ef-470">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-470">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="cd4ef-471">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cd4ef-471">Az.Profile</span></span>
- <span data-ttu-id="cd4ef-472">Az.Accounts에 모듈 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="cd4ef-472">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="cd4ef-473">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-473">Az.RecoveryServices</span></span>
- <span data-ttu-id="cd4ef-474">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-474">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="cd4ef-475">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-475">Az.Resources</span></span>
- <span data-ttu-id="cd4ef-476">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-476">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="cd4ef-477">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cd4ef-477">Az.ServiceFabric</span></span>
- <span data-ttu-id="cd4ef-478">일반 이름과 지문으로 지정 인증서 지원</span><span class="sxs-lookup"><span data-stu-id="cd4ef-478">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="cd4ef-479">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-479">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="cd4ef-480">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="cd4ef-480">Az.SIgnalR</span></span>
- <span data-ttu-id="cd4ef-481">SIgnalR에 대한 PowerShell cmdlet에 대한 일반 공급</span><span class="sxs-lookup"><span data-stu-id="cd4ef-481">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="cd4ef-482">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-482">Az.Sql</span></span>
- <span data-ttu-id="cd4ef-483">위협 탐지의 cmdlet에 새로운 Data_Exfiltration 및 Unsafe_Action 검색 유형 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-483">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="cd4ef-484">Sql 감사 cmdlet에 대한 설명서 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-484">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="cd4ef-485">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-485">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="cd4ef-486">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cd4ef-486">Az.Storage</span></span>
- <span data-ttu-id="cd4ef-487">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-487">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="cd4ef-488">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cd4ef-488">Az.Websites</span></span>
- <span data-ttu-id="cd4ef-489">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-489">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="cd4ef-490">0.7.0 - 2018년 12월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-490">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="cd4ef-491">일반</span><span class="sxs-lookup"><span data-stu-id="cd4ef-491">General</span></span>

* <span data-ttu-id="cd4ef-492">AzureRM에서 Az 전환 예정에 대한 사소한 변경</span><span class="sxs-lookup"><span data-stu-id="cd4ef-492">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="cd4ef-493">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-493">Az.Compute</span></span>

* <span data-ttu-id="cd4ef-494">`New-AzVm(ss)` cmdlet에 대한 간단한 매개 변수 집합에 UltraSSD 및 갤러리 이미지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-494">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="cd4ef-495">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cd4ef-495">Az.DataLakeStore</span></span>

* <span data-ttu-id="cd4ef-496">ADLS 계정의 도메인의 후행 슬래시를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-496">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="cd4ef-497">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="cd4ef-497">Az.FrontDoor</span></span>

* <span data-ttu-id="cd4ef-498">일부 끊어진 링크 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-498">Fixed some broken links</span></span>
    - <span data-ttu-id="cd4ef-499">New-AzureRmFrontDoor 및 Set-AzureRmFrontDoor 아티클에서 New-AzureRmFrontDoorHealthProbeSettingObject cmdlet 아티클에 대한 링크가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-499">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="cd4ef-500">New-AzureRmFrontDoorManagedRuleObject 아티클에서 New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet 아티클에 대한 링크가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-500">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="cd4ef-501">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-501">Az.RecoveryServices</span></span>

* <span data-ttu-id="cd4ef-502">Azure File Share 복원 작업에 클라이언트 측 유효성 검사가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-502">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="cd4ef-503">afs 복원의 경우 storageAccountName 및 storageAccountResourceGroupName을 선택적으로 만들었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-503">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="cd4ef-504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-504">Az.Resources</span></span>

* <span data-ttu-id="cd4ef-505">https://github.com/Azure/azure-powershell/issues/7679 에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-505">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="cd4ef-506">기본 관리자를 요청할 때 구독 범위가 제공되는 경우 Get-AzureRmRoleAssignment를 업데이트하여 구독 범위를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-506">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="cd4ef-507">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-507">Az.Sql</span></span>

* <span data-ttu-id="cd4ef-508">AzureRM에서 Az 전환 예정에 대한 사소한 변경</span><span class="sxs-lookup"><span data-stu-id="cd4ef-508">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="cd4ef-509">DotNet 코어에서 Get-AzureRmSqlDatabaseVulnerabilityAssessment를 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="cd4ef-509">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="cd4ef-510">SQL 감사 cmdlet과 관련된 도움말 메시지의 설명서가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-510">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="cd4ef-511">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cd4ef-511">Az.Storage</span></span>

* <span data-ttu-id="cd4ef-512">New-AzureRmStorageAccount에 -EnableHierarchicalNamespace 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-512">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="cd4ef-513">파일 복사 cmdlet이 -DestContext 입력이 없을 때 대상의 원본 컨텍스트를 다시 사용할 수 없는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-513">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="cd4ef-514">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="cd4ef-514">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="cd4ef-515">고정적인 웹 사이트 구성 지원</span><span class="sxs-lookup"><span data-stu-id="cd4ef-515">Support Static Website configuration</span></span>
    - <span data-ttu-id="cd4ef-516">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="cd4ef-516">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="cd4ef-517">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="cd4ef-517">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="cd4ef-518">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cd4ef-518">Az.Websites</span></span>

* <span data-ttu-id="cd4ef-519">Set-AzureRmWebApp 및 Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="cd4ef-519">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="cd4ef-520">Windows 및 Linux 컨테이너 응용 프로그램에 탑재할 Azure Storage 경로를 지정하기 위해 새 매개 변수(-AzureStoragePath)가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-520">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="cd4ef-521">새 cmdlet New-AzureRmWebAppAzureStoragePath의 출력을 매개 변수로 사용하여 Azure Storage 경로를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-521">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="cd4ef-522">0.6.1 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-522">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="cd4ef-523">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cd4ef-523">Az.ApiManagement</span></span>
* <span data-ttu-id="cd4ef-524">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-524">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="cd4ef-525">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cd4ef-525">Az.Automation</span></span>
* <span data-ttu-id="cd4ef-526">Azure Automation cmdlet 기반 Swagger</span><span class="sxs-lookup"><span data-stu-id="cd4ef-526">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="cd4ef-527">업데이트 관리 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-527">Added Update Management cmdlets</span></span>
* <span data-ttu-id="cd4ef-528">소스 제어 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-528">Added Source Control cmdlets</span></span>
* <span data-ttu-id="cd4ef-529">Remove-AzureRmAutomationHybridWorkerGroup cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-529">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="cd4ef-530">DSC 노드 등록 명령 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-530">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="cd4ef-531">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-531">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-532">SystemAssigned ID에 대한 ID 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-532">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="cd4ef-533">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-533">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="cd4ef-534">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cd4ef-534">Az.ContainerInstance</span></span>
* <span data-ttu-id="cd4ef-535">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-535">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="cd4ef-536">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="cd4ef-536">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="cd4ef-537">마켓플레이스 cmdlet에 대한 예제 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-537">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="cd4ef-538">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cd4ef-538">Az.Network</span></span>
* <span data-ttu-id="cd4ef-539">New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-539">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="cd4ef-540">지원되는 AzureFirewall 네트워크 프로토콜에 ICMP 다시 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-540">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="cd4ef-541">Test-AzureRmNetworkWatcherConnectivity cmdlet을 업데이트하여 대상 ID, 주소 및 포트 유효성 검사를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-541">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="cd4ef-542">VirtualNetwork 맵의 메모리 사용 문제 해결</span><span class="sxs-lookup"><span data-stu-id="cd4ef-542">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="cd4ef-543">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="cd4ef-543">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="cd4ef-544">보호된 파일 공유에 대한 정책을 수정하는 것에 대해 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-544">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="cd4ef-545">정책 표준 시간대를 대문자로 변환했습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-545">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="cd4ef-546">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="cd4ef-546">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="cd4ef-547">New-AzureRmRecoveryServicesAsrProtectableItem의 예제 정정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-547">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="cd4ef-548">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-548">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="cd4ef-549">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="cd4ef-549">Az.Relay</span></span>
* <span data-ttu-id="cd4ef-550">선택적 매개 변수 -KeyValue를 New-AzureRmRelayKey cmdlet에 추가하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-550">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="cd4ef-551">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-551">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-552">`New-AzureRmPolicyAssignment` 및 ??의 리소스 ID 관련 매개 변수에 대한 도움말 문서 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-552">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and</span></span> `Set-AzureRmPolicyAssignment`
* <span data-ttu-id="cd4ef-553">-Metadata를 사용하는 New-AzureRmPolicyDefinition에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-553">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="cd4ef-554">NetStandard의 태그 키에서 대소문자 보존을 허용하도록 수정: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="cd4ef-554">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="cd4ef-555">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cd4ef-555">Az.ServiceFabric</span></span>
* <span data-ttu-id="cd4ef-556">향후 호환성이 손상되는 변경에 대한 사용 중단 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-556">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="cd4ef-557">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-557">Az.Sql</span></span>
* <span data-ttu-id="cd4ef-558">Azure Sql Database Managed Instance 및 Azure Sql 관리 데이터베이스에 CRUD 작업을 위한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-558">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="cd4ef-559">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cd4ef-559">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cd4ef-560">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cd4ef-560">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cd4ef-561">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cd4ef-561">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cd4ef-562">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cd4ef-562">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cd4ef-563">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cd4ef-563">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cd4ef-564">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cd4ef-564">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cd4ef-565">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cd4ef-565">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cd4ef-566">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cd4ef-566">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="cd4ef-567">서버 또는 데이터베이스에서 확장 감사 정책 관리를 활성화했습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-567">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="cd4ef-568">새 매개 변수(PredicateExpression)가 감사 로그 필터링을 사용하도록 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-568">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="cd4ef-569">Cmdlet이 레거시 클라이언트 대신 SQL 클라이언트를 사용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-569">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="cd4ef-570">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-570">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="cd4ef-571">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-571">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="cd4ef-572">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-572">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="cd4ef-573">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-573">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="cd4ef-574">스토리지 계정 이름 매개 변수가 설정된 Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings를 사용할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="cd4ef-574">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="cd4ef-575">0.5.0 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-575">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="cd4ef-576">일반</span><span class="sxs-lookup"><span data-stu-id="cd4ef-576">General</span></span>
* <span data-ttu-id="cd4ef-577">많은 핵심 cmdlet에 Resource Completers를 추가하여 대화형으로 cmdlet을 호출할 때 기존 리소스 이름을 탭으로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-577">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="cd4ef-578">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cd4ef-578">Az.Profile</span></span>
* <span data-ttu-id="cd4ef-579">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-579">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="cd4ef-580">Connect-AzAccount cmdlet의 매개 변수 TenantId 이름을 Tenant로 바꾸고 TenantId의 별칭을 추가합니다</span><span class="sxs-lookup"><span data-stu-id="cd4ef-580">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="cd4ef-581">Connect-AzAccount의 업데이트된 TenantId 설명</span><span class="sxs-lookup"><span data-stu-id="cd4ef-581">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="cd4ef-582">테넌트 도메인을 제공할 때 실패한 로그인에 대한 오류 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-582">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="cd4ef-583">테넌트에 구독이 없는 계정의 컨텍스트 이름 충돌 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-583">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="cd4ef-584">MSI를 사용할 때 DataLake 엔드포인트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-584">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="cd4ef-585">연결되지 않은 경우 'Disconnect-AzAccount'가 throw하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-585">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="cd4ef-586">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-586">Az.CognitiveServices</span></span>
* <span data-ttu-id="cd4ef-587">Get-AzCognitiveServicesAccountSkus 작업을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-587">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cd4ef-588">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-588">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-589">Add-AzVmssVMDataDisk 및 Remove-AzVmssVMDataDisk cmdlet를 추가합니다</span><span class="sxs-lookup"><span data-stu-id="cd4ef-589">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="cd4ef-590">Get-AzVMImage는 AutomaticOSUpgradeProperties를 표시합니다</span><span class="sxs-lookup"><span data-stu-id="cd4ef-590">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="cd4ef-591">수정된 SetAzVMChefExtension -BootstrapOptions 및 -JsonAttribute option 값이 json 형식으로 설정하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-591">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cd4ef-592">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cd4ef-592">Az.DataLakeStore</span></span>
* <span data-ttu-id="cd4ef-593">DataLake 패키지를 1.1.10으로 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-593">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="cd4ef-594">기본 동시성을 다중 스레드 작업에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-594">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="cd4ef-595">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="cd4ef-595">Az.Insights</span></span>
* <span data-ttu-id="cd4ef-596">해결된 문제 #7267(자동 크기 조정 영역)</span><span class="sxs-lookup"><span data-stu-id="cd4ef-596">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="cd4ef-597">열거된 매개 변수를 제대로 설정하지 않은 새 자동 크기 조정 규칙을 만드는 데 문제가 있습니다(이를 항상 기본값으로 설정함).</span><span class="sxs-lookup"><span data-stu-id="cd4ef-597">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="cd4ef-598">해결된 문제 # 7513[자세한 정보] Set-AzDiagnosticSetting은 설정을 생성하는 동안 범주를 명시적으로 지정해야 합니다</span><span class="sxs-lookup"><span data-stu-id="cd4ef-598">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="cd4ef-599">이제 cmdlet은 생성 중에 사용할 범주를 명시적으로 표시할 필요가 없습니다. 즉, 문서화된대로 작동합니다</span><span class="sxs-lookup"><span data-stu-id="cd4ef-599">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cd4ef-600">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cd4ef-600">Az.Network</span></span>
* <span data-ttu-id="cd4ef-601">다음 cmdlet에 대해 PeeringType을 필수 매개 변수로 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-601">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="cd4ef-602">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="cd4ef-602">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="cd4ef-603">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="cd4ef-603">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="cd4ef-604">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="cd4ef-604">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="cd4ef-605">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="cd4ef-605">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="cd4ef-606">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="cd4ef-606">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="cd4ef-607">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="cd4ef-607">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="cd4ef-608">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="cd4ef-608">Az.PolicyInsights</span></span>
* <span data-ttu-id="cd4ef-609">추가된 정책 재구성 cmdlet</span><span class="sxs-lookup"><span data-stu-id="cd4ef-609">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="cd4ef-610">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-610">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-611">https://github.com/Azure/azure-powershell/issues/7402 에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-611">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="cd4ef-612">'Get-AzResource'에 대해 '-ResourceId' 매개 변수를 사용하여 리소스 나열 허용</span><span class="sxs-lookup"><span data-stu-id="cd4ef-612">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="cd4ef-613">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="cd4ef-613">Az.ServiceBus</span></span>
* <span data-ttu-id="cd4ef-614">마이그레이션 상태를 알 수 있도록 PSServiceBusMigrationConfigurationAttributes에 MigrationState 읽기 전용 속성 추가.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-614">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cd4ef-615">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cd4ef-615">Az.ServiceFabric</span></span>
* <span data-ttu-id="cd4ef-616">Linux Vmss에 인증서 추가 수정.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-616">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="cd4ef-617">Add-AzServiceFabricClusterCertificate 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-617">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="cd4ef-618">새 인증서(Azure/service-fabric-issues#932)에서 올바른 지문을 사용.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-618">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="cd4ef-619">올바르게 예외 표시(Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="cd4ef-619">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="cd4ef-620">Vmss CreateOrUpdate 작업을 시작하기 전에 'Update-AzServiceFabricDurability'를 수정하여 클러스터 구성 업데이트.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-620">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="cd4ef-621">0.4.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-621">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="cd4ef-622">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cd4ef-622">Az.Profile</span></span>
* <span data-ttu-id="cd4ef-623">CloudShell에서 Get-AzSubscription을 사용하여 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-623">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="cd4ef-624">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-624">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cd4ef-625">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-625">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-626">'New-AzVm'에 대해 간단한 매개 변수를 사용하는 경우 가속화된 네트워킹을 설정하기 위해 새 크기가 VM 크기의 허용 목록에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-626">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="cd4ef-627">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-627">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cd4ef-628">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cd4ef-628">Az.DataLakeStore</span></span>
* <span data-ttu-id="cd4ef-629">Virtual Network 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-629">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="cd4ef-630">Get-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 가져오거나 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-630">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="cd4ef-631">Add-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 가상 네트워크 규칙을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-631">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="cd4ef-632">Set-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 지정된 가상 네트워크 규칙을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-632">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="cd4ef-633">Remove-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-633">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cd4ef-634">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cd4ef-634">Az.Network</span></span>
* <span data-ttu-id="cd4ef-635">Test-AzNetworkWatcherConnectivity cmdlet을 업데이트하고, 백 엔드에 프로토콜 값을 전달합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-635">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="cd4ef-636">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-636">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cd4ef-637">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-637">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-638">(기본 프로필에 구독이 없고 범위가 지정되지 않은 경우) 시나리오에서 의미 있는 예외를 추가하여 Get-AzRoleDefinition이 인식할 수 없는 예외를 throw하는 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-638">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="cd4ef-639">또한 기본 매개 변수 집합을 'RoleDefinitionNameParameterSet'으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-639">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="cd4ef-640">0.3.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-640">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="cd4ef-641">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="cd4ef-641">Azure.Storage</span></span>
* <span data-ttu-id="cd4ef-642">대상에 메타데이터가 있을 때 Blob/파일이 메타 데이터를 복사하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-642">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="cd4ef-643">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="cd4ef-643">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="cd4ef-644">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="cd4ef-644">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="cd4ef-645">특정 위치의 저장소 리소스 사용을 지원하고 글로벌 저장소 리소스 사용 가져오기는 더 이상 사용되지 않는다는 경고 메시지를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-645">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="cd4ef-646">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="cd4ef-646">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="cd4ef-647">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cd4ef-647">Az.CognitiveServices</span></span>
* <span data-ttu-id="cd4ef-648">기존 계정이 없는 Get-AzCognitiveServicesAccountSkus를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-648">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cd4ef-649">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cd4ef-649">Az.Compute</span></span>
* <span data-ttu-id="cd4ef-650">Get-AzVM -ResourceGroupName <rg>가 필요한 경우 50개가 넘는 결과를 반환하도록 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-650">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="cd4ef-651">'SimpleParameterSet' 예제가 New-AzVmss cmdlet 도움말에 추가됨</span><span class="sxs-lookup"><span data-stu-id="cd4ef-651">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="cd4ef-652">Azure Disk Encryption 진행률 메시지의 오타를 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-652">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="cd4ef-653">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="cd4ef-653">Az.DataFactoryV2</span></span>
* <span data-ttu-id="cd4ef-654">ADF.Net SDK 버전을 2.3.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="cd4ef-654">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cd4ef-655">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cd4ef-655">Az.Network</span></span>
* <span data-ttu-id="cd4ef-656">NetworkProfile 기능 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-656">Added NetworkProfile functionality.</span></span> <span data-ttu-id="cd4ef-657">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-657">new cmdlets added</span></span>
    - <span data-ttu-id="cd4ef-658">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cd4ef-658">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="cd4ef-659">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cd4ef-659">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="cd4ef-660">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cd4ef-660">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="cd4ef-661">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cd4ef-661">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="cd4ef-662">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="cd4ef-662">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="cd4ef-663">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="cd4ef-663">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="cd4ef-664">서브넷 모델에 서비스 연결 링크 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-664">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="cd4ef-665">New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-665">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="cd4ef-666">Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-666">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="cd4ef-667">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="cd4ef-667">Az.RedisCache</span></span>
* <span data-ttu-id="cd4ef-668">모든 문자열을 Size 매개 변수로 진행되도록 허용</span><span class="sxs-lookup"><span data-stu-id="cd4ef-668">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="cd4ef-669">PSArgumentCompleter 팝업에 P5 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-669">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="cd4ef-670">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cd4ef-670">Az.Resources</span></span>
* <span data-ttu-id="cd4ef-671">-Mode 매개 변수를 Set-AzPolicyDefinition에 추가</span><span class="sxs-lookup"><span data-stu-id="cd4ef-671">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="cd4ef-672">사용자가 포함된 Origin 작업에서 Get-AzProviderOperation commandlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="cd4ef-672">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="cd4ef-673">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cd4ef-673">Az.Sql</span></span>
* <span data-ttu-id="cd4ef-674">일부 백업 cmdlet이 현재 azure 구독을 인식하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="cd4ef-674">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cd4ef-675">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cd4ef-675">Az.Websites</span></span>
* <span data-ttu-id="cd4ef-676">새 cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - 컨테이너 지속적인 배포 Webhook URL을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-676">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="cd4ef-677">새 cmdlet New-AzWebAppContainerPSSession 및 Enter-WebAppContainerPSSession -  windows 컨테이너 앱에 PowerShell 원격 세션을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="cd4ef-677">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="cd4ef-678">0.2.0 - 2018년 9월</span><span class="sxs-lookup"><span data-stu-id="cd4ef-678">0.2.0 - September 2018</span></span>
 <span data-ttu-id="cd4ef-679">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="cd4ef-679">Initial Release</span></span>