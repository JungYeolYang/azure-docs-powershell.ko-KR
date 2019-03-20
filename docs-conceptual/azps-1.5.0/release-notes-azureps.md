---
ms.openlocfilehash: 9915ff37e59a73c1d226a216213fd9016b55d3d4
ms.sourcegitcommit: 447276d46ffeeb37f0c07a570536665e36c5ddb8
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 03/14/2019
ms.locfileid: "57882475"
---
## <a name="150---march-2019"></a><span data-ttu-id="e4109-101">1.5.0 - 2019년 3월</span><span class="sxs-lookup"><span data-stu-id="e4109-101">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e4109-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e4109-102">Az.Accounts</span></span>
* <span data-ttu-id="e4109-103">'Register-AzModule' 명령을 추가하여 AutoRest 생성 cmdlet을 지원</span><span class="sxs-lookup"><span data-stu-id="e4109-103">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="e4109-104">Connect-AzAccount 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-104">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e4109-105">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e4109-105">Az.Automation</span></span>
* <span data-ttu-id="e4109-106">몇몇 Azure Automation cmdlet에서 특정 월별 일정을 검색할 때 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-106">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="e4109-107">상위 20개 노드를 반환하도록 Get-AzAutomationDscNode를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-107">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="e4109-108">이제 모든 노드 반환</span><span class="sxs-lookup"><span data-stu-id="e4109-108">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="e4109-109">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="e4109-109">Az.Cdn</span></span>
* <span data-ttu-id="e4109-110">사용자 지정 도메인 Https 사용/사용 안 함에 대한 새 Powershell cmdlet이 추가되었으며 기존의 것은 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-110">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e4109-111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e4109-111">Az.Compute</span></span>
* <span data-ttu-id="e4109-112">Get cmdlet에 와일드 카드 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-112">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e4109-113">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e4109-113">Az.DataFactory</span></span>
* <span data-ttu-id="e4109-114">ADF.Net SDK 버전이 3.0.1로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-114">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="e4109-115">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="e4109-115">Az.LogicApp</span></span>
* <span data-ttu-id="e4109-116">첫 결과 페이지 검색 시에만 ListWorkflows 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-116">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e4109-117">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e4109-117">Az.Network</span></span>
* <span data-ttu-id="e4109-118">Network cmdlet에 와일드 카드 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-118">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e4109-119">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e4109-119">Az.RecoveryServices</span></span>
* <span data-ttu-id="e4109-120">Azure VM 지원에 SQL 서버가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-120">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="e4109-121">SDK 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-121">SDK Update</span></span>
* <span data-ttu-id="e4109-122">VMappContainer 체크 인 Get-ProtectableItem 제거</span><span class="sxs-lookup"><span data-stu-id="e4109-122">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="e4109-123">Get ProtectableItem의 매개 변수로 Name과 ServerName이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-123">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="e4109-124">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-124">Az.Resources</span></span>
* <span data-ttu-id="e4109-125">`-TemplateObject` 매개 변수를 추가하여 cmdlet을 배포</span><span class="sxs-lookup"><span data-stu-id="e4109-125">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="e4109-126">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/2933를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-126">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="e4109-127">`Get-AzResource`의 결과를 `Set-AzResource`(으)로 파이프할 때 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-127">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="e4109-128">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8240를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-128">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="e4109-129">실행 시 JSON 데이터 형식 문제 해결 `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="e4109-129">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="e4109-130">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7930를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-130">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="e4109-131">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e4109-131">Az.Sql</span></span>
* <span data-ttu-id="e4109-132">AuditingEndpointsCommunicator를 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-132">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="e4109-133">새 진단 설정을 생성할 때 에지 사례의 동작을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-133">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e4109-134">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e4109-134">Az.Storage</span></span>
* <span data-ttu-id="e4109-135">스토리지 계정      - New-AzStorageAccount를 생성할 때 종류 BlockBlobStorage를 지원</span><span class="sxs-lookup"><span data-stu-id="e4109-135">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="e4109-136">1.4.0 - 2019년 2월</span><span class="sxs-lookup"><span data-stu-id="e4109-136">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="e4109-137">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="e4109-137">Az.AnalysisServices</span></span>
* <span data-ttu-id="e4109-138">사용되지 않는 AddAzureASAccount cmdlet</span><span class="sxs-lookup"><span data-stu-id="e4109-138">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e4109-139">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e4109-139">Az.Automation</span></span>
* <span data-ttu-id="e4109-140">Import-AzAutomationDscNodeConfiguration 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-140">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="e4109-141">Import-AzAutomationDscConfiguration cmdlet 구성 이름 유효성 검사 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-141">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="e4109-142">Import-AzAutomationDscConfiguration cmdlet 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="e4109-142">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="e4109-143">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e4109-143">Az.CognitiveServices</span></span>
* <span data-ttu-id="e4109-144">리소스의 하위 도메인을 지정하는 데 사용되는 New-AzCognitiveServicesAccount에 대한 새 선택적 매개 변수로 CustomSubdomainName이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-144">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e4109-145">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e4109-145">Az.Compute</span></span>
* <span data-ttu-id="e4109-146">ID 매개 변수 집합 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e4109-146">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="e4109-147">Name 매개 변수를 제공하지 않으면 Get-AzVMExtension이 설치된 모든 확장을 열거하도록 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-147">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="e4109-148">Update-AzImage cmdlet에 태그 및 ResourceId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-148">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="e4109-149">인스턴스 ID가 없는 Get-AzVmssVM과 InstanceView를 사용하면 인스턴스 보기가 있는 VMSS VM을 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-149">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e4109-150">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e4109-150">Az.DataLakeStore</span></span>
* <span data-ttu-id="e4109-151">ADL 삭제된 항목 열거 및 복원에 대한 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-151">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="e4109-152">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="e4109-152">Az.EventHub</span></span>
* <span data-ttu-id="e4109-153">Eventhub의 CaptureDescription 클래스에서 빈 보관을 건너뛰는 새 부울 속성 SkipEmptyArchives가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-153">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="e4109-154">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e4109-154">Az.KeyVault</span></span>
* <span data-ttu-id="e4109-155">Set-AzKeyVaultSecret 태그 지정 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-155">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="e4109-156">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="e4109-156">Az.LogicApp</span></span>
* <span data-ttu-id="e4109-157">통합 계정에 대한 기본 sku 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-157">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="e4109-158">XSLT 2.0, XSLT 3.0, Liquid 맵 형식 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-158">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="e4109-159">통합 계정 어셈블리에 대한 새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="e4109-159">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="e4109-160">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="e4109-160">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="e4109-161">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="e4109-161">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="e4109-162">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="e4109-162">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="e4109-163">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="e4109-163">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="e4109-164">통합 계정 일괄 처리 구성에 대한 새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="e4109-164">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="e4109-165">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4109-165">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="e4109-166">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4109-166">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="e4109-167">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4109-167">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="e4109-168">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4109-168">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="e4109-169">논리 앱 SDK를 버전 4.1.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-169">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="e4109-170">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e4109-170">Az.Monitor</span></span>
* <span data-ttu-id="e4109-171">Get-AzMetric에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-171">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e4109-172">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e4109-172">Az.Network</span></span>
* <span data-ttu-id="e4109-173">Add-AzApplicationGatewayCustomError에 대한 도움말 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-173">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="e4109-174">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="e4109-174">Az.OperationalInsights</span></span>
* <span data-ttu-id="e4109-175">New 및 Get ApplicationInsights 데이터 소스에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-175">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="e4109-176">지정된 작업 영역에 대한 특정 또는 전체 ApplicationInsights 데이터 원본 가져오기를 지원하기 위한 새로운 'ApplicationInsights' 종류가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-176">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="e4109-177">지정된 Application-Insights 리소스 매개 변수(구독 ID, resourceGroupName 및 이름)별로 데이터 원본을 만들기 위한 New-AzOperationalInsightsApplicationInsightsDataSource cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-177">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="e4109-178">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-178">Az.Resources</span></span>
* <span data-ttu-id="e4109-179">문제 https://github.com/Azure/azure-powershell/issues/8166 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-179">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="e4109-180">문제 https://github.com/Azure/azure-powershell/issues/8235 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-180">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="e4109-181">문제 https://github.com/Azure/azure-powershell/issues/6219 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-181">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="e4109-182">KeyCredentials 반복 만들기를 방지하기 위해 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-182">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="e4109-183">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e4109-183">Az.Sql</span></span>
* <span data-ttu-id="e4109-184">SQL DB 하이퍼스케일에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-184">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="e4109-185">복원 요청에서 불필요한 속성을 설정하여 복원이 실패할 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-185">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e4109-186">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e4109-186">Az.Websites</span></span>
* <span data-ttu-id="e4109-187">Get-AzWebAppSlotMetrics 내 올바른 예제</span><span class="sxs-lookup"><span data-stu-id="e4109-187">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="e4109-188">1.3.0 - 2019년 2월</span><span class="sxs-lookup"><span data-stu-id="e4109-188">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e4109-189">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e4109-189">Az.Accounts</span></span>
* <span data-ttu-id="e4109-190">ClientRuntime 최신 버전 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-190">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="e4109-191">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="e4109-191">Az.AnalysisServices</span></span>
<span data-ttu-id="e4109-192">Az.AnalysisServices 모듈의 전반적인 가용성.</span><span class="sxs-lookup"><span data-stu-id="e4109-192">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e4109-193">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e4109-193">Az.Compute</span></span>
* <span data-ttu-id="e4109-194">AEM 확장: UltraSSD 및 P60, P70, P80 디스크에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-194">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="e4109-195">Set-AzVMBootDiagnostics에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-195">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="e4109-196">Update-AzImage에 대한 도움말 및 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-196">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e4109-197">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e4109-197">Az.RecoveryServices</span></span>
<span data-ttu-id="e4109-198">Az.RecoveryServices 모듈의 전반적인 가용성.</span><span class="sxs-lookup"><span data-stu-id="e4109-198">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e4109-199">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-199">Az.Resources</span></span>
* <span data-ttu-id="e4109-200">리소스 그룹 관련 태그 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-200">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="e4109-201">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8166를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-201">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="e4109-202">`Get-AzureRmRoleAssignment`이(가) -ErrorAction을 준수하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-202">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="e4109-203">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8235를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-203">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="e4109-204">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e4109-204">Az.Sql</span></span>
* <span data-ttu-id="e4109-205">AzSqlDatabaseBackupShortTermRetentionPolicy 가져오기/설정하기 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-205">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="e4109-206">SQL cmdlet을 실행할 경우 Azure 계정에 로그인되어 있지 않은 것이 nullref 예외를 초래하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-206">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="e4109-207">Get-AzSqlCapability의 nullref 예외 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-207">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="e4109-208">1.2.1 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="e4109-208">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e4109-209">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e4109-209">Az.Accounts</span></span>
* <span data-ttu-id="e4109-210">올바른 인증 버전을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="e4109-210">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="e4109-211">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="e4109-211">Az.AnalysisServices</span></span>
* <span data-ttu-id="e4109-212">업데이트된 인증 종속성을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="e4109-212">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="e4109-213">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e4109-213">Az.RecoveryServices</span></span>
* <span data-ttu-id="e4109-214">업데이트된 인증 종속성을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="e4109-214">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="e4109-215">1.2.0 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="e4109-215">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e4109-216">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e4109-216">Az.Accounts</span></span>
* <span data-ttu-id="e4109-217">Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-217">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="e4109-218">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-218">Update incorrect online help URLs</span></span>
* <span data-ttu-id="e4109-219">Uninstall-AzureRm 관련 PS Core에 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-219">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="e4109-220">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="e4109-220">Az.Aks</span></span>
* <span data-ttu-id="e4109-221">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-221">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="e4109-222">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e4109-222">Az.Automation</span></span>
* <span data-ttu-id="e4109-223">Python 2 Runbook에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-223">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="e4109-224">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-224">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="e4109-225">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="e4109-225">Az.Cdn</span></span>
* <span data-ttu-id="e4109-226">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-226">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e4109-227">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e4109-227">Az.Compute</span></span>
* <span data-ttu-id="e4109-228">Invoke-AzVMReimage cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-228">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="e4109-229">Set-AzVmss에 TempDisk 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-229">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="e4109-230">New-AzVM 경고 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-230">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="e4109-231">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="e4109-231">Az.ContainerRegistry</span></span>
* <span data-ttu-id="e4109-232">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-232">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="e4109-233">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="e4109-233">Az.DataFactory</span></span>
* <span data-ttu-id="e4109-234">ADF.Net SDK 버전이 3.0.0으로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-234">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e4109-235">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e4109-235">Az.DataLakeStore</span></span>
* <span data-ttu-id="e4109-236">MSI를 사용할 때 ADLS 엔드포인트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-236">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="e4109-237">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7462를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-237">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="e4109-238">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-238">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e4109-239">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e4109-239">Az.IotHub</span></span>
* <span data-ttu-id="e4109-240">Add-IotHubRoutingEndpoint cmdlet에 인코딩 형식을 추가하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-240">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="e4109-241">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e4109-241">Az.KeyVault</span></span>
* <span data-ttu-id="e4109-242">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-242">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e4109-243">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e4109-243">Az.Network</span></span>
* <span data-ttu-id="e4109-244">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-244">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="e4109-245">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-245">Az.Resources</span></span>
* <span data-ttu-id="e4109-246">'New-AzADAppCredential' 및 'New-AzADSpCredential' 참조 설명서의 잘못된 예제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-246">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="e4109-247">리소스 그룹 배포 cmdlet 실행 전 '-TemplateFile' 매개 변수 경로가 확인되지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-247">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="e4109-248">Az.Resources: New-AzureRmPolicyDefinition -Mode 기본값에 대한 올바른 설명서</span><span class="sxs-lookup"><span data-stu-id="e4109-248">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="e4109-249">Az.Resources: 문제 https://github.com/Azure/azure-powershell/issues/7522 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-249">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="e4109-250">Az.Resources: 문제 https://github.com/Azure/azure-powershell/issues/5747 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-250">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="e4109-251">'PSResourceGroupDeployment' 개체의 서식 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-251">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="e4109-252">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/2123를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-252">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="e4109-253">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e4109-253">Az.ServiceFabric</span></span>
* <span data-ttu-id="e4109-254">인증서가 VMSS 모델에 추가되었는데도 예외가 발생할 경우 롤백합니다. 이는 버그 https://github.com/Azure/service-fabric-issues/issues/932를 수정하기 위함입니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-254">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="e4109-255">일부 오류 메시지를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-255">Fix some error messages.</span></span>
* <span data-ttu-id="e4109-256">Az로의 마이그레이션을 통해서는 작동하지 않는 New-AzServiceFabriCluster를 위해 기본값 ARM 템플릿을 가진 클러스터 만들기를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-256">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="e4109-257">확장에서 클러스터 id를 확인하여 클러스터에 해당하는 VMSS에만 추가되도록 클러스터/애플리케이션 인증서 추가를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-257">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="e4109-258">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="e4109-258">Az.SignalR</span></span>
* <span data-ttu-id="e4109-259">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-259">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="e4109-260">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e4109-260">Az.Sql</span></span>
* <span data-ttu-id="e4109-261">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-261">Update incorrect online help URLs</span></span>
* <span data-ttu-id="e4109-262">가능한 값을 가진 LicenseType 매개 변수에 대한 매개 변수 설명이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-262">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="e4109-263">유일하게 업데이트된 속성인데 작동하지 않는 관리되는 인스턴스 ID의 업데이트 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-263">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="e4109-264">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="e4109-264">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e4109-265">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e4109-265">Az.Storage</span></span>
* <span data-ttu-id="e4109-266">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-266">Update incorrect online help URLs</span></span>
* <span data-ttu-id="e4109-267">Premium Storage 계정이 클래식 로깅/메트릭을 지원하지 않기 때문에, Premium Storage 계정의 클래식 로깅/메트릭을 가져올/설정할 때 상세한 오류 메시지를 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-267">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="e4109-268">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="e4109-268">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="e4109-269">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="e4109-269">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="e4109-270">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="e4109-270">Az.TrafficManager</span></span>
* <span data-ttu-id="e4109-271">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-271">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e4109-272">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e4109-272">Az.Websites</span></span>
* <span data-ttu-id="e4109-273">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-273">Update incorrect online help URLs</span></span>
* <span data-ttu-id="e4109-274">앱이 ASE에 호스팅되면 'New-AzWebAppSSLBinding'을 수정하여 올바른 resourcegroup+location에 인증서를 업로드합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-274">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="e4109-275">'New-AzWebAppSSLBinding'을 수정하여 SSL 인증서를 앱에 바인딩하는 데 붙는 태그를 덮어쓰지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-275">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="e4109-276">1.1.0 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="e4109-276">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="e4109-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e4109-277">Az.Accounts</span></span>
* <span data-ttu-id="e4109-278">Enable-AzureRmAlias에 'Local' 범위 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-278">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e4109-279">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e4109-279">Az.Compute</span></span>
* <span data-ttu-id="e4109-280">이름이 Restart/Start/Stop/Remove/Set-AzVM과 Save-AzVMImage에 설정된 ID 매개 변수에서 선택 사항이 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-280">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="e4109-281">도움말 파일의 ID에 대한 설명이 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-281">Updated the description of ID in help files</span></span>
* <span data-ttu-id="e4109-282">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-282">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e4109-283">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e4109-283">Az.DataLakeStore</span></span>
* <span data-ttu-id="e4109-284">SDK 수정을 위해 데이터 평면의 SDK 버전을 1.1.14로 업데이트하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-284">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="e4109-285">getfilestatus 및 liststatus에 대한 음수 acesstime 및 modificationtime 수정, 비동기 취소 토큰 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-285">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="e4109-286">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="e4109-286">Az.EventGrid</span></span>
* <span data-ttu-id="e4109-287">2019-01-01 API 버전을 사용하도록 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-287">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="e4109-288">2019-01-01 API 버전에서 새 시나리오를 지원하도록 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-288">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="e4109-289">New-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-289">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="e4109-290">이벤트 Time-to-Live</span><span class="sxs-lookup"><span data-stu-id="e4109-290">Event Time-To-Live,</span></span>
        - <span data-ttu-id="e4109-291">이벤트에 대한 최대 배달 시도</span><span class="sxs-lookup"><span data-stu-id="e4109-291">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="e4109-292">배달 못한 편지의 엔드포인트입니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-292">Dead letter endpoint.</span></span>
    - <span data-ttu-id="e4109-293">Update-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-293">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="e4109-294">이벤트 Time-to-Live</span><span class="sxs-lookup"><span data-stu-id="e4109-294">Event Time-To-Live,</span></span>
        - <span data-ttu-id="e4109-295">이벤트에 대한 최대 배달 시도</span><span class="sxs-lookup"><span data-stu-id="e4109-295">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="e4109-296">배달 못한 편지의 엔드포인트입니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-296">Dead letter endpoint.</span></span>
