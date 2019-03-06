## <a name="140---february-2019"></a><span data-ttu-id="17808-101">1.4.0 - 2019년 2월</span><span class="sxs-lookup"><span data-stu-id="17808-101">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="17808-102">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="17808-102">Az.AnalysisServices</span></span>
* <span data-ttu-id="17808-103">사용되지 않는 AddAzureASAccount cmdlet</span><span class="sxs-lookup"><span data-stu-id="17808-103">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="17808-104">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="17808-104">Az.Automation</span></span>
* <span data-ttu-id="17808-105">Import-AzAutomationDscNodeConfiguration 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-105">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="17808-106">Import-AzAutomationDscConfiguration cmdlet 구성 이름 유효성 검사 추가</span><span class="sxs-lookup"><span data-stu-id="17808-106">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="17808-107">Import-AzAutomationDscConfiguration cmdlet 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="17808-107">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="17808-108">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="17808-108">Az.CognitiveServices</span></span>
* <span data-ttu-id="17808-109">리소스의 하위 도메인을 지정하는 데 사용되는 New-AzCognitiveServicesAccount에 대한 새 선택적 매개 변수로 CustomSubdomainName이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-109">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="17808-110">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="17808-110">Az.Compute</span></span>
* <span data-ttu-id="17808-111">ID 매개 변수 집합 문제 해결</span><span class="sxs-lookup"><span data-stu-id="17808-111">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="17808-112">Name 매개 변수를 제공하지 않으면 Get-AzVMExtension이 설치된 모든 확장을 열거하도록 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-112">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="17808-113">Update-AzImage cmdlet에 태그 및 ResourceId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="17808-113">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="17808-114">인스턴스 ID가 없는 Get-AzVmssVM과 InstanceView를 사용하면 인스턴스 보기가 있는 VMSS VM을 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-114">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="17808-115">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="17808-115">Az.DataLakeStore</span></span>
* <span data-ttu-id="17808-116">ADL 삭제된 항목 열거 및 복원에 대한 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="17808-116">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="17808-117">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="17808-117">Az.EventHub</span></span>
* <span data-ttu-id="17808-118">Eventhub의 CaptureDescription 클래스에서 빈 보관을 건너뛰는 새 부울 속성 SkipEmptyArchives가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-118">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="17808-119">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="17808-119">Az.KeyVault</span></span>
* <span data-ttu-id="17808-120">Set-AzKeyVaultSecret 태그 지정 수정</span><span class="sxs-lookup"><span data-stu-id="17808-120">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="17808-121">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="17808-121">Az.LogicApp</span></span>
* <span data-ttu-id="17808-122">통합 계정에 대한 기본 sku 추가</span><span class="sxs-lookup"><span data-stu-id="17808-122">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="17808-123">XSLT 2.0, XSLT 3.0, Liquid 맵 형식 추가</span><span class="sxs-lookup"><span data-stu-id="17808-123">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="17808-124">통합 계정 어셈블리에 대한 새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="17808-124">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="17808-125">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="17808-125">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="17808-126">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="17808-126">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="17808-127">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="17808-127">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="17808-128">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="17808-128">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="17808-129">통합 계정 일괄 처리 구성에 대한 새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="17808-129">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="17808-130">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="17808-130">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="17808-131">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="17808-131">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="17808-132">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="17808-132">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="17808-133">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="17808-133">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="17808-134">논리 앱 SDK를 버전 4.1.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-134">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="17808-135">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="17808-135">Az.Monitor</span></span>
* <span data-ttu-id="17808-136">Get-AzMetric에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-136">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="17808-137">Az.Network</span><span class="sxs-lookup"><span data-stu-id="17808-137">Az.Network</span></span>
* <span data-ttu-id="17808-138">Add-AzApplicationGatewayCustomError에 대한 도움말 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-138">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="17808-139">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="17808-139">Az.OperationalInsights</span></span>
* <span data-ttu-id="17808-140">New 및 Get ApplicationInsights 데이터 소스에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="17808-140">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="17808-141">지정된 작업 영역에 대한 특정 또는 전체 ApplicationInsights 데이터 원본 가져오기를 지원하기 위한 새로운 'ApplicationInsights' 종류가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-141">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="17808-142">지정된 Application-Insights 리소스 매개 변수(구독 ID, resourceGroupName 및 이름)별로 데이터 원본을 만들기 위한 New-AzOperationalInsightsApplicationInsightsDataSource cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-142">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="17808-143">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="17808-143">Az.Resources</span></span>
* <span data-ttu-id="17808-144">문제 https://github.com/Azure/azure-powershell/issues/8166 수정</span><span class="sxs-lookup"><span data-stu-id="17808-144">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="17808-145">문제 https://github.com/Azure/azure-powershell/issues/8235 수정</span><span class="sxs-lookup"><span data-stu-id="17808-145">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="17808-146">문제 https://github.com/Azure/azure-powershell/issues/6219 수정</span><span class="sxs-lookup"><span data-stu-id="17808-146">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="17808-147">KeyCredentials 반복 만들기를 방지하기 위해 버그 수정</span><span class="sxs-lookup"><span data-stu-id="17808-147">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="17808-148">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="17808-148">Az.Sql</span></span>
* <span data-ttu-id="17808-149">SQL DB 하이퍼스케일에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="17808-149">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="17808-150">복원 요청에서 불필요한 속성을 설정하여 복원이 실패할 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="17808-150">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="17808-151">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="17808-151">Az.Websites</span></span>
* <span data-ttu-id="17808-152">Get-AzWebAppSlotMetrics 내 올바른 예제</span><span class="sxs-lookup"><span data-stu-id="17808-152">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="17808-153">1.3.0 - 2019년 2월</span><span class="sxs-lookup"><span data-stu-id="17808-153">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="17808-154">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="17808-154">Az.Accounts</span></span>
* <span data-ttu-id="17808-155">ClientRuntime 최신 버전 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-155">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="17808-156">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="17808-156">Az.AnalysisServices</span></span>
<span data-ttu-id="17808-157">Az.AnalysisServices 모듈의 전반적인 가용성.</span><span class="sxs-lookup"><span data-stu-id="17808-157">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="17808-158">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="17808-158">Az.Compute</span></span>
* <span data-ttu-id="17808-159">AEM 확장: UltraSSD 및 P60, P70, P80 디스크에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="17808-159">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="17808-160">Set-AzVMBootDiagnostics에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-160">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="17808-161">Update-AzImage에 대한 도움말 및 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-161">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="17808-162">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="17808-162">Az.RecoveryServices</span></span>
<span data-ttu-id="17808-163">Az.RecoveryServices 모듈의 전반적인 가용성.</span><span class="sxs-lookup"><span data-stu-id="17808-163">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="17808-164">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="17808-164">Az.Resources</span></span>
* <span data-ttu-id="17808-165">리소스 그룹 관련 태그 수정</span><span class="sxs-lookup"><span data-stu-id="17808-165">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="17808-166">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8166를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-166">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="17808-167">`Get-AzureRmRoleAssignment`이(가) -ErrorAction을 준수하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-167">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="17808-168">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8235를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-168">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="17808-169">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="17808-169">Az.Sql</span></span>
* <span data-ttu-id="17808-170">AzSqlDatabaseBackupShortTermRetentionPolicy 가져오기/설정하기 추가</span><span class="sxs-lookup"><span data-stu-id="17808-170">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="17808-171">SQL cmdlet을 실행할 경우 Azure 계정에 로그인되어 있지 않은 것이 nullref 예외를 초래하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-171">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="17808-172">Get-AzSqlCapability의 nullref 예외 수정</span><span class="sxs-lookup"><span data-stu-id="17808-172">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="17808-173">1.2.1 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="17808-173">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="17808-174">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="17808-174">Az.Accounts</span></span>
* <span data-ttu-id="17808-175">올바른 인증 버전을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="17808-175">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="17808-176">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="17808-176">Az.AnalysisServices</span></span>
* <span data-ttu-id="17808-177">업데이트된 인증 종속성을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="17808-177">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="17808-178">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="17808-178">Az.RecoveryServices</span></span>
* <span data-ttu-id="17808-179">업데이트된 인증 종속성을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="17808-179">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="17808-180">1.2.0 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="17808-180">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="17808-181">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="17808-181">Az.Accounts</span></span>
* <span data-ttu-id="17808-182">Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증 추가</span><span class="sxs-lookup"><span data-stu-id="17808-182">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="17808-183">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-183">Update incorrect online help URLs</span></span>
* <span data-ttu-id="17808-184">Uninstall-AzureRm 관련 PS Core에 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="17808-184">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="17808-185">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="17808-185">Az.Aks</span></span>
* <span data-ttu-id="17808-186">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-186">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="17808-187">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="17808-187">Az.Automation</span></span>
* <span data-ttu-id="17808-188">Python 2 Runbook에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-188">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="17808-189">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-189">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="17808-190">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="17808-190">Az.Cdn</span></span>
* <span data-ttu-id="17808-191">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-191">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="17808-192">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="17808-192">Az.Compute</span></span>
* <span data-ttu-id="17808-193">Invoke-AzVMReimage cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="17808-193">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="17808-194">Set-AzVmss에 TempDisk 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="17808-194">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="17808-195">New-AzVM 경고 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="17808-195">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="17808-196">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="17808-196">Az.ContainerRegistry</span></span>
* <span data-ttu-id="17808-197">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-197">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="17808-198">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="17808-198">Az.DataFactory</span></span>
* <span data-ttu-id="17808-199">ADF.Net SDK 버전이 3.0.0으로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-199">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="17808-200">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="17808-200">Az.DataLakeStore</span></span>
* <span data-ttu-id="17808-201">MSI를 사용할 때 ADLS 엔드포인트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-201">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="17808-202">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7462를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-202">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="17808-203">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-203">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="17808-204">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="17808-204">Az.IotHub</span></span>
* <span data-ttu-id="17808-205">Add-IotHubRoutingEndpoint cmdlet에 인코딩 형식을 추가하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-205">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="17808-206">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="17808-206">Az.KeyVault</span></span>
* <span data-ttu-id="17808-207">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-207">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="17808-208">Az.Network</span><span class="sxs-lookup"><span data-stu-id="17808-208">Az.Network</span></span>
* <span data-ttu-id="17808-209">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-209">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="17808-210">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="17808-210">Az.Resources</span></span>
* <span data-ttu-id="17808-211">'New-AzADAppCredential' 및 'New-AzADSpCredential' 참조 설명서의 잘못된 예제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-211">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="17808-212">리소스 그룹 배포 cmdlet 실행 전 '-TemplateFile' 매개 변수 경로가 확인되지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-212">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="17808-213">Az.Resources: New-AzureRmPolicyDefinition -Mode 기본값에 대한 올바른 설명서</span><span class="sxs-lookup"><span data-stu-id="17808-213">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="17808-214">Az.Resources: 문제 https://github.com/Azure/azure-powershell/issues/7522 수정</span><span class="sxs-lookup"><span data-stu-id="17808-214">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="17808-215">Az.Resources: 문제 https://github.com/Azure/azure-powershell/issues/5747 수정</span><span class="sxs-lookup"><span data-stu-id="17808-215">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="17808-216">'PSResourceGroupDeployment' 개체의 서식 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-216">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="17808-217">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/2123를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-217">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="17808-218">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="17808-218">Az.ServiceFabric</span></span>
* <span data-ttu-id="17808-219">인증서가 VMSS 모델에 추가되었는데도 예외가 발생할 경우 롤백합니다. 이는 버그 https://github.com/Azure/service-fabric-issues/issues/932를 수정하기 위함입니다.</span><span class="sxs-lookup"><span data-stu-id="17808-219">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="17808-220">일부 오류 메시지를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-220">Fix some error messages.</span></span>
* <span data-ttu-id="17808-221">Az로의 마이그레이션을 통해서는 작동하지 않는 New-AzServiceFabriCluster를 위해 기본값 ARM 템플릿을 가진 클러스터 만들기를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-221">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="17808-222">확장에서 클러스터 id를 확인하여 클러스터에 해당하는 VMSS에만 추가되도록 클러스터/애플리케이션 인증서 추가를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-222">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="17808-223">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="17808-223">Az.SignalR</span></span>
* <span data-ttu-id="17808-224">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-224">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="17808-225">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="17808-225">Az.Sql</span></span>
* <span data-ttu-id="17808-226">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-226">Update incorrect online help URLs</span></span>
* <span data-ttu-id="17808-227">가능한 값을 가진 LicenseType 매개 변수에 대한 매개 변수 설명이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-227">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="17808-228">유일하게 업데이트된 속성인데 작동하지 않는 관리되는 인스턴스 ID의 업데이트 수정</span><span class="sxs-lookup"><span data-stu-id="17808-228">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="17808-229">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="17808-229">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="17808-230">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="17808-230">Az.Storage</span></span>
* <span data-ttu-id="17808-231">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-231">Update incorrect online help URLs</span></span>
* <span data-ttu-id="17808-232">Premium Storage 계정이 클래식 로깅/메트릭을 지원하지 않기 때문에, Premium Storage 계정의 클래식 로깅/메트릭을 가져올/설정할 때 상세한 오류 메시지를 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-232">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="17808-233">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="17808-233">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="17808-234">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="17808-234">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="17808-235">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="17808-235">Az.TrafficManager</span></span>
* <span data-ttu-id="17808-236">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-236">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="17808-237">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="17808-237">Az.Websites</span></span>
* <span data-ttu-id="17808-238">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-238">Update incorrect online help URLs</span></span>
* <span data-ttu-id="17808-239">앱이 ASE에 호스팅되면 'New-AzWebAppSSLBinding'을 수정하여 올바른 resourcegroup+location에 인증서를 업로드합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-239">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="17808-240">'New-AzWebAppSSLBinding'을 수정하여 SSL 인증서를 앱에 바인딩하는 데 붙는 태그를 덮어쓰지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-240">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="17808-241">1.1.0 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="17808-241">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="17808-242">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="17808-242">Az.Accounts</span></span>
* <span data-ttu-id="17808-243">Enable-AzureRmAlias에 'Local' 범위 추가</span><span class="sxs-lookup"><span data-stu-id="17808-243">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="17808-244">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="17808-244">Az.Compute</span></span>
* <span data-ttu-id="17808-245">이름이 Restart/Start/Stop/Remove/Set-AzVM과 Save-AzVMImage에 설정된 ID 매개 변수에서 선택 사항이 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-245">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="17808-246">도움말 파일의 ID에 대한 설명이 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-246">Updated the description of ID in help files</span></span>
* <span data-ttu-id="17808-247">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-247">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="17808-248">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="17808-248">Az.DataLakeStore</span></span>
* <span data-ttu-id="17808-249">SDK 수정을 위해 데이터 평면의 SDK 버전을 1.1.14로 업데이트하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-249">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="17808-250">getfilestatus 및 liststatus에 대한 음수 acesstime 및 modificationtime 수정, 비동기 취소 토큰 수정</span><span class="sxs-lookup"><span data-stu-id="17808-250">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="17808-251">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="17808-251">Az.EventGrid</span></span>
* <span data-ttu-id="17808-252">2019-01-01 API 버전을 사용하도록 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-252">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="17808-253">2019-01-01 API 버전에서 새 시나리오를 지원하도록 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-253">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="17808-254">New-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="17808-254">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="17808-255">이벤트 Time-to-Live</span><span class="sxs-lookup"><span data-stu-id="17808-255">Event Time-To-Live,</span></span>
        - <span data-ttu-id="17808-256">이벤트에 대한 최대 배달 시도</span><span class="sxs-lookup"><span data-stu-id="17808-256">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="17808-257">배달 못한 편지의 엔드포인트입니다.</span><span class="sxs-lookup"><span data-stu-id="17808-257">Dead letter endpoint.</span></span>
    - <span data-ttu-id="17808-258">Update-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="17808-258">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="17808-259">이벤트 Time-to-Live</span><span class="sxs-lookup"><span data-stu-id="17808-259">Event Time-To-Live,</span></span>
        - <span data-ttu-id="17808-260">이벤트에 대한 최대 배달 시도</span><span class="sxs-lookup"><span data-stu-id="17808-260">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="17808-261">배달 못한 편지의 엔드포인트입니다.</span><span class="sxs-lookup"><span data-stu-id="17808-261">Dead letter endpoint.</span></span>
