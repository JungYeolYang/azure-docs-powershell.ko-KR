## <a name="100---december-2018"></a><span data-ttu-id="2dff5-101">1.0.0 - 2018년 12월</span><span class="sxs-lookup"><span data-stu-id="2dff5-101">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="2dff5-102">일반</span><span class="sxs-lookup"><span data-stu-id="2dff5-102">General</span></span>

- <span data-ttu-id="2dff5-103">Az 모듈 일반 공급</span><span class="sxs-lookup"><span data-stu-id="2dff5-103">General Availability of Az Module</span></span>
- <span data-ttu-id="2dff5-104">각 모듈에 대 한 온라인 도움말</span><span class="sxs-lookup"><span data-stu-id="2dff5-104">Online help for each module</span></span>
- <span data-ttu-id="2dff5-105">자세한 내용과 로드맵은 [Az 알림 페이지](https://aka.ms/azps-announce)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-105">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="2dff5-106">AzureRM에서 마이그레이션하는 것에 대한 정보는 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-106">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="2dff5-107">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2dff5-107">Az.Accounts</span></span>
- <span data-ttu-id="2dff5-108">Az.Profile에서 변경</span><span class="sxs-lookup"><span data-stu-id="2dff5-108">Changed from Az.Profile</span></span>
- <span data-ttu-id="2dff5-109">프로필 및 컨텍스트 형식에 대한 표 형식 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-109">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="2dff5-110">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2dff5-110">Az.ApiManagement</span></span>
- <span data-ttu-id="2dff5-111">#7002에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-111">Fixes for #7002</span></span>
- <span data-ttu-id="2dff5-112">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-112">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="2dff5-113">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="2dff5-113">Az.Batch</span></span>
- <span data-ttu-id="2dff5-114">`PSComputeNode`의 새로운 `NodeAgentInformation` 속성을 통해 풀의 각 VM에서 실행 중인 Azure Batch 노드 에이전트의 버전을 확인하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-114">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="2dff5-115">`PSDataDisk`에 대한 `Caching` 기본 값은 이제 `None` 대신 `ReadWrite`입니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-115">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="2dff5-116">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-116">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="2dff5-117">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="2dff5-117">Az.Billing</span></span>
- <span data-ttu-id="2dff5-118">청구, 소비 및 UsageAggregates cmdlet 결합 cmdlet에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-118">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="2dff5-119">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="2dff5-119">Az.CognitivServices</span></span>
- <span data-ttu-id="2dff5-120">New-AzureRmCognitiveServicesAccount 작업에서 사용 가능한 SkuName 및 Typem에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-120">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="2dff5-121">Get-AzCognitiveServicesAccountSkus에서 GetSkusWithAccountParamSetName 매개 변수 집합을 제거</span><span class="sxs-lookup"><span data-stu-id="2dff5-121">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="2dff5-122">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="2dff5-122">Az.ContainerInstance</span></span>
- <span data-ttu-id="2dff5-123">ManagedIdentity 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="2dff5-123">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="2dff5-124">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="2dff5-124">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="2dff5-125">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-125">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="2dff5-126">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2dff5-126">Az.DataLakeStore</span></span>
- <span data-ttu-id="2dff5-127">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-127">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="2dff5-128">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2dff5-128">Az.Monitor</span></span>
- <span data-ttu-id="2dff5-129">Az.Monitor 이름 변경 및 기타 사소한 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-129">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="2dff5-130">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2dff5-130">Az.KeyVault</span></span>
- <span data-ttu-id="2dff5-131">출력 형식에서 사용되지 않는 'PurgeDisabled' 속성 제거</span><span class="sxs-lookup"><span data-stu-id="2dff5-131">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="2dff5-132">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="2dff5-132">Az.MachineLearning</span></span>
- <span data-ttu-id="2dff5-133">Az.MachineLearningCompute 모듈의 cmdlet 포함</span><span class="sxs-lookup"><span data-stu-id="2dff5-133">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="2dff5-134">Az.Media</span><span class="sxs-lookup"><span data-stu-id="2dff5-134">Az.Media</span></span>
- <span data-ttu-id="2dff5-135">New-AzMediaService에서 사용되지 않는 -Tags 별칭이 제거됨</span><span class="sxs-lookup"><span data-stu-id="2dff5-135">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="2dff5-136">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2dff5-136">Az.Network</span></span>
<span data-ttu-id="2dff5-137">Application Gateway에서 RewriteRuleSets를 구성하는 것에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="2dff5-137">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="2dff5-138">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-138">New cmdlets added:</span></span>
        - <span data-ttu-id="2dff5-139">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2dff5-139">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="2dff5-140">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2dff5-140">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="2dff5-141">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2dff5-141">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="2dff5-142">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2dff5-142">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="2dff5-143">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2dff5-143">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="2dff5-144">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="2dff5-144">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="2dff5-145">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="2dff5-145">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="2dff5-146">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="2dff5-146">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="2dff5-147">선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2dff5-147">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="2dff5-148">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="2dff5-148">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="2dff5-149">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="2dff5-149">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="2dff5-150">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="2dff5-150">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="2dff5-151">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2dff5-151">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="2dff5-152">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="2dff5-152">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="2dff5-153">New-AzureRmApplicationGatewayUrlPathMapConfig로 ID를 사용하여 Application Gateway에 KeyVault 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-153">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="2dff5-154">선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="2dff5-154">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="2dff5-155">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="2dff5-155">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="2dff5-156">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="2dff5-156">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="2dff5-157">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="2dff5-157">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="2dff5-158">New-AzApplicationGateway cmdlet이 선택적 매개 변수를 사용하도록 업데이트됨 -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="2dff5-158">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="2dff5-159">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-159">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="2dff5-160">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2dff5-160">Az.OperationalInsights</span></span>
- <span data-ttu-id="2dff5-161">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-161">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="2dff5-162">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="2dff5-162">Az.Profile</span></span>
- <span data-ttu-id="2dff5-163">Az.Accounts에 모듈 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="2dff5-163">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="2dff5-164">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2dff5-164">Az.RecoveryServices</span></span>
- <span data-ttu-id="2dff5-165">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-165">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="2dff5-166">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2dff5-166">Az.Resources</span></span>
- <span data-ttu-id="2dff5-167">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-167">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="2dff5-168">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2dff5-168">Az.ServiceFabric</span></span>
- <span data-ttu-id="2dff5-169">일반 이름과 지문으로 지정 인증서 지원</span><span class="sxs-lookup"><span data-stu-id="2dff5-169">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="2dff5-170">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-170">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="2dff5-171">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="2dff5-171">Az.SIgnalR</span></span>
- <span data-ttu-id="2dff5-172">SIgnalR에 대한 PowerShell cmdlet에 대한 일반 공급</span><span class="sxs-lookup"><span data-stu-id="2dff5-172">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="2dff5-173">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2dff5-173">Az.Sql</span></span>
- <span data-ttu-id="2dff5-174">위협 탐지의 cmdlet에 새로운 Data_Exfiltration 및 Unsafe_Action 검색 유형 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-174">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="2dff5-175">Sql 감사 cmdlet에 대한 설명서 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="2dff5-175">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="2dff5-176">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-176">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="2dff5-177">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2dff5-177">Az.Storage</span></span>
- <span data-ttu-id="2dff5-178">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-178">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="2dff5-179">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2dff5-179">Az.Websites</span></span>
- <span data-ttu-id="2dff5-180">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="2dff5-180">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="2dff5-181">0.7.0 - 2018년 12월</span><span class="sxs-lookup"><span data-stu-id="2dff5-181">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="2dff5-182">일반</span><span class="sxs-lookup"><span data-stu-id="2dff5-182">General</span></span>

* <span data-ttu-id="2dff5-183">AzureRM에서 Az 전환 예정에 대한 사소한 변경</span><span class="sxs-lookup"><span data-stu-id="2dff5-183">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="2dff5-184">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2dff5-184">Az.Compute</span></span>

* <span data-ttu-id="2dff5-185">`New-AzVm(ss)` cmdlet에 대한 간단한 매개 변수 집합에 UltraSSD 및 갤러리 이미지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-185">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="2dff5-186">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2dff5-186">Az.DataLakeStore</span></span>

* <span data-ttu-id="2dff5-187">ADLS 계정의 도메인의 후행 슬래시를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-187">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="2dff5-188">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="2dff5-188">Az.FrontDoor</span></span>

* <span data-ttu-id="2dff5-189">일부 끊어진 링크 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-189">Fixed some broken links</span></span>
    - <span data-ttu-id="2dff5-190">New-AzureRmFrontDoor 및 Set-AzureRmFrontDoor 아티클에서 New-AzureRmFrontDoorHealthProbeSettingObject cmdlet 아티클에 대한 링크가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-190">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="2dff5-191">New-AzureRmFrontDoorManagedRuleObject 아티클에서 New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet 아티클에 대한 링크가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-191">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="2dff5-192">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2dff5-192">Az.RecoveryServices</span></span>

* <span data-ttu-id="2dff5-193">Azure File Share 복원 작업에 클라이언트 측 유효성 검사가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-193">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="2dff5-194">afs 복원의 경우 storageAccountName 및 storageAccountResourceGroupName을 선택적으로 만들었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-194">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="2dff5-195">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2dff5-195">Az.Resources</span></span>

* <span data-ttu-id="2dff5-196">https://github.com/Azure/azure-powershell/issues/7679에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-196">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="2dff5-197">기본 관리자를 요청할 때 구독 범위가 제공되는 경우 Get-AzureRmRoleAssignment를 업데이트하여 구독 범위를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-197">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="2dff5-198">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2dff5-198">Az.Sql</span></span>

* <span data-ttu-id="2dff5-199">AzureRM에서 Az 전환 예정에 대한 사소한 변경</span><span class="sxs-lookup"><span data-stu-id="2dff5-199">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="2dff5-200">DotNet 코어에서 Get-AzureRmSqlDatabaseVulnerabilityAssessment를 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="2dff5-200">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="2dff5-201">SQL 감사 cmdlet과 관련된 도움말 메시지의 설명서가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-201">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="2dff5-202">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2dff5-202">Az.Storage</span></span>

* <span data-ttu-id="2dff5-203">New-AzureRmStorageAccount에 -EnableHierarchicalNamespace 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-203">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="2dff5-204">파일 복사 cmdlet이 -DestContext 입력이 없을 때 대상의 원본 컨텍스트를 다시 사용할 수 없는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-204">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="2dff5-205">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="2dff5-205">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="2dff5-206">고정적인 웹 사이트 구성 지원</span><span class="sxs-lookup"><span data-stu-id="2dff5-206">Support Static Website configuration</span></span>
    - <span data-ttu-id="2dff5-207">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="2dff5-207">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="2dff5-208">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="2dff5-208">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="2dff5-209">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2dff5-209">Az.Websites</span></span>

* <span data-ttu-id="2dff5-210">Set-AzureRmWebApp 및 Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="2dff5-210">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="2dff5-211">Windows 및 Linux 컨테이너 응용 프로그램에 탑재할 Azure Storage 경로를 지정하기 위해 새 매개 변수(-AzureStoragePath)가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-211">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="2dff5-212">새 cmdlet New-AzureRmWebAppAzureStoragePath의 출력을 매개 변수로 사용하여 Azure Storage 경로를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-212">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="2dff5-213">0.6.1 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="2dff5-213">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="2dff5-214">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2dff5-214">Az.ApiManagement</span></span>
* <span data-ttu-id="2dff5-215">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="2dff5-215">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="2dff5-216">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2dff5-216">Az.Automation</span></span>
* <span data-ttu-id="2dff5-217">Azure Automation cmdlet 기반 Swagger</span><span class="sxs-lookup"><span data-stu-id="2dff5-217">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="2dff5-218">업데이트 관리 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-218">Added Update Management cmdlets</span></span>
* <span data-ttu-id="2dff5-219">소스 제어 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-219">Added Source Control cmdlets</span></span>
* <span data-ttu-id="2dff5-220">Remove-AzureRmAutomationHybridWorkerGroup cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-220">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="2dff5-221">DSC 노드 등록 명령 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-221">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="2dff5-222">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2dff5-222">Az.Compute</span></span>
* <span data-ttu-id="2dff5-223">SystemAssigned ID에 대한 ID 문제 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-223">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="2dff5-224">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="2dff5-224">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="2dff5-225">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="2dff5-225">Az.ContainerInstance</span></span>
* <span data-ttu-id="2dff5-226">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="2dff5-226">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="2dff5-227">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="2dff5-227">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="2dff5-228">마켓플레이스 cmdlet에 대한 예제 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="2dff5-228">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="2dff5-229">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2dff5-229">Az.Network</span></span>
* <span data-ttu-id="2dff5-230">New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-230">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="2dff5-231">지원되는 AzureFirewall 네트워크 프로토콜에 ICMP 다시 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-231">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="2dff5-232">Test-AzureRmNetworkWatcherConnectivity cmdlet을 업데이트하여 대상 ID, 주소 및 포트 유효성 검사를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-232">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="2dff5-233">VirtualNetwork 맵의 메모리 사용 문제 해결</span><span class="sxs-lookup"><span data-stu-id="2dff5-233">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="2dff5-234">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="2dff5-234">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="2dff5-235">보호된 파일 공유에 대한 정책을 수정하는 것에 대해 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-235">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="2dff5-236">정책 표준 시간대를 대문자로 변환했습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-236">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="2dff5-237">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="2dff5-237">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="2dff5-238">New-AzureRmRecoveryServicesAsrProtectableItem의 예제 정정</span><span class="sxs-lookup"><span data-stu-id="2dff5-238">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="2dff5-239">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="2dff5-239">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="2dff5-240">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="2dff5-240">Az.Relay</span></span>
* <span data-ttu-id="2dff5-241">선택적 매개 변수 -KeyValue를 New-AzureRmRelayKey cmdlet에 추가하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-241">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="2dff5-242">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2dff5-242">Az.Resources</span></span>
* <span data-ttu-id="2dff5-243">`New-AzureRmPolicyAssignment` 및 `Set-AzureRmPolicyAssignment`의 자원 ID 관련 매개 변수에 대한 도움말 문서를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="2dff5-243">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="2dff5-244">-Metadata를 사용하는 New-AzureRmPolicyDefinition에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-244">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="2dff5-245">NetStandard의 태그 키에서 대소문자 보존을 허용하도록 수정: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="2dff5-245">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="2dff5-246">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2dff5-246">Az.ServiceFabric</span></span>
* <span data-ttu-id="2dff5-247">향후 호환성이 손상되는 변경에 대한 사용 중단 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-247">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="2dff5-248">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2dff5-248">Az.Sql</span></span>
* <span data-ttu-id="2dff5-249">Azure Sql Database Managed Instance 및 Azure Sql 관리 데이터베이스에 CRUD 작업을 위한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-249">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="2dff5-250">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="2dff5-250">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="2dff5-251">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="2dff5-251">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="2dff5-252">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="2dff5-252">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="2dff5-253">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="2dff5-253">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="2dff5-254">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="2dff5-254">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="2dff5-255">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="2dff5-255">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="2dff5-256">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="2dff5-256">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="2dff5-257">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="2dff5-257">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="2dff5-258">서버 또는 데이터베이스에서 확장 감사 정책 관리를 활성화했습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-258">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="2dff5-259">새 매개 변수(PredicateExpression)가 감사 로그 필터링을 사용하도록 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-259">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="2dff5-260">Cmdlet이 레거시 클라이언트 대신 SQL 클라이언트를 사용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-260">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="2dff5-261">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="2dff5-261">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="2dff5-262">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="2dff5-262">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="2dff5-263">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="2dff5-263">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="2dff5-264">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="2dff5-264">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="2dff5-265">스토리지 계정 이름 매개 변수가 설정된 Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings를 사용할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="2dff5-265">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="2dff5-266">0.5.0 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="2dff5-266">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="2dff5-267">일반</span><span class="sxs-lookup"><span data-stu-id="2dff5-267">General</span></span>
* <span data-ttu-id="2dff5-268">많은 핵심 cmdlet에 Resource Completers를 추가하여 대화형으로 cmdlet을 호출할 때 기존 리소스 이름을 탭으로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-268">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="2dff5-269">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="2dff5-269">Az.Profile</span></span>
* <span data-ttu-id="2dff5-270">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-270">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="2dff5-271">Connect-AzAccount cmdlet의 매개 변수 TenantId 이름을 Tenant로 바꾸고 TenantId의 별칭을 추가합니다</span><span class="sxs-lookup"><span data-stu-id="2dff5-271">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="2dff5-272">Connect-AzAccount의 업데이트된 TenantId 설명</span><span class="sxs-lookup"><span data-stu-id="2dff5-272">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="2dff5-273">테넌트 도메인을 제공할 때 실패한 로그인에 대한 오류 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-273">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="2dff5-274">테넌트에 구독이 없는 계정의 컨텍스트 이름 충돌 문제 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-274">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="2dff5-275">MSI를 사용할 때 DataLake 엔드포인트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-275">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="2dff5-276">연결되지 않은 경우 'Disconnect-AzAccount'가 throw하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-276">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="2dff5-277">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2dff5-277">Az.CognitiveServices</span></span>
* <span data-ttu-id="2dff5-278">Get-AzCognitiveServicesAccountSkus 작업을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-278">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2dff5-279">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2dff5-279">Az.Compute</span></span>
* <span data-ttu-id="2dff5-280">Add-AzVmssVMDataDisk 및 Remove-AzVmssVMDataDisk cmdlet를 추가합니다</span><span class="sxs-lookup"><span data-stu-id="2dff5-280">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="2dff5-281">Get-AzVMImage는 AutomaticOSUpgradeProperties를 표시합니다</span><span class="sxs-lookup"><span data-stu-id="2dff5-281">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="2dff5-282">수정된 SetAzVMChefExtension -BootstrapOptions 및 -JsonAttribute option 값이 json 형식으로 설정하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-282">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2dff5-283">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2dff5-283">Az.DataLakeStore</span></span>
* <span data-ttu-id="2dff5-284">DataLake 패키지를 1.1.10으로 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-284">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="2dff5-285">기본 동시성을 다중 스레드 작업에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-285">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="2dff5-286">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="2dff5-286">Az.Insights</span></span>
* <span data-ttu-id="2dff5-287">해결된 문제 #7267(자동 크기 조정 영역)</span><span class="sxs-lookup"><span data-stu-id="2dff5-287">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="2dff5-288">열거된 매개 변수를 제대로 설정하지 않은 새 자동 크기 조정 규칙을 만드는 데 문제가 있습니다(이를 항상 기본값으로 설정함).</span><span class="sxs-lookup"><span data-stu-id="2dff5-288">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="2dff5-289">해결된 문제 # 7513[자세한 정보] Set-AzDiagnosticSetting은 설정을 생성하는 동안 범주를 명시적으로 지정해야 합니다</span><span class="sxs-lookup"><span data-stu-id="2dff5-289">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="2dff5-290">이제 cmdlet은 생성 중에 사용할 범주를 명시적으로 표시할 필요가 없습니다. 즉, 문서화된대로 작동합니다</span><span class="sxs-lookup"><span data-stu-id="2dff5-290">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2dff5-291">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2dff5-291">Az.Network</span></span>
* <span data-ttu-id="2dff5-292">다음 cmdlet에 대해 PeeringType을 필수 매개 변수로 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-292">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="2dff5-293">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="2dff5-293">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="2dff5-294">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="2dff5-294">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="2dff5-295">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="2dff5-295">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="2dff5-296">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="2dff5-296">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="2dff5-297">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="2dff5-297">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="2dff5-298">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="2dff5-298">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="2dff5-299">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2dff5-299">Az.PolicyInsights</span></span>
* <span data-ttu-id="2dff5-300">추가된 정책 재구성 cmdlet</span><span class="sxs-lookup"><span data-stu-id="2dff5-300">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="2dff5-301">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2dff5-301">Az.Resources</span></span>
* <span data-ttu-id="2dff5-302">https://github.com/Azure/azure-powershell/issues/7402에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-302">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="2dff5-303">'Get-AzResource'에 대해 '-ResourceId' 매개 변수를 사용하여 리소스 나열 허용</span><span class="sxs-lookup"><span data-stu-id="2dff5-303">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="2dff5-304">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2dff5-304">Az.ServiceBus</span></span>
* <span data-ttu-id="2dff5-305">마이그레이션 상태를 알 수 있도록 PSServiceBusMigrationConfigurationAttributes에 MigrationState 읽기 전용 속성 추가.</span><span class="sxs-lookup"><span data-stu-id="2dff5-305">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="2dff5-306">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2dff5-306">Az.ServiceFabric</span></span>
* <span data-ttu-id="2dff5-307">Linux Vmss에 인증서 추가 수정.</span><span class="sxs-lookup"><span data-stu-id="2dff5-307">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="2dff5-308">Add-AzServiceFabricClusterCertificate 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-308">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="2dff5-309">새 인증서(Azure/service-fabric-issues#932)에서 올바른 지문을 사용.</span><span class="sxs-lookup"><span data-stu-id="2dff5-309">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="2dff5-310">올바르게 예외 표시(Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="2dff5-310">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="2dff5-311">Vmss CreateOrUpdate 작업을 시작하기 전에 'Update-AzServiceFabricDurability'를 수정하여 클러스터 구성 업데이트.</span><span class="sxs-lookup"><span data-stu-id="2dff5-311">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="2dff5-312">0.4.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="2dff5-312">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="2dff5-313">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="2dff5-313">Az.Profile</span></span>
* <span data-ttu-id="2dff5-314">CloudShell에서 Get-AzSubscription을 사용하여 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-314">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="2dff5-315">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-315">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2dff5-316">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2dff5-316">Az.Compute</span></span>
* <span data-ttu-id="2dff5-317">'New-AzVm'에 대해 간단한 매개 변수를 사용하는 경우 가속화된 네트워킹을 설정하기 위해 새 크기가 VM 크기의 허용 목록에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-317">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="2dff5-318">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-318">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2dff5-319">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2dff5-319">Az.DataLakeStore</span></span>
* <span data-ttu-id="2dff5-320">Virtual Network 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-320">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="2dff5-321">Get-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 가져오거나 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-321">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="2dff5-322">Add-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 가상 네트워크 규칙을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-322">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="2dff5-323">Set-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 지정된 가상 네트워크 규칙을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-323">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="2dff5-324">Remove-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-324">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2dff5-325">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2dff5-325">Az.Network</span></span>
* <span data-ttu-id="2dff5-326">Test-AzNetworkWatcherConnectivity cmdlet을 업데이트하고, 백 엔드에 프로토콜 값을 전달합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-326">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="2dff5-327">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-327">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="2dff5-328">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2dff5-328">Az.Resources</span></span>
* <span data-ttu-id="2dff5-329">(기본 프로필에 구독이 없고 범위가 지정되지 않은 경우) 시나리오에서 의미 있는 예외를 추가하여 Get-AzRoleDefinition이 인식할 수 없는 예외를 throw하는 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-329">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="2dff5-330">또한 기본 매개 변수 집합을 'RoleDefinitionNameParameterSet'으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-330">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="2dff5-331">0.3.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="2dff5-331">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="2dff5-332">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="2dff5-332">Azure.Storage</span></span>
* <span data-ttu-id="2dff5-333">대상에 메타데이터가 있을 때 Blob/파일이 메타 데이터를 복사하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-333">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="2dff5-334">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="2dff5-334">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="2dff5-335">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="2dff5-335">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="2dff5-336">특정 위치의 저장소 리소스 사용을 지원하고 글로벌 저장소 리소스 사용 가져오기는 더 이상 사용되지 않는다는 경고 메시지를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-336">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="2dff5-337">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="2dff5-337">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="2dff5-338">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2dff5-338">Az.CognitiveServices</span></span>
* <span data-ttu-id="2dff5-339">기존 계정이 없는 Get-AzCognitiveServicesAccountSkus를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-339">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2dff5-340">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2dff5-340">Az.Compute</span></span>
* <span data-ttu-id="2dff5-341">Get-AzVM -ResourceGroupName <rg>가 필요한 경우 50개가 넘는 결과를 반환하도록 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-341">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="2dff5-342">'SimpleParameterSet' 예제가 New-AzVmss cmdlet 도움말에 추가됨</span><span class="sxs-lookup"><span data-stu-id="2dff5-342">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="2dff5-343">Azure Disk Encryption 진행률 메시지의 오타를 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-343">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="2dff5-344">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="2dff5-344">Az.DataFactoryV2</span></span>
* <span data-ttu-id="2dff5-345">ADF.Net SDK 버전을 2.3.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="2dff5-345">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2dff5-346">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2dff5-346">Az.Network</span></span>
* <span data-ttu-id="2dff5-347">NetworkProfile 기능 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-347">Added NetworkProfile functionality.</span></span> <span data-ttu-id="2dff5-348">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-348">new cmdlets added</span></span>
    - <span data-ttu-id="2dff5-349">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2dff5-349">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="2dff5-350">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2dff5-350">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="2dff5-351">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2dff5-351">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="2dff5-352">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2dff5-352">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="2dff5-353">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="2dff5-353">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="2dff5-354">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="2dff5-354">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="2dff5-355">서브넷 모델에 서비스 연결 링크 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-355">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="2dff5-356">New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-356">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="2dff5-357">Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-357">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="2dff5-358">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="2dff5-358">Az.RedisCache</span></span>
* <span data-ttu-id="2dff5-359">모든 문자열을 Size 매개 변수로 진행되도록 허용</span><span class="sxs-lookup"><span data-stu-id="2dff5-359">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="2dff5-360">PSArgumentCompleter 팝업에 P5 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-360">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="2dff5-361">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2dff5-361">Az.Resources</span></span>
* <span data-ttu-id="2dff5-362">-Mode 매개 변수를 Set-AzPolicyDefinition에 추가</span><span class="sxs-lookup"><span data-stu-id="2dff5-362">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="2dff5-363">사용자가 포함된 Origin 작업에서 Get-AzProviderOperation commandlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="2dff5-363">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="2dff5-364">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2dff5-364">Az.Sql</span></span>
* <span data-ttu-id="2dff5-365">일부 백업 cmdlet이 현재 azure 구독을 인식하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="2dff5-365">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2dff5-366">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2dff5-366">Az.Websites</span></span>
* <span data-ttu-id="2dff5-367">새 cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - 컨테이너 지속적인 배포 Webhook URL을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-367">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="2dff5-368">새 cmdlet New-AzWebAppContainerPSSession 및 Enter-WebAppContainerPSSession -  windows 컨테이너 앱에 PowerShell 원격 세션을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="2dff5-368">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="2dff5-369">0.2.0 - 2018년 9월</span><span class="sxs-lookup"><span data-stu-id="2dff5-369">0.2.0 - September 2018</span></span>
 <span data-ttu-id="2dff5-370">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="2dff5-370">Initial Release</span></span>