* <span data-ttu-id="e4109-297">New-AzureRmEventGridSubscription 및 Update-AzureRmEventGridSubscription cmdlet의 EndpointType 옵션에 새 열거형 값(즉, storageQueue 및 hybridConnection)을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-297">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="e4109-298">이벤트 구독을 생성 또는 업데이트할 때 사용자가 직접 조치를 취해야 할 경우 경고 메시지를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-298">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="e4109-299">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="e4109-299">Az.IotHub</span></span>
* <span data-ttu-id="e4109-300">최신 버전의 Azure IotHub SDK로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="e4109-300">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="e4109-301">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="e4109-301">Az.LogicApp</span></span>
* <span data-ttu-id="e4109-302">지정된 이름이 없는 모든 Get-AzLogicApp 목록</span><span class="sxs-lookup"><span data-stu-id="e4109-302">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="e4109-303">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-303">Az.Resources</span></span>
* <span data-ttu-id="e4109-304">'Get-AzResource'에 '-ODataQuery'및 '-ResourceId' 매개 변수를 제공할 때 매개 변수 집합 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-304">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="e4109-305">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7875를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-305">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="e4109-306">New/Set-AzPolicyDefinition에서 -Custom 매개 변수 처리 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-306">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="e4109-307">New-AzDeployment 설명서에서 오타 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-307">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="e4109-308">'New-AzADUser'에 '-MailNickname'매개 변수가 필수 항목으로 지정됨</span><span class="sxs-lookup"><span data-stu-id="e4109-308">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="e4109-309">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8220를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-309">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="e4109-310">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="e4109-310">Az.SignalR</span></span>
* <span data-ttu-id="e4109-311">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-311">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="e4109-312">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e4109-312">Az.Sql</span></span>
* <span data-ttu-id="e4109-313">Storage 관리 클라이언트 종속성을 일반적인 SDK 구현으로 변환했습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-313">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="e4109-314">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e4109-314">Az.Storage</span></span>
* <span data-ttu-id="e4109-315">Sas Token, OAuth 또는 Anonymous를 사용하여 스토리지 컨텍스트의 StorageAccountName을 실제 스토리지 계정 이름으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-315">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="e4109-316">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="e4109-316">New-AzStorageContext</span></span>
* <span data-ttu-id="e4109-317">'-FullUri' 매개 변수를 사용하여 BLOB 스냅숏 개체의 Sas Token을 생성하고 반환된 Uri를 스냅숏 Uri로 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-317">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="e4109-318">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="e4109-318">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e4109-319">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e4109-319">Az.Websites</span></span>
* <span data-ttu-id="e4109-320">'Get-AzDeletedWebApp'의 날짜 구문 분석 버그를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-320">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="e4109-321">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-321">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="e4109-322">1.0.0 - 2018년 12월</span><span class="sxs-lookup"><span data-stu-id="e4109-322">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="e4109-323">일반</span><span class="sxs-lookup"><span data-stu-id="e4109-323">General</span></span>