* <span data-ttu-id="17808-262">New-AzureRmEventGridSubscription 및 Update-AzureRmEventGridSubscription cmdlet의 EndpointType 옵션에 새 열거형 값(즉, storageQueue 및 hybridConnection)을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-262">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="17808-263">이벤트 구독을 생성 또는 업데이트할 때 사용자가 직접 조치를 취해야 할 경우 경고 메시지를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-263">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="17808-264">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="17808-264">Az.IotHub</span></span>
* <span data-ttu-id="17808-265">최신 버전의 Azure IotHub SDK로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="17808-265">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="17808-266">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="17808-266">Az.LogicApp</span></span>
* <span data-ttu-id="17808-267">지정된 이름이 없는 모든 Get-AzLogicApp 목록</span><span class="sxs-lookup"><span data-stu-id="17808-267">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="17808-268">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="17808-268">Az.Resources</span></span>
* <span data-ttu-id="17808-269">'Get-AzResource'에 '-ODataQuery'및 '-ResourceId' 매개 변수를 제공할 때 매개 변수 집합 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-269">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="17808-270">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7875를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-270">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="17808-271">New/Set-AzPolicyDefinition에서 -Custom 매개 변수 처리 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-271">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="17808-272">New-AzDeployment 설명서에서 오타 수정</span><span class="sxs-lookup"><span data-stu-id="17808-272">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="17808-273">'New-AzADUser'에 '-MailNickname'매개 변수가 필수 항목으로 지정됨</span><span class="sxs-lookup"><span data-stu-id="17808-273">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="17808-274">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8220를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-274">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="17808-275">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="17808-275">Az.SignalR</span></span>
* <span data-ttu-id="17808-276">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-276">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="17808-277">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="17808-277">Az.Sql</span></span>
* <span data-ttu-id="17808-278">Storage 관리 클라이언트 종속성을 일반적인 SDK 구현으로 변환했습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-278">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="17808-279">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="17808-279">Az.Storage</span></span>
* <span data-ttu-id="17808-280">Sas Token, OAuth 또는 Anonymous를 사용하여 스토리지 컨텍스트의 StorageAccountName을 실제 스토리지 계정 이름으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-280">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="17808-281">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="17808-281">New-AzStorageContext</span></span>
* <span data-ttu-id="17808-282">'-FullUri' 매개 변수를 사용하여 BLOB 스냅숏 개체의 Sas Token을 생성하고 반환된 Uri를 스냅숏 Uri로 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-282">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="17808-283">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="17808-283">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="17808-284">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="17808-284">Az.Websites</span></span>
* <span data-ttu-id="17808-285">'Get-AzDeletedWebApp'의 날짜 구문 분석 버그를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-285">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="17808-286">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-286">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="17808-287">1.0.0 - 2018년 12월</span><span class="sxs-lookup"><span data-stu-id="17808-287">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="17808-288">일반</span><span class="sxs-lookup"><span data-stu-id="17808-288">General</span></span>