- <span data-ttu-id="e4109-324">Az 모듈 일반 공급</span><span class="sxs-lookup"><span data-stu-id="e4109-324">General Availability of Az Module</span></span>
- <span data-ttu-id="e4109-325">각 모듈에 대 한 온라인 도움말</span><span class="sxs-lookup"><span data-stu-id="e4109-325">Online help for each module</span></span>
- <span data-ttu-id="e4109-326">자세한 내용과 로드맵은 [Az 알림 페이지](https://aka.ms/azps-announce)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-326">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="e4109-327">AzureRM에서 마이그레이션하는 것에 대한 정보는 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-327">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="e4109-328">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="e4109-328">Az.Accounts</span></span>
- <span data-ttu-id="e4109-329">Az.Profile에서 변경</span><span class="sxs-lookup"><span data-stu-id="e4109-329">Changed from Az.Profile</span></span>
- <span data-ttu-id="e4109-330">프로필 및 컨텍스트 형식에 대한 표 형식 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-330">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="e4109-331">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e4109-331">Az.ApiManagement</span></span>
- <span data-ttu-id="e4109-332">#7002에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-332">Fixes for #7002</span></span>
- <span data-ttu-id="e4109-333">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-333">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="e4109-334">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="e4109-334">Az.Batch</span></span>
- <span data-ttu-id="e4109-335">`PSComputeNode`의 새로운 `NodeAgentInformation` 속성을 통해 풀의 각 VM에서 실행 중인 Azure Batch 노드 에이전트의 버전을 확인하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-335">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="e4109-336">`PSDataDisk`에 대한 `Caching` 기본 값은 이제 `None` 대신 `ReadWrite`입니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-336">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="e4109-337">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-337">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="e4109-338">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="e4109-338">Az.Billing</span></span>
- <span data-ttu-id="e4109-339">청구, 소비 및 UsageAggregates cmdlet 결합 cmdlet에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-339">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="e4109-340">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="e4109-340">Az.CognitivServices</span></span>
- <span data-ttu-id="e4109-341">New-AzureRmCognitiveServicesAccount 작업에서 사용 가능한 SkuName 및 Typem에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-341">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="e4109-342">Get-AzCognitiveServicesAccountSkus에서 GetSkusWithAccountParamSetName 매개 변수 집합을 제거</span><span class="sxs-lookup"><span data-stu-id="e4109-342">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="e4109-343">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="e4109-343">Az.ContainerInstance</span></span>
- <span data-ttu-id="e4109-344">ManagedIdentity 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e4109-344">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="e4109-345">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="e4109-345">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="e4109-346">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-346">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="e4109-347">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e4109-347">Az.DataLakeStore</span></span>
- <span data-ttu-id="e4109-348">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-348">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="e4109-349">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="e4109-349">Az.Monitor</span></span>
- <span data-ttu-id="e4109-350">Az.Monitor 이름 변경 및 기타 사소한 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-350">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="e4109-351">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="e4109-351">Az.KeyVault</span></span>
- <span data-ttu-id="e4109-352">출력 형식에서 사용되지 않는 'PurgeDisabled' 속성 제거</span><span class="sxs-lookup"><span data-stu-id="e4109-352">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="e4109-353">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="e4109-353">Az.MachineLearning</span></span>
- <span data-ttu-id="e4109-354">Az.MachineLearningCompute 모듈의 cmdlet 포함</span><span class="sxs-lookup"><span data-stu-id="e4109-354">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="e4109-355">Az.Media</span><span class="sxs-lookup"><span data-stu-id="e4109-355">Az.Media</span></span>
- <span data-ttu-id="e4109-356">New-AzMediaService에서 사용되지 않는 -Tags 별칭이 제거됨</span><span class="sxs-lookup"><span data-stu-id="e4109-356">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="e4109-357">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e4109-357">Az.Network</span></span>
<span data-ttu-id="e4109-358">Application Gateway에서 RewriteRuleSets를 구성하는 것에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="e4109-358">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="e4109-359">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-359">New cmdlets added:</span></span>
        - <span data-ttu-id="e4109-360">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e4109-360">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="e4109-361">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e4109-361">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="e4109-362">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e4109-362">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="e4109-363">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e4109-363">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="e4109-364">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e4109-364">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="e4109-365">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="e4109-365">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="e4109-366">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="e4109-366">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="e4109-367">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4109-367">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="e4109-368">선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="e4109-368">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="e4109-369">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="e4109-369">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="e4109-370">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="e4109-370">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="e4109-371">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="e4109-371">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="e4109-372">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="e4109-372">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="e4109-373">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="e4109-373">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="e4109-374">New-AzureRmApplicationGatewayUrlPathMapConfig로 ID를 사용하여 Application Gateway에 KeyVault 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-374">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="e4109-375">선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="e4109-375">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="e4109-376">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="e4109-376">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="e4109-377">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="e4109-377">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="e4109-378">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="e4109-378">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="e4109-379">New-AzApplicationGateway cmdlet이 선택적 매개 변수를 사용하도록 업데이트됨 -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="e4109-379">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="e4109-380">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-380">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="e4109-381">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="e4109-381">Az.OperationalInsights</span></span>
- <span data-ttu-id="e4109-382">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-382">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="e4109-383">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="e4109-383">Az.Profile</span></span>
- <span data-ttu-id="e4109-384">Az.Accounts에 모듈 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="e4109-384">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="e4109-385">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e4109-385">Az.RecoveryServices</span></span>
- <span data-ttu-id="e4109-386">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-386">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="e4109-387">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-387">Az.Resources</span></span>
- <span data-ttu-id="e4109-388">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-388">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="e4109-389">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e4109-389">Az.ServiceFabric</span></span>
- <span data-ttu-id="e4109-390">일반 이름과 지문으로 지정 인증서 지원</span><span class="sxs-lookup"><span data-stu-id="e4109-390">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="e4109-391">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-391">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="e4109-392">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="e4109-392">Az.SIgnalR</span></span>
- <span data-ttu-id="e4109-393">SIgnalR에 대한 PowerShell cmdlet에 대한 일반 공급</span><span class="sxs-lookup"><span data-stu-id="e4109-393">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="e4109-394">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e4109-394">Az.Sql</span></span>
- <span data-ttu-id="e4109-395">위협 탐지의 cmdlet에 새로운 Data_Exfiltration 및 Unsafe_Action 검색 유형 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-395">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="e4109-396">Sql 감사 cmdlet에 대한 설명서 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-396">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="e4109-397">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-397">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="e4109-398">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e4109-398">Az.Storage</span></span>
- <span data-ttu-id="e4109-399">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-399">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="e4109-400">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e4109-400">Az.Websites</span></span>
- <span data-ttu-id="e4109-401">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="e4109-401">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="e4109-402">0.7.0 - 2018년 12월</span><span class="sxs-lookup"><span data-stu-id="e4109-402">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="e4109-403">일반</span><span class="sxs-lookup"><span data-stu-id="e4109-403">General</span></span>

* <span data-ttu-id="e4109-404">AzureRM에서 Az 전환 예정에 대한 사소한 변경</span><span class="sxs-lookup"><span data-stu-id="e4109-404">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="e4109-405">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e4109-405">Az.Compute</span></span>

* <span data-ttu-id="e4109-406">`New-AzVm(ss)` cmdlet에 대한 간단한 매개 변수 집합에 UltraSSD 및 갤러리 이미지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-406">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="e4109-407">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e4109-407">Az.DataLakeStore</span></span>

* <span data-ttu-id="e4109-408">ADLS 계정의 도메인의 후행 슬래시를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-408">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="e4109-409">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="e4109-409">Az.FrontDoor</span></span>

* <span data-ttu-id="e4109-410">일부 끊어진 링크 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-410">Fixed some broken links</span></span>
    - <span data-ttu-id="e4109-411">New-AzureRmFrontDoor 및 Set-AzureRmFrontDoor 아티클에서 New-AzureRmFrontDoorHealthProbeSettingObject cmdlet 아티클에 대한 링크가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-411">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="e4109-412">New-AzureRmFrontDoorManagedRuleObject 아티클에서 New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet 아티클에 대한 링크가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-412">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="e4109-413">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="e4109-413">Az.RecoveryServices</span></span>

* <span data-ttu-id="e4109-414">Azure File Share 복원 작업에 클라이언트 측 유효성 검사가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-414">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="e4109-415">afs 복원의 경우 storageAccountName 및 storageAccountResourceGroupName을 선택적으로 만들었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-415">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="e4109-416">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-416">Az.Resources</span></span>

* <span data-ttu-id="e4109-417">https://github.com/Azure/azure-powershell/issues/7679 에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-417">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="e4109-418">기본 관리자를 요청할 때 구독 범위가 제공되는 경우 Get-AzureRmRoleAssignment를 업데이트하여 구독 범위를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-418">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="e4109-419">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e4109-419">Az.Sql</span></span>

* <span data-ttu-id="e4109-420">AzureRM에서 Az 전환 예정에 대한 사소한 변경</span><span class="sxs-lookup"><span data-stu-id="e4109-420">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="e4109-421">DotNet 코어에서 Get-AzureRmSqlDatabaseVulnerabilityAssessment를 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e4109-421">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="e4109-422">SQL 감사 cmdlet과 관련된 도움말 메시지의 설명서가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-422">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="e4109-423">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="e4109-423">Az.Storage</span></span>

* <span data-ttu-id="e4109-424">New-AzureRmStorageAccount에 -EnableHierarchicalNamespace 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-424">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="e4109-425">파일 복사 cmdlet이 -DestContext 입력이 없을 때 대상의 원본 컨텍스트를 다시 사용할 수 없는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-425">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="e4109-426">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="e4109-426">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="e4109-427">고정적인 웹 사이트 구성 지원</span><span class="sxs-lookup"><span data-stu-id="e4109-427">Support Static Website configuration</span></span>
    - <span data-ttu-id="e4109-428">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="e4109-428">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="e4109-429">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="e4109-429">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="e4109-430">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e4109-430">Az.Websites</span></span>

* <span data-ttu-id="e4109-431">Set-AzureRmWebApp 및 Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="e4109-431">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="e4109-432">Windows 및 Linux 컨테이너 응용 프로그램에 탑재할 Azure Storage 경로를 지정하기 위해 새 매개 변수(-AzureStoragePath)가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-432">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="e4109-433">새 cmdlet New-AzureRmWebAppAzureStoragePath의 출력을 매개 변수로 사용하여 Azure Storage 경로를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-433">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="e4109-434">0.6.1 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="e4109-434">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="e4109-435">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="e4109-435">Az.ApiManagement</span></span>
* <span data-ttu-id="e4109-436">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-436">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="e4109-437">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="e4109-437">Az.Automation</span></span>
* <span data-ttu-id="e4109-438">Azure Automation cmdlet 기반 Swagger</span><span class="sxs-lookup"><span data-stu-id="e4109-438">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="e4109-439">업데이트 관리 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-439">Added Update Management cmdlets</span></span>
* <span data-ttu-id="e4109-440">소스 제어 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-440">Added Source Control cmdlets</span></span>
* <span data-ttu-id="e4109-441">Remove-AzureRmAutomationHybridWorkerGroup cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-441">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="e4109-442">DSC 노드 등록 명령 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-442">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="e4109-443">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e4109-443">Az.Compute</span></span>
* <span data-ttu-id="e4109-444">SystemAssigned ID에 대한 ID 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-444">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="e4109-445">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-445">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="e4109-446">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="e4109-446">Az.ContainerInstance</span></span>
* <span data-ttu-id="e4109-447">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-447">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="e4109-448">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="e4109-448">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="e4109-449">마켓플레이스 cmdlet에 대한 예제 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-449">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="e4109-450">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e4109-450">Az.Network</span></span>
* <span data-ttu-id="e4109-451">New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-451">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="e4109-452">지원되는 AzureFirewall 네트워크 프로토콜에 ICMP 다시 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-452">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="e4109-453">Test-AzureRmNetworkWatcherConnectivity cmdlet을 업데이트하여 대상 ID, 주소 및 포트 유효성 검사를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-453">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="e4109-454">VirtualNetwork 맵의 메모리 사용 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e4109-454">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="e4109-455">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="e4109-455">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="e4109-456">보호된 파일 공유에 대한 정책을 수정하는 것에 대해 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-456">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="e4109-457">정책 표준 시간대를 대문자로 변환했습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-457">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="e4109-458">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="e4109-458">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="e4109-459">New-AzureRmRecoveryServicesAsrProtectableItem의 예제 정정</span><span class="sxs-lookup"><span data-stu-id="e4109-459">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="e4109-460">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-460">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="e4109-461">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="e4109-461">Az.Relay</span></span>
* <span data-ttu-id="e4109-462">선택적 매개 변수 -KeyValue를 New-AzureRmRelayKey cmdlet에 추가하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-462">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="e4109-463">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-463">Az.Resources</span></span>
* <span data-ttu-id="e4109-464">`New-AzureRmPolicyAssignment` 및 `Set-AzureRmPolicyAssignment`의 자원 ID 관련 매개 변수에 대한 도움말 문서를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="e4109-464">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="e4109-465">-Metadata를 사용하는 New-AzureRmPolicyDefinition에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-465">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="e4109-466">NetStandard의 태그 키에서 대소문자 보존을 허용하도록 수정: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="e4109-466">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="e4109-467">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e4109-467">Az.ServiceFabric</span></span>
* <span data-ttu-id="e4109-468">향후 호환성이 손상되는 변경에 대한 사용 중단 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-468">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="e4109-469">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e4109-469">Az.Sql</span></span>
* <span data-ttu-id="e4109-470">Azure Sql Database Managed Instance 및 Azure Sql 관리 데이터베이스에 CRUD 작업을 위한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-470">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="e4109-471">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="e4109-471">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="e4109-472">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="e4109-472">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="e4109-473">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="e4109-473">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="e4109-474">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="e4109-474">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="e4109-475">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="e4109-475">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="e4109-476">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="e4109-476">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="e4109-477">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="e4109-477">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="e4109-478">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="e4109-478">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="e4109-479">서버 또는 데이터베이스에서 확장 감사 정책 관리를 활성화했습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-479">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="e4109-480">새 매개 변수(PredicateExpression)가 감사 로그 필터링을 사용하도록 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-480">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="e4109-481">Cmdlet이 레거시 클라이언트 대신 SQL 클라이언트를 사용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-481">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="e4109-482">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="e4109-482">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="e4109-483">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="e4109-483">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="e4109-484">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="e4109-484">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="e4109-485">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="e4109-485">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="e4109-486">스토리지 계정 이름 매개 변수가 설정된 Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings를 사용할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e4109-486">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="e4109-487">0.5.0 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="e4109-487">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="e4109-488">일반</span><span class="sxs-lookup"><span data-stu-id="e4109-488">General</span></span>
* <span data-ttu-id="e4109-489">많은 핵심 cmdlet에 Resource Completers를 추가하여 대화형으로 cmdlet을 호출할 때 기존 리소스 이름을 탭으로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-489">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="e4109-490">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="e4109-490">Az.Profile</span></span>
* <span data-ttu-id="e4109-491">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-491">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="e4109-492">Connect-AzAccount cmdlet의 매개 변수 TenantId 이름을 Tenant로 바꾸고 TenantId의 별칭을 추가합니다</span><span class="sxs-lookup"><span data-stu-id="e4109-492">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="e4109-493">Connect-AzAccount의 업데이트된 TenantId 설명</span><span class="sxs-lookup"><span data-stu-id="e4109-493">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="e4109-494">테넌트 도메인을 제공할 때 실패한 로그인에 대한 오류 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-494">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="e4109-495">테넌트에 구독이 없는 계정의 컨텍스트 이름 충돌 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-495">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="e4109-496">MSI를 사용할 때 DataLake 엔드포인트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-496">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="e4109-497">연결되지 않은 경우 'Disconnect-AzAccount'가 throw하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-497">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="e4109-498">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e4109-498">Az.CognitiveServices</span></span>
* <span data-ttu-id="e4109-499">Get-AzCognitiveServicesAccountSkus 작업을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-499">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e4109-500">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e4109-500">Az.Compute</span></span>
* <span data-ttu-id="e4109-501">Add-AzVmssVMDataDisk 및 Remove-AzVmssVMDataDisk cmdlet를 추가합니다</span><span class="sxs-lookup"><span data-stu-id="e4109-501">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="e4109-502">Get-AzVMImage는 AutomaticOSUpgradeProperties를 표시합니다</span><span class="sxs-lookup"><span data-stu-id="e4109-502">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="e4109-503">수정된 SetAzVMChefExtension -BootstrapOptions 및 -JsonAttribute option 값이 json 형식으로 설정하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-503">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e4109-504">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e4109-504">Az.DataLakeStore</span></span>
* <span data-ttu-id="e4109-505">DataLake 패키지를 1.1.10으로 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-505">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="e4109-506">기본 동시성을 다중 스레드 작업에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-506">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="e4109-507">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="e4109-507">Az.Insights</span></span>
* <span data-ttu-id="e4109-508">해결된 문제 #7267(자동 크기 조정 영역)</span><span class="sxs-lookup"><span data-stu-id="e4109-508">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="e4109-509">열거된 매개 변수를 제대로 설정하지 않은 새 자동 크기 조정 규칙을 만드는 데 문제가 있습니다(이를 항상 기본값으로 설정함).</span><span class="sxs-lookup"><span data-stu-id="e4109-509">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="e4109-510">해결된 문제 # 7513[자세한 정보] Set-AzDiagnosticSetting은 설정을 생성하는 동안 범주를 명시적으로 지정해야 합니다</span><span class="sxs-lookup"><span data-stu-id="e4109-510">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="e4109-511">이제 cmdlet은 생성 중에 사용할 범주를 명시적으로 표시할 필요가 없습니다. 즉, 문서화된대로 작동합니다</span><span class="sxs-lookup"><span data-stu-id="e4109-511">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e4109-512">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e4109-512">Az.Network</span></span>
* <span data-ttu-id="e4109-513">다음 cmdlet에 대해 PeeringType을 필수 매개 변수로 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-513">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="e4109-514">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="e4109-514">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="e4109-515">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="e4109-515">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="e4109-516">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="e4109-516">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="e4109-517">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="e4109-517">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="e4109-518">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="e4109-518">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="e4109-519">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="e4109-519">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="e4109-520">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="e4109-520">Az.PolicyInsights</span></span>
* <span data-ttu-id="e4109-521">추가된 정책 재구성 cmdlet</span><span class="sxs-lookup"><span data-stu-id="e4109-521">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="e4109-522">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-522">Az.Resources</span></span>
* <span data-ttu-id="e4109-523">https://github.com/Azure/azure-powershell/issues/7402 에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-523">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="e4109-524">'Get-AzResource'에 대해 '-ResourceId' 매개 변수를 사용하여 리소스 나열 허용</span><span class="sxs-lookup"><span data-stu-id="e4109-524">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="e4109-525">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="e4109-525">Az.ServiceBus</span></span>
* <span data-ttu-id="e4109-526">마이그레이션 상태를 알 수 있도록 PSServiceBusMigrationConfigurationAttributes에 MigrationState 읽기 전용 속성 추가.</span><span class="sxs-lookup"><span data-stu-id="e4109-526">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="e4109-527">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="e4109-527">Az.ServiceFabric</span></span>
* <span data-ttu-id="e4109-528">Linux Vmss에 인증서 추가 수정.</span><span class="sxs-lookup"><span data-stu-id="e4109-528">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="e4109-529">Add-AzServiceFabricClusterCertificate 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-529">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="e4109-530">새 인증서(Azure/service-fabric-issues#932)에서 올바른 지문을 사용.</span><span class="sxs-lookup"><span data-stu-id="e4109-530">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="e4109-531">올바르게 예외 표시(Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="e4109-531">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="e4109-532">Vmss CreateOrUpdate 작업을 시작하기 전에 'Update-AzServiceFabricDurability'를 수정하여 클러스터 구성 업데이트.</span><span class="sxs-lookup"><span data-stu-id="e4109-532">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="e4109-533">0.4.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="e4109-533">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="e4109-534">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="e4109-534">Az.Profile</span></span>
* <span data-ttu-id="e4109-535">CloudShell에서 Get-AzSubscription을 사용하여 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-535">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="e4109-536">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-536">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e4109-537">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e4109-537">Az.Compute</span></span>
* <span data-ttu-id="e4109-538">'New-AzVm'에 대해 간단한 매개 변수를 사용하는 경우 가속화된 네트워킹을 설정하기 위해 새 크기가 VM 크기의 허용 목록에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-538">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="e4109-539">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-539">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="e4109-540">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="e4109-540">Az.DataLakeStore</span></span>
* <span data-ttu-id="e4109-541">Virtual Network 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-541">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="e4109-542">Get-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 가져오거나 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-542">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="e4109-543">Add-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 가상 네트워크 규칙을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-543">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="e4109-544">Set-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 지정된 가상 네트워크 규칙을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-544">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="e4109-545">Remove-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-545">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e4109-546">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e4109-546">Az.Network</span></span>
* <span data-ttu-id="e4109-547">Test-AzNetworkWatcherConnectivity cmdlet을 업데이트하고, 백 엔드에 프로토콜 값을 전달합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-547">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="e4109-548">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-548">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="e4109-549">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-549">Az.Resources</span></span>
* <span data-ttu-id="e4109-550">(기본 프로필에 구독이 없고 범위가 지정되지 않은 경우) 시나리오에서 의미 있는 예외를 추가하여 Get-AzRoleDefinition이 인식할 수 없는 예외를 throw하는 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-550">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="e4109-551">또한 기본 매개 변수 집합을 'RoleDefinitionNameParameterSet'으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-551">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="e4109-552">0.3.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="e4109-552">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="e4109-553">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="e4109-553">Azure.Storage</span></span>
* <span data-ttu-id="e4109-554">대상에 메타데이터가 있을 때 Blob/파일이 메타 데이터를 복사하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-554">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="e4109-555">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="e4109-555">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="e4109-556">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="e4109-556">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="e4109-557">특정 위치의 저장소 리소스 사용을 지원하고 글로벌 저장소 리소스 사용 가져오기는 더 이상 사용되지 않는다는 경고 메시지를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-557">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="e4109-558">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="e4109-558">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="e4109-559">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="e4109-559">Az.CognitiveServices</span></span>
* <span data-ttu-id="e4109-560">기존 계정이 없는 Get-AzCognitiveServicesAccountSkus를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-560">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="e4109-561">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="e4109-561">Az.Compute</span></span>
* <span data-ttu-id="e4109-562">Get-AzVM -ResourceGroupName <rg>가 필요한 경우 50개가 넘는 결과를 반환하도록 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-562">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="e4109-563">'SimpleParameterSet' 예제가 New-AzVmss cmdlet 도움말에 추가됨</span><span class="sxs-lookup"><span data-stu-id="e4109-563">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="e4109-564">Azure Disk Encryption 진행률 메시지의 오타를 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-564">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="e4109-565">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="e4109-565">Az.DataFactoryV2</span></span>
* <span data-ttu-id="e4109-566">ADF.Net SDK 버전을 2.3.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="e4109-566">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="e4109-567">Az.Network</span><span class="sxs-lookup"><span data-stu-id="e4109-567">Az.Network</span></span>
* <span data-ttu-id="e4109-568">NetworkProfile 기능 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-568">Added NetworkProfile functionality.</span></span> <span data-ttu-id="e4109-569">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-569">new cmdlets added</span></span>
    - <span data-ttu-id="e4109-570">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e4109-570">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="e4109-571">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e4109-571">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="e4109-572">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e4109-572">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="e4109-573">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="e4109-573">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="e4109-574">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="e4109-574">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="e4109-575">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="e4109-575">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="e4109-576">서브넷 모델에 서비스 연결 링크 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-576">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="e4109-577">New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-577">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="e4109-578">Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-578">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="e4109-579">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="e4109-579">Az.RedisCache</span></span>
* <span data-ttu-id="e4109-580">모든 문자열을 Size 매개 변수로 진행되도록 허용</span><span class="sxs-lookup"><span data-stu-id="e4109-580">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="e4109-581">PSArgumentCompleter 팝업에 P5 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-581">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="e4109-582">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="e4109-582">Az.Resources</span></span>
* <span data-ttu-id="e4109-583">-Mode 매개 변수를 Set-AzPolicyDefinition에 추가</span><span class="sxs-lookup"><span data-stu-id="e4109-583">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="e4109-584">사용자가 포함된 Origin 작업에서 Get-AzProviderOperation commandlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="e4109-584">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="e4109-585">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="e4109-585">Az.Sql</span></span>
* <span data-ttu-id="e4109-586">일부 백업 cmdlet이 현재 azure 구독을 인식하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="e4109-586">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="e4109-587">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="e4109-587">Az.Websites</span></span>
* <span data-ttu-id="e4109-588">새 cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - 컨테이너 지속적인 배포 Webhook URL을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-588">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="e4109-589">새 cmdlet New-AzWebAppContainerPSSession 및 Enter-WebAppContainerPSSession -  windows 컨테이너 앱에 PowerShell 원격 세션을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="e4109-589">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="e4109-590">0.2.0 - 2018년 9월</span><span class="sxs-lookup"><span data-stu-id="e4109-590">0.2.0 - September 2018</span></span>
 <span data-ttu-id="e4109-591">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="e4109-591">Initial Release</span></span>