- <span data-ttu-id="17808-289">Az 모듈 일반 공급</span><span class="sxs-lookup"><span data-stu-id="17808-289">General Availability of Az Module</span></span>
- <span data-ttu-id="17808-290">각 모듈에 대 한 온라인 도움말</span><span class="sxs-lookup"><span data-stu-id="17808-290">Online help for each module</span></span>
- <span data-ttu-id="17808-291">자세한 내용과 로드맵은 [Az 알림 페이지](https://aka.ms/azps-announce)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-291">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="17808-292">AzureRM에서 마이그레이션하는 것에 대한 정보는 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-292">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="17808-293">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="17808-293">Az.Accounts</span></span>
- <span data-ttu-id="17808-294">Az.Profile에서 변경</span><span class="sxs-lookup"><span data-stu-id="17808-294">Changed from Az.Profile</span></span>
- <span data-ttu-id="17808-295">프로필 및 컨텍스트 형식에 대한 표 형식 수정</span><span class="sxs-lookup"><span data-stu-id="17808-295">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="17808-296">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="17808-296">Az.ApiManagement</span></span>
- <span data-ttu-id="17808-297">#7002에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="17808-297">Fixes for #7002</span></span>
- <span data-ttu-id="17808-298">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-298">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="17808-299">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="17808-299">Az.Batch</span></span>
- <span data-ttu-id="17808-300">`PSComputeNode`의 새로운 `NodeAgentInformation` 속성을 통해 풀의 각 VM에서 실행 중인 Azure Batch 노드 에이전트의 버전을 확인하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-300">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="17808-301">`PSDataDisk`에 대한 `Caching` 기본 값은 이제 `None` 대신 `ReadWrite`입니다.</span><span class="sxs-lookup"><span data-stu-id="17808-301">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="17808-302">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-302">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="17808-303">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="17808-303">Az.Billing</span></span>
- <span data-ttu-id="17808-304">청구, 소비 및 UsageAggregates cmdlet 결합 cmdlet에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-304">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="17808-305">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="17808-305">Az.CognitivServices</span></span>
- <span data-ttu-id="17808-306">New-AzureRmCognitiveServicesAccount 작업에서 사용 가능한 SkuName 및 Typem에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="17808-306">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="17808-307">Get-AzCognitiveServicesAccountSkus에서 GetSkusWithAccountParamSetName 매개 변수 집합을 제거</span><span class="sxs-lookup"><span data-stu-id="17808-307">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="17808-308">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="17808-308">Az.ContainerInstance</span></span>
- <span data-ttu-id="17808-309">ManagedIdentity 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="17808-309">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="17808-310">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="17808-310">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="17808-311">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-311">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="17808-312">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="17808-312">Az.DataLakeStore</span></span>
- <span data-ttu-id="17808-313">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-313">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="17808-314">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="17808-314">Az.Monitor</span></span>
- <span data-ttu-id="17808-315">Az.Monitor 이름 변경 및 기타 사소한 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-315">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="17808-316">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="17808-316">Az.KeyVault</span></span>
- <span data-ttu-id="17808-317">출력 형식에서 사용되지 않는 'PurgeDisabled' 속성 제거</span><span class="sxs-lookup"><span data-stu-id="17808-317">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="17808-318">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="17808-318">Az.MachineLearning</span></span>
- <span data-ttu-id="17808-319">Az.MachineLearningCompute 모듈의 cmdlet 포함</span><span class="sxs-lookup"><span data-stu-id="17808-319">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="17808-320">Az.Media</span><span class="sxs-lookup"><span data-stu-id="17808-320">Az.Media</span></span>
- <span data-ttu-id="17808-321">New-AzMediaService에서 사용되지 않는 -Tags 별칭이 제거됨</span><span class="sxs-lookup"><span data-stu-id="17808-321">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="17808-322">Az.Network</span><span class="sxs-lookup"><span data-stu-id="17808-322">Az.Network</span></span>
<span data-ttu-id="17808-323">Application Gateway에서 RewriteRuleSets를 구성하는 것에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="17808-323">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="17808-324">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-324">New cmdlets added:</span></span>
        - <span data-ttu-id="17808-325">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="17808-325">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="17808-326">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="17808-326">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="17808-327">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="17808-327">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="17808-328">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="17808-328">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="17808-329">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="17808-329">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="17808-330">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="17808-330">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="17808-331">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="17808-331">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="17808-332">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="17808-332">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="17808-333">선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="17808-333">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="17808-334">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="17808-334">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="17808-335">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="17808-335">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="17808-336">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="17808-336">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="17808-337">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="17808-337">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="17808-338">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="17808-338">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="17808-339">New-AzureRmApplicationGatewayUrlPathMapConfig로 ID를 사용하여 Application Gateway에 KeyVault 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-339">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="17808-340">선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="17808-340">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="17808-341">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="17808-341">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="17808-342">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="17808-342">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="17808-343">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="17808-343">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="17808-344">New-AzApplicationGateway cmdlet이 선택적 매개 변수를 사용하도록 업데이트됨 -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="17808-344">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="17808-345">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-345">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="17808-346">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="17808-346">Az.OperationalInsights</span></span>
- <span data-ttu-id="17808-347">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-347">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="17808-348">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="17808-348">Az.Profile</span></span>
- <span data-ttu-id="17808-349">Az.Accounts에 모듈 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="17808-349">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="17808-350">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="17808-350">Az.RecoveryServices</span></span>
- <span data-ttu-id="17808-351">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-351">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="17808-352">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="17808-352">Az.Resources</span></span>
- <span data-ttu-id="17808-353">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-353">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="17808-354">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="17808-354">Az.ServiceFabric</span></span>
- <span data-ttu-id="17808-355">일반 이름과 지문으로 지정 인증서 지원</span><span class="sxs-lookup"><span data-stu-id="17808-355">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="17808-356">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-356">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="17808-357">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="17808-357">Az.SIgnalR</span></span>
- <span data-ttu-id="17808-358">SIgnalR에 대한 PowerShell cmdlet에 대한 일반 공급</span><span class="sxs-lookup"><span data-stu-id="17808-358">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="17808-359">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="17808-359">Az.Sql</span></span>
- <span data-ttu-id="17808-360">위협 탐지의 cmdlet에 새로운 Data_Exfiltration 및 Unsafe_Action 검색 유형 추가</span><span class="sxs-lookup"><span data-stu-id="17808-360">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="17808-361">Sql 감사 cmdlet에 대한 설명서 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-361">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="17808-362">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-362">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="17808-363">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="17808-363">Az.Storage</span></span>
- <span data-ttu-id="17808-364">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-364">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="17808-365">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="17808-365">Az.Websites</span></span>
- <span data-ttu-id="17808-366">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="17808-366">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="17808-367">0.7.0 - 2018년 12월</span><span class="sxs-lookup"><span data-stu-id="17808-367">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="17808-368">일반</span><span class="sxs-lookup"><span data-stu-id="17808-368">General</span></span>

* <span data-ttu-id="17808-369">AzureRM에서 Az 전환 예정에 대한 사소한 변경</span><span class="sxs-lookup"><span data-stu-id="17808-369">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="17808-370">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="17808-370">Az.Compute</span></span>

* <span data-ttu-id="17808-371">`New-AzVm(ss)` cmdlet에 대한 간단한 매개 변수 집합에 UltraSSD 및 갤러리 이미지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-371">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="17808-372">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="17808-372">Az.DataLakeStore</span></span>

* <span data-ttu-id="17808-373">ADLS 계정의 도메인의 후행 슬래시를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-373">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="17808-374">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="17808-374">Az.FrontDoor</span></span>

* <span data-ttu-id="17808-375">일부 끊어진 링크 수정</span><span class="sxs-lookup"><span data-stu-id="17808-375">Fixed some broken links</span></span>
    - <span data-ttu-id="17808-376">New-AzureRmFrontDoor 및 Set-AzureRmFrontDoor 아티클에서 New-AzureRmFrontDoorHealthProbeSettingObject cmdlet 아티클에 대한 링크가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-376">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="17808-377">New-AzureRmFrontDoorManagedRuleObject 아티클에서 New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet 아티클에 대한 링크가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-377">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="17808-378">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="17808-378">Az.RecoveryServices</span></span>

* <span data-ttu-id="17808-379">Azure File Share 복원 작업에 클라이언트 측 유효성 검사가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-379">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="17808-380">afs 복원의 경우 storageAccountName 및 storageAccountResourceGroupName을 선택적으로 만들었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-380">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="17808-381">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="17808-381">Az.Resources</span></span>

* <span data-ttu-id="17808-382">https://github.com/Azure/azure-powershell/issues/7679 에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="17808-382">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="17808-383">기본 관리자를 요청할 때 구독 범위가 제공되는 경우 Get-AzureRmRoleAssignment를 업데이트하여 구독 범위를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-383">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="17808-384">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="17808-384">Az.Sql</span></span>

* <span data-ttu-id="17808-385">AzureRM에서 Az 전환 예정에 대한 사소한 변경</span><span class="sxs-lookup"><span data-stu-id="17808-385">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="17808-386">DotNet 코어에서 Get-AzureRmSqlDatabaseVulnerabilityAssessment를 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="17808-386">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="17808-387">SQL 감사 cmdlet과 관련된 도움말 메시지의 설명서가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-387">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="17808-388">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="17808-388">Az.Storage</span></span>

* <span data-ttu-id="17808-389">New-AzureRmStorageAccount에 -EnableHierarchicalNamespace 추가</span><span class="sxs-lookup"><span data-stu-id="17808-389">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="17808-390">파일 복사 cmdlet이 -DestContext 입력이 없을 때 대상의 원본 컨텍스트를 다시 사용할 수 없는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-390">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="17808-391">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="17808-391">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="17808-392">고정적인 웹 사이트 구성 지원</span><span class="sxs-lookup"><span data-stu-id="17808-392">Support Static Website configuration</span></span>
    - <span data-ttu-id="17808-393">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="17808-393">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="17808-394">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="17808-394">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="17808-395">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="17808-395">Az.Websites</span></span>

* <span data-ttu-id="17808-396">Set-AzureRmWebApp 및 Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="17808-396">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="17808-397">Windows 및 Linux 컨테이너 응용 프로그램에 탑재할 Azure Storage 경로를 지정하기 위해 새 매개 변수(-AzureStoragePath)가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-397">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="17808-398">새 cmdlet New-AzureRmWebAppAzureStoragePath의 출력을 매개 변수로 사용하여 Azure Storage 경로를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-398">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="17808-399">0.6.1 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="17808-399">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="17808-400">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="17808-400">Az.ApiManagement</span></span>
* <span data-ttu-id="17808-401">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-401">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="17808-402">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="17808-402">Az.Automation</span></span>
* <span data-ttu-id="17808-403">Azure Automation cmdlet 기반 Swagger</span><span class="sxs-lookup"><span data-stu-id="17808-403">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="17808-404">업데이트 관리 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="17808-404">Added Update Management cmdlets</span></span>
* <span data-ttu-id="17808-405">소스 제어 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="17808-405">Added Source Control cmdlets</span></span>
* <span data-ttu-id="17808-406">Remove-AzureRmAutomationHybridWorkerGroup cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="17808-406">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="17808-407">DSC 노드 등록 명령 수정</span><span class="sxs-lookup"><span data-stu-id="17808-407">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="17808-408">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="17808-408">Az.Compute</span></span>
* <span data-ttu-id="17808-409">SystemAssigned ID에 대한 ID 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-409">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="17808-410">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-410">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="17808-411">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="17808-411">Az.ContainerInstance</span></span>
* <span data-ttu-id="17808-412">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-412">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="17808-413">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="17808-413">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="17808-414">마켓플레이스 cmdlet에 대한 예제 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-414">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="17808-415">Az.Network</span><span class="sxs-lookup"><span data-stu-id="17808-415">Az.Network</span></span>
* <span data-ttu-id="17808-416">New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="17808-416">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="17808-417">지원되는 AzureFirewall 네트워크 프로토콜에 ICMP 다시 추가</span><span class="sxs-lookup"><span data-stu-id="17808-417">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="17808-418">Test-AzureRmNetworkWatcherConnectivity cmdlet을 업데이트하여 대상 ID, 주소 및 포트 유효성 검사를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-418">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="17808-419">VirtualNetwork 맵의 메모리 사용 문제 해결</span><span class="sxs-lookup"><span data-stu-id="17808-419">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="17808-420">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="17808-420">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="17808-421">보호된 파일 공유에 대한 정책을 수정하는 것에 대해 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-421">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="17808-422">정책 표준 시간대를 대문자로 변환했습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-422">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="17808-423">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="17808-423">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="17808-424">New-AzureRmRecoveryServicesAsrProtectableItem의 예제 정정</span><span class="sxs-lookup"><span data-stu-id="17808-424">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="17808-425">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-425">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="17808-426">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="17808-426">Az.Relay</span></span>
* <span data-ttu-id="17808-427">선택적 매개 변수 -KeyValue를 New-AzureRmRelayKey cmdlet에 추가하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-427">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="17808-428">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="17808-428">Az.Resources</span></span>
* <span data-ttu-id="17808-429">`New-AzureRmPolicyAssignment` 및 `Set-AzureRmPolicyAssignment`의 자원 ID 관련 매개 변수에 대한 도움말 문서를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="17808-429">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="17808-430">-Metadata를 사용하는 New-AzureRmPolicyDefinition에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="17808-430">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="17808-431">NetStandard의 태그 키에서 대소문자 보존을 허용하도록 수정: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="17808-431">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="17808-432">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="17808-432">Az.ServiceFabric</span></span>
* <span data-ttu-id="17808-433">향후 호환성이 손상되는 변경에 대한 사용 중단 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="17808-433">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="17808-434">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="17808-434">Az.Sql</span></span>
* <span data-ttu-id="17808-435">Azure Sql Database Managed Instance 및 Azure Sql 관리 데이터베이스에 CRUD 작업을 위한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="17808-435">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="17808-436">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="17808-436">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="17808-437">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="17808-437">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="17808-438">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="17808-438">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="17808-439">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="17808-439">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="17808-440">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="17808-440">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="17808-441">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="17808-441">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="17808-442">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="17808-442">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="17808-443">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="17808-443">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="17808-444">서버 또는 데이터베이스에서 확장 감사 정책 관리를 활성화했습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-444">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="17808-445">새 매개 변수(PredicateExpression)가 감사 로그 필터링을 사용하도록 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-445">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="17808-446">Cmdlet이 레거시 클라이언트 대신 SQL 클라이언트를 사용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-446">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="17808-447">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="17808-447">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="17808-448">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="17808-448">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="17808-449">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="17808-449">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="17808-450">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="17808-450">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="17808-451">스토리지 계정 이름 매개 변수가 설정된 Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings를 사용할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="17808-451">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="17808-452">0.5.0 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="17808-452">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="17808-453">일반</span><span class="sxs-lookup"><span data-stu-id="17808-453">General</span></span>
* <span data-ttu-id="17808-454">많은 핵심 cmdlet에 Resource Completers를 추가하여 대화형으로 cmdlet을 호출할 때 기존 리소스 이름을 탭으로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-454">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="17808-455">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="17808-455">Az.Profile</span></span>
* <span data-ttu-id="17808-456">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-456">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="17808-457">Connect-AzAccount cmdlet의 매개 변수 TenantId 이름을 Tenant로 바꾸고 TenantId의 별칭을 추가합니다</span><span class="sxs-lookup"><span data-stu-id="17808-457">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="17808-458">Connect-AzAccount의 업데이트된 TenantId 설명</span><span class="sxs-lookup"><span data-stu-id="17808-458">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="17808-459">테넌트 도메인을 제공할 때 실패한 로그인에 대한 오류 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="17808-459">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="17808-460">테넌트에 구독이 없는 계정의 컨텍스트 이름 충돌 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-460">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="17808-461">MSI를 사용할 때 DataLake 엔드포인트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-461">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="17808-462">연결되지 않은 경우 'Disconnect-AzAccount'가 throw하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-462">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="17808-463">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="17808-463">Az.CognitiveServices</span></span>
* <span data-ttu-id="17808-464">Get-AzCognitiveServicesAccountSkus 작업을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-464">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="17808-465">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="17808-465">Az.Compute</span></span>
* <span data-ttu-id="17808-466">Add-AzVmssVMDataDisk 및 Remove-AzVmssVMDataDisk cmdlet를 추가합니다</span><span class="sxs-lookup"><span data-stu-id="17808-466">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="17808-467">Get-AzVMImage는 AutomaticOSUpgradeProperties를 표시합니다</span><span class="sxs-lookup"><span data-stu-id="17808-467">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="17808-468">수정된 SetAzVMChefExtension -BootstrapOptions 및 -JsonAttribute option 값이 json 형식으로 설정하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-468">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="17808-469">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="17808-469">Az.DataLakeStore</span></span>
* <span data-ttu-id="17808-470">DataLake 패키지를 1.1.10으로 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-470">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="17808-471">기본 동시성을 다중 스레드 작업에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-471">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="17808-472">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="17808-472">Az.Insights</span></span>
* <span data-ttu-id="17808-473">해결된 문제 #7267(자동 크기 조정 영역)</span><span class="sxs-lookup"><span data-stu-id="17808-473">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="17808-474">열거된 매개 변수를 제대로 설정하지 않은 새 자동 크기 조정 규칙을 만드는 데 문제가 있습니다(이를 항상 기본값으로 설정함).</span><span class="sxs-lookup"><span data-stu-id="17808-474">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="17808-475">해결된 문제 # 7513[자세한 정보] Set-AzDiagnosticSetting은 설정을 생성하는 동안 범주를 명시적으로 지정해야 합니다</span><span class="sxs-lookup"><span data-stu-id="17808-475">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="17808-476">이제 cmdlet은 생성 중에 사용할 범주를 명시적으로 표시할 필요가 없습니다. 즉, 문서화된대로 작동합니다</span><span class="sxs-lookup"><span data-stu-id="17808-476">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="17808-477">Az.Network</span><span class="sxs-lookup"><span data-stu-id="17808-477">Az.Network</span></span>
* <span data-ttu-id="17808-478">다음 cmdlet에 대해 PeeringType을 필수 매개 변수로 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-478">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="17808-479">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="17808-479">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="17808-480">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="17808-480">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="17808-481">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="17808-481">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="17808-482">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="17808-482">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="17808-483">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="17808-483">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="17808-484">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="17808-484">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="17808-485">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="17808-485">Az.PolicyInsights</span></span>
* <span data-ttu-id="17808-486">추가된 정책 재구성 cmdlet</span><span class="sxs-lookup"><span data-stu-id="17808-486">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="17808-487">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="17808-487">Az.Resources</span></span>
* <span data-ttu-id="17808-488">https://github.com/Azure/azure-powershell/issues/7402 에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="17808-488">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="17808-489">'Get-AzResource'에 대해 '-ResourceId' 매개 변수를 사용하여 리소스 나열 허용</span><span class="sxs-lookup"><span data-stu-id="17808-489">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="17808-490">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="17808-490">Az.ServiceBus</span></span>
* <span data-ttu-id="17808-491">마이그레이션 상태를 알 수 있도록 PSServiceBusMigrationConfigurationAttributes에 MigrationState 읽기 전용 속성 추가.</span><span class="sxs-lookup"><span data-stu-id="17808-491">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="17808-492">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="17808-492">Az.ServiceFabric</span></span>
* <span data-ttu-id="17808-493">Linux Vmss에 인증서 추가 수정.</span><span class="sxs-lookup"><span data-stu-id="17808-493">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="17808-494">Add-AzServiceFabricClusterCertificate 수정</span><span class="sxs-lookup"><span data-stu-id="17808-494">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="17808-495">새 인증서(Azure/service-fabric-issues#932)에서 올바른 지문을 사용.</span><span class="sxs-lookup"><span data-stu-id="17808-495">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="17808-496">올바르게 예외 표시(Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="17808-496">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="17808-497">Vmss CreateOrUpdate 작업을 시작하기 전에 'Update-AzServiceFabricDurability'를 수정하여 클러스터 구성 업데이트.</span><span class="sxs-lookup"><span data-stu-id="17808-497">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="17808-498">0.4.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="17808-498">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="17808-499">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="17808-499">Az.Profile</span></span>
* <span data-ttu-id="17808-500">CloudShell에서 Get-AzSubscription을 사용하여 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-500">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="17808-501">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-501">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="17808-502">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="17808-502">Az.Compute</span></span>
* <span data-ttu-id="17808-503">'New-AzVm'에 대해 간단한 매개 변수를 사용하는 경우 가속화된 네트워킹을 설정하기 위해 새 크기가 VM 크기의 허용 목록에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-503">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="17808-504">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-504">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="17808-505">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="17808-505">Az.DataLakeStore</span></span>
* <span data-ttu-id="17808-506">Virtual Network 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="17808-506">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="17808-507">Get-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 가져오거나 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-507">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="17808-508">Add-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 가상 네트워크 규칙을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-508">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="17808-509">Set-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 지정된 가상 네트워크 규칙을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-509">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="17808-510">Remove-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-510">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="17808-511">Az.Network</span><span class="sxs-lookup"><span data-stu-id="17808-511">Az.Network</span></span>
* <span data-ttu-id="17808-512">Test-AzNetworkWatcherConnectivity cmdlet을 업데이트하고, 백 엔드에 프로토콜 값을 전달합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-512">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="17808-513">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-513">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="17808-514">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="17808-514">Az.Resources</span></span>
* <span data-ttu-id="17808-515">(기본 프로필에 구독이 없고 범위가 지정되지 않은 경우) 시나리오에서 의미 있는 예외를 추가하여 Get-AzRoleDefinition이 인식할 수 없는 예외를 throw하는 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-515">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="17808-516">또한 기본 매개 변수 집합을 'RoleDefinitionNameParameterSet'으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-516">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="17808-517">0.3.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="17808-517">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="17808-518">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="17808-518">Azure.Storage</span></span>
* <span data-ttu-id="17808-519">대상에 메타데이터가 있을 때 Blob/파일이 메타 데이터를 복사하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="17808-519">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="17808-520">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="17808-520">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="17808-521">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="17808-521">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="17808-522">특정 위치의 저장소 리소스 사용을 지원하고 글로벌 저장소 리소스 사용 가져오기는 더 이상 사용되지 않는다는 경고 메시지를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-522">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="17808-523">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="17808-523">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="17808-524">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="17808-524">Az.CognitiveServices</span></span>
* <span data-ttu-id="17808-525">기존 계정이 없는 Get-AzCognitiveServicesAccountSkus를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-525">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="17808-526">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="17808-526">Az.Compute</span></span>
* <span data-ttu-id="17808-527">Get-AzVM -ResourceGroupName <rg>가 필요한 경우 50개가 넘는 결과를 반환하도록 수정</span><span class="sxs-lookup"><span data-stu-id="17808-527">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="17808-528">'SimpleParameterSet' 예제가 New-AzVmss cmdlet 도움말에 추가됨</span><span class="sxs-lookup"><span data-stu-id="17808-528">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="17808-529">Azure Disk Encryption 진행률 메시지의 오타를 수정</span><span class="sxs-lookup"><span data-stu-id="17808-529">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="17808-530">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="17808-530">Az.DataFactoryV2</span></span>
* <span data-ttu-id="17808-531">ADF.Net SDK 버전을 2.3.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="17808-531">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="17808-532">Az.Network</span><span class="sxs-lookup"><span data-stu-id="17808-532">Az.Network</span></span>
* <span data-ttu-id="17808-533">NetworkProfile 기능 추가</span><span class="sxs-lookup"><span data-stu-id="17808-533">Added NetworkProfile functionality.</span></span> <span data-ttu-id="17808-534">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="17808-534">new cmdlets added</span></span>
    - <span data-ttu-id="17808-535">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="17808-535">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="17808-536">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="17808-536">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="17808-537">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="17808-537">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="17808-538">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="17808-538">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="17808-539">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="17808-539">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="17808-540">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="17808-540">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="17808-541">서브넷 모델에 서비스 연결 링크 추가</span><span class="sxs-lookup"><span data-stu-id="17808-541">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="17808-542">New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="17808-542">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="17808-543">Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="17808-543">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="17808-544">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="17808-544">Az.RedisCache</span></span>
* <span data-ttu-id="17808-545">모든 문자열을 Size 매개 변수로 진행되도록 허용</span><span class="sxs-lookup"><span data-stu-id="17808-545">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="17808-546">PSArgumentCompleter 팝업에 P5 추가</span><span class="sxs-lookup"><span data-stu-id="17808-546">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="17808-547">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="17808-547">Az.Resources</span></span>
* <span data-ttu-id="17808-548">-Mode 매개 변수를 Set-AzPolicyDefinition에 추가</span><span class="sxs-lookup"><span data-stu-id="17808-548">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="17808-549">사용자가 포함된 Origin 작업에서 Get-AzProviderOperation commandlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="17808-549">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="17808-550">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="17808-550">Az.Sql</span></span>
* <span data-ttu-id="17808-551">일부 백업 cmdlet이 현재 azure 구독을 인식하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="17808-551">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="17808-552">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="17808-552">Az.Websites</span></span>
* <span data-ttu-id="17808-553">새 cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - 컨테이너 지속적인 배포 Webhook URL을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="17808-553">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="17808-554">새 cmdlet New-AzWebAppContainerPSSession 및 Enter-WebAppContainerPSSession -  windows 컨테이너 앱에 PowerShell 원격 세션을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="17808-554">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="17808-555">0.2.0 - 2018년 9월</span><span class="sxs-lookup"><span data-stu-id="17808-555">0.2.0 - September 2018</span></span>
 <span data-ttu-id="17808-556">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="17808-556">Initial Release</span></span>