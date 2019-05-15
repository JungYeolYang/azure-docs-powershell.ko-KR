---
ms.openlocfilehash: 3848f7fb8e298d137c747405f32a0776c1a8f029
ms.sourcegitcommit: accff0c2cd6035fcda2d917f6051a5b509eb6255
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 05/06/2019
ms.locfileid: "65048634"
---
## <a name="200---may-2019"></a><span data-ttu-id="c5154-101">2.0.0 - 2019년 5월</span><span class="sxs-lookup"><span data-stu-id="c5154-101">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c5154-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c5154-102">Az.Accounts</span></span>
* <span data-ttu-id="c5154-103">사용자 이름/비밀번호 인증을 사용하여 ADFS 문제를 해결하도록 인증 라이브러리 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-103">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c5154-104">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c5154-104">Az.CognitiveServices</span></span>
* <span data-ttu-id="c5154-105">Bing Search 서비스에 대해서만 Bing 면책 조항을 표시하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-105">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="c5154-106">계정 생성 실패 시 오류 개선.</span><span class="sxs-lookup"><span data-stu-id="c5154-106">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-107">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-107">Az.Compute</span></span>
* <span data-ttu-id="c5154-108">근접 배치 그룹 기능</span><span class="sxs-lookup"><span data-stu-id="c5154-108">Proximity placement group feature.</span></span>
    - <span data-ttu-id="c5154-109">다음과 같은 새 cmdlet을 추가했습니다.   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="c5154-109">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="c5154-110">새 매개 변수 ProximityPlacementGroupId가 다음 cmdlet에 추가됩니다.   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="c5154-110">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="c5154-111">New-AzGalleryImageVersion에 StorageAccountType 매개 변수가 추가됩니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-111">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="c5154-112">New-AzGalleryImageVersion의 TargetRegion이 StorageAccountType를 포함할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-112">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="c5154-113">SkipShutdown 스위치 매개 변수가 Stop-AzVM 및 Stop-AzVmss에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-113">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="c5154-114">주요 변경 내용</span><span class="sxs-lookup"><span data-stu-id="c5154-114">Breaking changes</span></span>
    - <span data-ttu-id="c5154-115">Set-AzVMBootDiagnostics이 Set-AzVMBootDiagnostic으로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-115">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="c5154-116">Export-AzLogAnalyticThrottledRequests이 Export-AzLogAnalyticThrottledRequests로 변경되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-116">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="c5154-117">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="c5154-117">Az.DeploymentManager</span></span>
* <span data-ttu-id="c5154-118">Azure 배포 관리자 cmdlet의 일반적으로 사용 가능한 첫 번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="c5154-118">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="c5154-119">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="c5154-119">Az.Dns</span></span>
* <span data-ttu-id="c5154-120">자동 DNS 이름 서버 위임</span><span class="sxs-lookup"><span data-stu-id="c5154-120">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="c5154-121">DNS 영역 만들기 cmdlet은 추가 선택적 매개 변수로 부모 영역 이름을 허용합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-121">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="c5154-122">새로 생성 된 자식 영역의 부모 영역에 NS 레코드를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-122">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="c5154-123">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c5154-123">Az.FrontDoor</span></span>
* <span data-ttu-id="c5154-124">Azure FrontDoor cmdlet의 일반적으로 사용 가능한 첫 번째 릴리스</span><span class="sxs-lookup"><span data-stu-id="c5154-124">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="c5154-125">'Waf'를 포함하도록 WAF cmdlet의 이름 바꾸기</span><span class="sxs-lookup"><span data-stu-id="c5154-125">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="c5154-126">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c5154-126">Az.HDInsight</span></span>
* <span data-ttu-id="c5154-127">두 개의 cmdlet을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-127">Removed two cmdlets:</span></span>
    - <span data-ttu-id="c5154-128">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c5154-128">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="c5154-129">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="c5154-129">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="c5154-130">Grant-AzHDInsightHttpServicesAccess를 대체할 새 cmdlet Set-AzHDInsightGatewayCredential을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-130">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="c5154-131">reader 역할과 HDInsight 운영자 역할을 구분하도록 cmdlet Get-AzHDInsightJobOutput 업데이트:</span><span class="sxs-lookup"><span data-stu-id="c5154-131">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="c5154-132">reader 역할을 가진 사용자는 'DefaultStorageAccountKey'매개 변수를 명시적으로 지정해야 합니다. 그렇지 않으면 오류가 발생합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-132">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="c5154-133">Hdinsight 운영자 역할을 가진 사용자를 영향을 받지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-133">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c5154-134">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c5154-134">Az.Monitor</span></span>
* <span data-ttu-id="c5154-135">SQR API(예약 쿼리 규칙)용 새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="c5154-135">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="c5154-136">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="c5154-136">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="c5154-137">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="c5154-137">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="c5154-138">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="c5154-138">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="c5154-139">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="c5154-139">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="c5154-140">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="c5154-140">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="c5154-141">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="c5154-141">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="c5154-142">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c5154-142">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c5154-143">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c5154-143">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c5154-144">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c5154-144">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c5154-145">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c5154-145">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c5154-146">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="c5154-146">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="c5154-147">SQR API에 대한 [자세한 내용](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules)</span><span class="sxs-lookup"><span data-stu-id="c5154-147">[More](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="c5154-148">GenV2(비 클래식) 메트릭 기반 경고 규칙에 대한 cmdlet을 포함하도록 Az.Monitor.md가 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="c5154-148">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c5154-149">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-149">Az.Network</span></span>
* <span data-ttu-id="c5154-150">Nat 게이트웨이 리소스에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-150">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="c5154-151">새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="c5154-151">New cmdlets</span></span>
        - <span data-ttu-id="c5154-152">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c5154-152">New-AzNatGateway</span></span>
        - <span data-ttu-id="c5154-153">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c5154-153">Get-AzNatGateway</span></span>
        - <span data-ttu-id="c5154-154">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c5154-154">Set-AzNatGateway</span></span>
        - <span data-ttu-id="c5154-155">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="c5154-155">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="c5154-156">다음 Cmdlet이 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-156">Updated cmdlets</span></span>
        - <span data-ttu-id="c5154-157">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="c5154-157">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="c5154-158">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="c5154-158">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="c5154-159">기능에 대한 새로운 명령이 업데이트됨: Brooklyn Gateway에서 사용자 지정 경로 설정/제거.</span><span class="sxs-lookup"><span data-stu-id="c5154-159">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="c5154-160">New-AzVirtualNetworkGateway가 업데이트됨: 선택적 매개 변수 -CustomRoute를 추가하여 게이트웨이에서 설정할 사용자 지정 경로로 주소 접두사를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-160">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="c5154-161">Set-AzVirtualNetworkGateway가 업데이트됨: 선택적 매개 변수 -CustomRoute를 추가하여 게이트웨이에서 설정할 사용자 지정 경로로 주소 접두사를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-161">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c5154-162">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c5154-162">Az.PolicyInsights</span></span>
* <span data-ttu-id="c5154-163">정책 평가 세부 정보 쿼리 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-163">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="c5154-164">Get-AzPolicyState에 '-Expand'매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-164">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="c5154-165">'-Expand PolicyEvaluationDetails' 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-165">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c5154-166">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c5154-166">Az.RecoveryServices</span></span>
* <span data-ttu-id="c5154-167">크로스 구독 Azure에서 Azure 사이트 복구 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-167">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="c5154-168">Azure Site Recovery에 대한 호환성이 손상되는 변경 표시</span><span class="sxs-lookup"><span data-stu-id="c5154-168">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="c5154-169">Azure Site Recovery 복구 계획 최종 실행 계획에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-169">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="c5154-170">Azure에서 Azure에 대한 Azure Site Recovery 업데이트 네트워크 매핑 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-170">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="c5154-171">관리 디스크에 대한 Azure에서 Azure에 대한 Azure Site Recovery 업데이트 보호 방향 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-171">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="c5154-172">기타 사소한 수정.</span><span class="sxs-lookup"><span data-stu-id="c5154-172">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="c5154-173">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="c5154-173">Az.Relay</span></span>
* <span data-ttu-id="c5154-174">고객 관련 메시지의 철자 오류 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-174">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c5154-175">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c5154-175">Az.ServiceBus</span></span>
* <span data-ttu-id="c5154-176">네임스페이스의 NetworkRuleSet에 대한 새 cmdlet가 추가되었습니다</span><span class="sxs-lookup"><span data-stu-id="c5154-176">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c5154-177">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c5154-177">Az.Storage</span></span>
* <span data-ttu-id="c5154-178">저장소 클라이언트 라이브러리 10.0.1로 업그레이드(이 SDK의 모든 개체의 네임스페이스가 'Microsoft.WindowsAzure.Storage.*'에서 'Microsoft.Azure.Storage.*'로 변경됨)</span><span class="sxs-lookup"><span data-stu-id="c5154-178">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="c5154-179">새로운 API 버전 2019-04-01을 지원하기 위해 Microsoft.Azure.Management.Storage 11.0.0으로 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-179">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="c5154-180">스토리지 생성 계정의 기본 스토리지 계정 종류가 'Storage'에서 'StorageV2'로 변경됩니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-180">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="c5154-181">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c5154-181">New-AzStorageAccount</span></span>
* <span data-ttu-id="c5154-182">'StandardLRS'가 'Standard_LRS'로 변경되는 것과 같이 '-'을 추가하여 입력 SkuName과 정렬되도록 스토리지 계정 cmdlet 출력 Sku.Name을 변경합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-182">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="c5154-183">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c5154-183">New-AzStorageAccount</span></span>
    - <span data-ttu-id="c5154-184">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c5154-184">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="c5154-185">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="c5154-185">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c5154-186">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c5154-186">Az.Websites</span></span>
* <span data-ttu-id="c5154-187">Get-AzWebApp에서 반환한 PSSite 개체에 대해 'Kind'속성이 설정됩니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-187">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="c5154-188">Get-AzWebApp\* 메트릭 및 Get-AzAppServicePlanMetrics가 사용되지 않음으로 표시되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-188">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="c5154-189">1.8.0 - 2019년 4월</span><span class="sxs-lookup"><span data-stu-id="c5154-189">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c5154-190">마지막 주 릴리스 이후의 주요 사항</span><span class="sxs-lookup"><span data-stu-id="c5154-190">Highlights since the last major release</span></span>
* <span data-ttu-id="c5154-191">`Az` 모듈 일반 공급</span><span class="sxs-lookup"><span data-stu-id="c5154-191">General availability of `Az` module</span></span>
* <span data-ttu-id="c5154-192">`Az` 모듈에 대한 자세한 내용은 https://aka.ms/azps-announce를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-192">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c5154-193">Location, ResourceGroup 및 ResourceName 완성자가 추가되었습니다(https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/).</span><span class="sxs-lookup"><span data-stu-id="c5154-193">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c5154-194">와일드카드 지원이 Az.Compute 및 Az.Network에 대한 Get cmdlet에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-194">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c5154-195">Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-195">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c5154-196">Python 2 Runbook 지원이 Az.Automation에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-196">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c5154-197">Az.LogicApp: 통합 계정 어셈블리 및 일괄 처리 구성을 위한 새로운 cmdlet입니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-197">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c5154-198">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c5154-198">Az.Accounts</span></span>
* <span data-ttu-id="c5154-199">Mac에서 모듈을 올바르게 삭제하기 위해 Uninstall-AzureRm을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-199">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="c5154-200">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c5154-200">Az.Batch</span></span>
* <span data-ttu-id="c5154-201">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-201">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c5154-202">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c5154-202">Az.Cdn</span></span>
* <span data-ttu-id="c5154-203">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-203">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c5154-204">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c5154-204">Az.CognitiveServices</span></span>
* <span data-ttu-id="c5154-205">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-205">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-206">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-206">Az.Compute</span></span>
* <span data-ttu-id="c5154-207">디스크의 리소스 ID에 리소스 ID의 소문자 resourcegroups가 있는 경우 AEM 설치 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-207">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="c5154-208">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-208">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c5154-209">와일드 카드에 대한 설명서 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-209">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c5154-210">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c5154-210">Az.DataFactory</span></span>
* <span data-ttu-id="c5154-211">NodeCount가 관리형 통합 런타임에 대해 Null이 아닌 경우 SsisProperties를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-211">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c5154-212">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c5154-212">Az.DataLakeStore</span></span>
* <span data-ttu-id="c5154-213">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-213">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c5154-214">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c5154-214">Az.EventGrid</span></span>
* <span data-ttu-id="c5154-215">이벤트 구독 cmdlet 만들기/업데이트를 사용하기 전에 리소스를 만들어야 함을 나타내기 위해 엔드포인트의 도움말 텍스트가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-215">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c5154-216">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c5154-216">Az.EventHub</span></span>
* <span data-ttu-id="c5154-217">네임스페이스의 NetworkRuleSet에 대한 새 cmdlet가 추가되었습니다</span><span class="sxs-lookup"><span data-stu-id="c5154-217">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="c5154-218">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="c5154-218">Az.HDInsight</span></span>
* <span data-ttu-id="c5154-219">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-219">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c5154-220">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c5154-220">Az.IotHub</span></span>
* <span data-ttu-id="c5154-221">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-221">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c5154-222">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5154-222">Az.KeyVault</span></span>
* <span data-ttu-id="c5154-223">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-223">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c5154-224">와일드 카드에 대한 설명서 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-224">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="c5154-225">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c5154-225">Az.MachineLearning</span></span>
* <span data-ttu-id="c5154-226">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-226">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="c5154-227">Az.Media</span><span class="sxs-lookup"><span data-stu-id="c5154-227">Az.Media</span></span>
* <span data-ttu-id="c5154-228">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-228">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c5154-229">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c5154-229">Az.Monitor</span></span>
  * <span data-ttu-id="c5154-230">GenV2(비 클래식) 메트릭 기반 경고 규칙에 대한 새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="c5154-230">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="c5154-231">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="c5154-231">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="c5154-232">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="c5154-232">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="c5154-233">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c5154-233">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="c5154-234">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c5154-234">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="c5154-235">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="c5154-235">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="c5154-236">모니터 SDK가 버전 0.22.0-preview로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-236">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c5154-237">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-237">Az.Network</span></span>
* <span data-ttu-id="c5154-238">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-238">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c5154-239">와일드 카드에 대한 설명서 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-239">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="c5154-240">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="c5154-240">Az.NotificationHubs</span></span>
* <span data-ttu-id="c5154-241">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-241">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c5154-242">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c5154-242">Az.OperationalInsights</span></span>
* <span data-ttu-id="c5154-243">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-243">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="c5154-244">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="c5154-244">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="c5154-245">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-245">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c5154-246">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c5154-246">Az.RecoveryServices</span></span>
* <span data-ttu-id="c5154-247">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-247">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c5154-248">Azure VM의 SQL용 테이블 형식이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-248">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="c5154-249">AzureFileShare에서 위치를 가져오는 대체 메서드가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-249">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="c5154-250">시간대에 따라 SchedulePolicy 개체의 ScheduleRunDays가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-250">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c5154-251">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c5154-251">Az.RedisCache</span></span>
* <span data-ttu-id="c5154-252">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-252">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c5154-253">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-253">Az.Resources</span></span>
* <span data-ttu-id="c5154-254">와일드 카드에 대한 설명서 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-254">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="c5154-255">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-255">Az.Sql</span></span>
* <span data-ttu-id="c5154-256">Monitor SDK의 종속성을 공용 코드로 바꿉니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-256">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="c5154-257">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-257">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c5154-258">다중 열 분류 프로세스가 향상되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-258">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="c5154-259">기본적으로 Get-AzSqlServerServiceObjective의 응답으로 SKU 속성(SKU 이름, 제품군, 용량)과 테이블 형식을 포함합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-259">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="c5154-260">해당 지역에 기존 서버 없이 위치별로 Get-AzSqlServerServiceObjective를 가져올 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-260">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="c5154-261">관리형 인스턴스 생성 시 표준 시간대 매개 변수를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-261">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="c5154-262">와일드 카드에 대한 설명서 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-262">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c5154-263">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c5154-263">Az.Websites</span></span>
* <span data-ttu-id="c5154-264">실행 시 태그를 제거하지 않도록 Set-AzWebApp 및 Set-AzWebAppSlot를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-264">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="c5154-265">복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-265">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="c5154-266">WebSites SDK가 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-266">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="c5154-267">PSAppServicePlan에서 AdminSiteName 속성을 제거했습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-267">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="c5154-268">1.7.0 - 2019년 4월</span><span class="sxs-lookup"><span data-stu-id="c5154-268">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c5154-269">마지막 주 릴리스 이후의 주요 사항</span><span class="sxs-lookup"><span data-stu-id="c5154-269">Highlights since the last major release</span></span>
* <span data-ttu-id="c5154-270">`Az` 모듈 일반 공급</span><span class="sxs-lookup"><span data-stu-id="c5154-270">General availability of `Az` module</span></span>
* <span data-ttu-id="c5154-271">`Az` 모듈에 대한 자세한 내용은 https://aka.ms/azps-announce를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-271">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c5154-272">Location, ResourceGroup 및 ResourceName 완성자가 추가되었습니다(https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/).</span><span class="sxs-lookup"><span data-stu-id="c5154-272">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c5154-273">와일드카드 지원이 Az.Compute 및 Az.Network에 대한 Get cmdlet에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-273">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c5154-274">Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-274">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c5154-275">Python 2 Runbook 지원이 Az.Automation에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-275">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c5154-276">Az.LogicApp: 통합 계정 어셈블리 및 일괄 처리 구성을 위한 새로운 cmdlet입니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-276">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="c5154-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c5154-277">Az.Accounts</span></span>
* <span data-ttu-id="c5154-278">매개 변수 AzureAnalysisServicesEndpointResourceId를 허용하도록 Add-AzEnvironment 및 Set-AzEnvironment 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-278">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c5154-279">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c5154-279">Az.AnalysisServices</span></span>
* <span data-ttu-id="c5154-280">데이터 평면 cmdlet에서 ServiceClient 사용 및 원본 인증 논리 제거</span><span class="sxs-lookup"><span data-stu-id="c5154-280">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="c5154-281">호환성이 손상되는 변경을 방지하기 위해 Add-AzureASAccount를 Connect-AzAccount의 래퍼로 만듦</span><span class="sxs-lookup"><span data-stu-id="c5154-281">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c5154-282">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c5154-282">Az.Automation</span></span>
* <span data-ttu-id="c5154-283">포함에 대한 New-AzAutomationSoftwareUpdateConfiguration cmdlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-283">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="c5154-284">이제 매개 변수 IncludedKbNumber 및 IncludedPackageNameMask가 작동함</span><span class="sxs-lookup"><span data-stu-id="c5154-284">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="c5154-285">Azure 자동화 업데이트 관리 동적 그룹에 대한 버그 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-285">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-286">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-286">Az.Compute</span></span>
* <span data-ttu-id="c5154-287">New-AzDiskConfig 및 New-AzSnapshotConfig에 HyperVGeneration 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-287">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="c5154-288">다른 테넌트의 갤러리 이미지를 사용하여 VM을 만들 수 있음</span><span class="sxs-lookup"><span data-stu-id="c5154-288">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="c5154-289">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c5154-289">Az.ContainerInstance</span></span>
* <span data-ttu-id="c5154-290">후행 빈 인수를 추가한 New-AzContainerGroup의 -Command 매개 변수의 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-290">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c5154-291">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c5154-291">Az.DataFactory</span></span>
* <span data-ttu-id="c5154-292">ADF .Net SDK 버전을 3.0.2로 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-292">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="c5154-293">RepoConfiguration 관련 설정에 대한 추가 매개 변수로 Set-AzDataFactoryV2 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-293">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c5154-294">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-294">Az.Resources</span></span>
* <span data-ttu-id="c5154-295">'-ResourceId' 또는 '-ResourceGroupName', '-Name' 및 '-ResourceType' 매개 변수를 제공할 때 'Get-AzResource'에 대한 공급자 처리 개선</span><span class="sxs-lookup"><span data-stu-id="c5154-295">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="c5154-296">'Test-AzDeployment' 및 'Test-AzResourceGroupDeployment'에 대한 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="c5154-296">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="c5154-297">배포 유효성 검사 외부에서 발생한 오류를 처리하고 그 대신 명령의 출력에 포함</span><span class="sxs-lookup"><span data-stu-id="c5154-297">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="c5154-298">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/6856를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-298">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="c5154-299">배포 cmdlet 세트에 스크립트 및 작업 시나리오에서 프롬프트를 건너뛰는 '-IgnoreDynamicParameters' 스위치 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-299">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="c5154-300">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/6856를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-300">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="c5154-301">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-301">Az.Sql</span></span>
* <span data-ttu-id="c5154-302">데이터베이스 데이터 분류 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-302">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c5154-303">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c5154-303">Az.Storage</span></span>
* <span data-ttu-id="c5154-304">매개 변수 -UseConnectedAccount를 사용하여 스토리지 컨텍스트를 만들 때 자세한 오류 보고(단, 로그인 Azure 계정 없이)</span><span class="sxs-lookup"><span data-stu-id="c5154-304">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="c5154-305">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="c5154-305">New-AzStorageContext</span></span>
* <span data-ttu-id="c5154-306">관리 평면 API를 사용하여 지정한 스토리지 계정의 BLOB 서비스 속성 관리 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-306">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="c5154-307">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="c5154-307">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="c5154-308">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="c5154-308">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="c5154-309">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c5154-309">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="c5154-310">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c5154-310">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="c5154-311">BLOB 및 파일 업로드/다운로드 cmdlet에 대한 -AsJob 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-311">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="c5154-312">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c5154-312">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="c5154-313">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="c5154-313">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="c5154-314">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c5154-314">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="c5154-315">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="c5154-315">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="c5154-316">1.6.0 - 2019년 3월</span><span class="sxs-lookup"><span data-stu-id="c5154-316">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="c5154-317">마지막 주 릴리스 이후의 주요 사항</span><span class="sxs-lookup"><span data-stu-id="c5154-317">Highlights since the last major release</span></span>
* <span data-ttu-id="c5154-318">`Az` 모듈 일반 공급</span><span class="sxs-lookup"><span data-stu-id="c5154-318">General availability of `Az` module</span></span>
* <span data-ttu-id="c5154-319">`Az` 모듈에 대한 자세한 내용은 https://aka.ms/azps-announce를 방문하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-319">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="c5154-320">Location, ResourceGroup 및 ResourceName 완성자가 추가되었습니다(https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/).</span><span class="sxs-lookup"><span data-stu-id="c5154-320">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="c5154-321">와일드카드 지원이 Az.Compute 및 Az.Network에 대한 Get cmdlet에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-321">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="c5154-322">Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-322">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c5154-323">Python 2 Runbook 지원이 Az.Automation에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-323">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="c5154-324">Az.LogicApp: 통합 계정 어셈블리 및 일괄 처리 구성을 위한 새로운 cmdlet입니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-324">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c5154-325">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c5154-325">Az.Automation</span></span>
* <span data-ttu-id="c5154-326">Azure 자동화 업데이트 관리에서 변경된 지원 기능은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-326">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="c5154-327">동적 그룹화</span><span class="sxs-lookup"><span data-stu-id="c5154-327">Dynamic grouping</span></span>
    * <span data-ttu-id="c5154-328">사전 스크립트</span><span class="sxs-lookup"><span data-stu-id="c5154-328">Pre-Post script</span></span>
    * <span data-ttu-id="c5154-329">다시 부팅 설정</span><span class="sxs-lookup"><span data-stu-id="c5154-329">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-330">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-330">Az.Compute</span></span>
* <span data-ttu-id="c5154-331">Get-AzVmBootDiagnosticsData의 경로 확인 문제가 해결되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-331">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="c5154-332">Compute 클라이언트 라이브러리가 25.0.0으로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-332">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c5154-333">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5154-333">Az.KeyVault</span></span>
* <span data-ttu-id="c5154-334">와일드카드 지원이 KeyVault cmdlet에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-334">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c5154-335">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-335">Az.Network</span></span>
* <span data-ttu-id="c5154-336">Azure Firewall에 대한 위협 인텔리전스 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-336">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="c5154-337">Application Gateway 방화벽 정책의 최상위 수준 리소스 및 사용자 지정 규칙이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-337">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c5154-338">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c5154-338">Az.RecoveryServices</span></span>
* <span data-ttu-id="c5154-339">인스턴트 RP를 지원하기 위해 SnapshotRetentionInDays가 Azure VM 정책에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-339">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="c5154-340">컨테이너 등록을 취소하는 파이프 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-340">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="c5154-341">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-341">Az.Resources</span></span>
* <span data-ttu-id="c5154-342">Get-AzResource 및 Get-AzResourceGroup에 대한 와일드카드 지원을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-342">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="c5154-343">ARM에 대한 일반 호출을 수행할 때 사용되는 자격 증명을 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-343">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="c5154-344">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-344">Az.Sql</span></span>
* <span data-ttu-id="c5154-345">위협 탐지의 cmdlet 매개 변수(ExcludeDetectionType)가 DetectionType에서 string[]으로 변경되어 새 DetectionType이 추가되면 이후의 증명이 되고 자동 완성도 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-345">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c5154-346">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c5154-346">Az.Storage</span></span>
* <span data-ttu-id="c5154-347">스토리지 계정에 대한 관리 정책 가져오기/설정/제거를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-347">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="c5154-348">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c5154-348">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c5154-349">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c5154-349">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c5154-350">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="c5154-350">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="c5154-351">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="c5154-351">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="c5154-352">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="c5154-352">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="c5154-353">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="c5154-353">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c5154-354">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c5154-354">Az.Websites</span></span>
* <span data-ttu-id="c5154-355">'New-AzWebApp -IncludeSourceWebAppSlots'를 사용하여 모든 슬롯의 복제를 중단하는 ARM 템플릿 버그가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-355">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="c5154-356">1.5.0 - 2019년 3월</span><span class="sxs-lookup"><span data-stu-id="c5154-356">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c5154-357">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c5154-357">Az.Accounts</span></span>
* <span data-ttu-id="c5154-358">'Register-AzModule' 명령을 추가하여 AutoRest 생성 cmdlet을 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-358">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="c5154-359">Connect-AzAccount 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-359">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c5154-360">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c5154-360">Az.Automation</span></span>
* <span data-ttu-id="c5154-361">몇몇 Azure Automation cmdlet에서 특정 월별 일정을 검색할 때 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-361">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="c5154-362">상위 20개 노드를 반환하도록 Get-AzAutomationDscNode를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-362">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="c5154-363">이제 모든 노드 반환</span><span class="sxs-lookup"><span data-stu-id="c5154-363">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c5154-364">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c5154-364">Az.Cdn</span></span>
* <span data-ttu-id="c5154-365">사용자 지정 도메인 Https 사용/사용 안 함에 대한 새 Powershell cmdlet이 추가되었으며 기존의 것은 사용되지 않았습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-365">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-366">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-366">Az.Compute</span></span>
* <span data-ttu-id="c5154-367">Get cmdlet에 와일드 카드 지원 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-367">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c5154-368">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c5154-368">Az.DataFactory</span></span>
* <span data-ttu-id="c5154-369">ADF.Net SDK 버전이 3.0.1로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-369">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c5154-370">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c5154-370">Az.LogicApp</span></span>
* <span data-ttu-id="c5154-371">첫 결과 페이지 검색 시에만 ListWorkflows 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-371">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c5154-372">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-372">Az.Network</span></span>
* <span data-ttu-id="c5154-373">Network cmdlet에 와일드 카드 지원 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-373">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c5154-374">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c5154-374">Az.RecoveryServices</span></span>
* <span data-ttu-id="c5154-375">Azure VM 지원에 SQL 서버가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-375">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="c5154-376">SDK 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-376">SDK Update</span></span>
* <span data-ttu-id="c5154-377">VMappContainer 체크 인 Get-ProtectableItem 제거</span><span class="sxs-lookup"><span data-stu-id="c5154-377">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="c5154-378">Get ProtectableItem의 매개 변수로 Name과 ServerName이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-378">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="c5154-379">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-379">Az.Resources</span></span>
* <span data-ttu-id="c5154-380">`-TemplateObject` 매개 변수를 추가하여 cmdlet을 배포</span><span class="sxs-lookup"><span data-stu-id="c5154-380">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="c5154-381">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/2933를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-381">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="c5154-382">`Get-AzResource`의 결과를 `Set-AzResource`(으)로 파이프할 때 발생하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-382">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="c5154-383">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8240를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-383">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="c5154-384">실행 시 JSON 데이터 형식 문제 해결 `Set-AzResource`</span><span class="sxs-lookup"><span data-stu-id="c5154-384">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="c5154-385">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7930를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-385">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="c5154-386">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-386">Az.Sql</span></span>
* <span data-ttu-id="c5154-387">AuditingEndpointsCommunicator를 업데이트 합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-387">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="c5154-388">새 진단 설정을 생성할 때 에지 사례의 동작을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-388">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c5154-389">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c5154-389">Az.Storage</span></span>
* <span data-ttu-id="c5154-390">스토리지 계정      - New-AzStorageAccount를 생성할 때 종류 BlockBlobStorage를 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-390">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="c5154-391">1.4.0 - 2019년 2월</span><span class="sxs-lookup"><span data-stu-id="c5154-391">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="c5154-392">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c5154-392">Az.AnalysisServices</span></span>
* <span data-ttu-id="c5154-393">사용되지 않는 AddAzureASAccount cmdlet</span><span class="sxs-lookup"><span data-stu-id="c5154-393">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c5154-394">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c5154-394">Az.Automation</span></span>
* <span data-ttu-id="c5154-395">Import-AzAutomationDscNodeConfiguration 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-395">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="c5154-396">Import-AzAutomationDscConfiguration cmdlet 구성 이름 유효성 검사 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-396">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="c5154-397">Import-AzAutomationDscConfiguration cmdlet 오류 처리 개선</span><span class="sxs-lookup"><span data-stu-id="c5154-397">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="c5154-398">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c5154-398">Az.CognitiveServices</span></span>
* <span data-ttu-id="c5154-399">리소스의 하위 도메인을 지정하는 데 사용되는 New-AzCognitiveServicesAccount에 대한 새 선택적 매개 변수로 CustomSubdomainName이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-399">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-400">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-400">Az.Compute</span></span>
* <span data-ttu-id="c5154-401">ID 매개 변수 집합 문제 해결</span><span class="sxs-lookup"><span data-stu-id="c5154-401">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="c5154-402">Name 매개 변수를 제공하지 않으면 Get-AzVMExtension이 설치된 모든 확장을 열거하도록 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-402">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="c5154-403">Update-AzImage cmdlet에 태그 및 ResourceId 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-403">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="c5154-404">인스턴스 ID가 없는 Get-AzVmssVM과 InstanceView를 사용하면 인스턴스 보기가 있는 VMSS VM을 나열할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-404">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c5154-405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c5154-405">Az.DataLakeStore</span></span>
* <span data-ttu-id="c5154-406">ADL 삭제된 항목 열거 및 복원에 대한 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-406">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="c5154-407">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="c5154-407">Az.EventHub</span></span>
* <span data-ttu-id="c5154-408">Eventhub의 CaptureDescription 클래스에서 빈 보관을 건너뛰는 새 부울 속성 SkipEmptyArchives가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-408">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="c5154-409">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5154-409">Az.KeyVault</span></span>
* <span data-ttu-id="c5154-410">Set-AzKeyVaultSecret 태그 지정 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-410">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c5154-411">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c5154-411">Az.LogicApp</span></span>
* <span data-ttu-id="c5154-412">통합 계정에 대한 기본 sku 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-412">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="c5154-413">XSLT 2.0, XSLT 3.0, Liquid 맵 형식 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-413">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="c5154-414">통합 계정 어셈블리에 대한 새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="c5154-414">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="c5154-415">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c5154-415">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c5154-416">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c5154-416">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c5154-417">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c5154-417">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="c5154-418">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="c5154-418">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="c5154-419">통합 계정 일괄 처리 구성에 대한 새 cmdlet</span><span class="sxs-lookup"><span data-stu-id="c5154-419">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="c5154-420">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5154-420">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c5154-421">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5154-421">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c5154-422">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5154-422">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="c5154-423">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5154-423">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="c5154-424">논리 앱 SDK를 버전 4.1.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-424">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="c5154-425">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c5154-425">Az.Monitor</span></span>
* <span data-ttu-id="c5154-426">Get-AzMetric에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-426">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c5154-427">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-427">Az.Network</span></span>
* <span data-ttu-id="c5154-428">Add-AzApplicationGatewayCustomError에 대한 도움말 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-428">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="c5154-429">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c5154-429">Az.OperationalInsights</span></span>
* <span data-ttu-id="c5154-430">New 및 Get ApplicationInsights 데이터 소스에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-430">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="c5154-431">지정된 작업 영역에 대한 특정 또는 전체 ApplicationInsights 데이터 원본 가져오기를 지원하기 위한 새로운 'ApplicationInsights' 종류가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-431">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="c5154-432">지정된 Application-Insights 리소스 매개 변수(구독 ID, resourceGroupName 및 이름)별로 데이터 원본을 만들기 위한 New-AzOperationalInsightsApplicationInsightsDataSource cmdlet이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-432">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="c5154-433">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-433">Az.Resources</span></span>
* <span data-ttu-id="c5154-434">문제 https://github.com/Azure/azure-powershell/issues/8166 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-434">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="c5154-435">문제 https://github.com/Azure/azure-powershell/issues/8235 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-435">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="c5154-436">문제 https://github.com/Azure/azure-powershell/issues/6219 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-436">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="c5154-437">KeyCredentials 반복 만들기를 방지하기 위해 버그 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-437">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="c5154-438">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-438">Az.Sql</span></span>
* <span data-ttu-id="c5154-439">SQL DB 하이퍼스케일에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-439">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="c5154-440">복원 요청에서 불필요한 속성을 설정하여 복원이 실패할 수 있는 버그 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-440">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c5154-441">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c5154-441">Az.Websites</span></span>
* <span data-ttu-id="c5154-442">Get-AzWebAppSlotMetrics 내 올바른 예제</span><span class="sxs-lookup"><span data-stu-id="c5154-442">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="c5154-443">1.3.0 - 2019년 2월</span><span class="sxs-lookup"><span data-stu-id="c5154-443">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c5154-444">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c5154-444">Az.Accounts</span></span>
* <span data-ttu-id="c5154-445">ClientRuntime 최신 버전 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-445">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c5154-446">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c5154-446">Az.AnalysisServices</span></span>
<span data-ttu-id="c5154-447">Az.AnalysisServices 모듈의 전반적인 가용성.</span><span class="sxs-lookup"><span data-stu-id="c5154-447">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-448">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-448">Az.Compute</span></span>
* <span data-ttu-id="c5154-449">AEM 확장: UltraSSD 및 P60, P70, P80 디스크에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-449">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="c5154-450">Set-AzVMBootDiagnostics에 대한 도움말 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-450">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="c5154-451">Update-AzImage에 대한 도움말 및 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-451">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c5154-452">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c5154-452">Az.RecoveryServices</span></span>
<span data-ttu-id="c5154-453">Az.RecoveryServices 모듈의 전반적인 가용성.</span><span class="sxs-lookup"><span data-stu-id="c5154-453">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c5154-454">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-454">Az.Resources</span></span>
* <span data-ttu-id="c5154-455">리소스 그룹 관련 태그 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-455">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="c5154-456">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8166를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-456">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="c5154-457">`Get-AzureRmRoleAssignment`이(가) -ErrorAction을 준수하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-457">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="c5154-458">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8235를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-458">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="c5154-459">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-459">Az.Sql</span></span>
* <span data-ttu-id="c5154-460">AzSqlDatabaseBackupShortTermRetentionPolicy 가져오기/설정하기 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-460">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="c5154-461">SQL cmdlet을 실행할 경우 Azure 계정에 로그인되어 있지 않은 것이 nullref 예외를 초래하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-461">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="c5154-462">Get-AzSqlCapability의 nullref 예외 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-462">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="c5154-463">1.2.1 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="c5154-463">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c5154-464">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c5154-464">Az.Accounts</span></span>
* <span data-ttu-id="c5154-465">올바른 인증 버전을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="c5154-465">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="c5154-466">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="c5154-466">Az.AnalysisServices</span></span>
* <span data-ttu-id="c5154-467">업데이트된 인증 종속성을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="c5154-467">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="c5154-468">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c5154-468">Az.RecoveryServices</span></span>
* <span data-ttu-id="c5154-469">업데이트된 인증 종속성을 사용하여 릴리스</span><span class="sxs-lookup"><span data-stu-id="c5154-469">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="c5154-470">1.2.0 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="c5154-470">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c5154-471">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c5154-471">Az.Accounts</span></span>
* <span data-ttu-id="c5154-472">Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-472">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="c5154-473">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-473">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c5154-474">Uninstall-AzureRm 관련 PS Core에 경고 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-474">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="c5154-475">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="c5154-475">Az.Aks</span></span>
* <span data-ttu-id="c5154-476">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-476">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="c5154-477">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c5154-477">Az.Automation</span></span>
* <span data-ttu-id="c5154-478">Python 2 Runbook에 대한 지원이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-478">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="c5154-479">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-479">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="c5154-480">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="c5154-480">Az.Cdn</span></span>
* <span data-ttu-id="c5154-481">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-481">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-482">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-482">Az.Compute</span></span>
* <span data-ttu-id="c5154-483">Invoke-AzVMReimage cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-483">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="c5154-484">Set-AzVmss에 TempDisk 매개 변수 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-484">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="c5154-485">New-AzVM 경고 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-485">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="c5154-486">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="c5154-486">Az.ContainerRegistry</span></span>
* <span data-ttu-id="c5154-487">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-487">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="c5154-488">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="c5154-488">Az.DataFactory</span></span>
* <span data-ttu-id="c5154-489">ADF.Net SDK 버전이 3.0.0으로 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-489">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c5154-490">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c5154-490">Az.DataLakeStore</span></span>
* <span data-ttu-id="c5154-491">MSI를 사용할 때 ADLS 엔드포인트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-491">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="c5154-492">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7462를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-492">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="c5154-493">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-493">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c5154-494">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c5154-494">Az.IotHub</span></span>
* <span data-ttu-id="c5154-495">Add-IotHubRoutingEndpoint cmdlet에 인코딩 형식을 추가하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-495">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="c5154-496">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5154-496">Az.KeyVault</span></span>
* <span data-ttu-id="c5154-497">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-497">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c5154-498">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-498">Az.Network</span></span>
* <span data-ttu-id="c5154-499">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-499">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="c5154-500">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-500">Az.Resources</span></span>
* <span data-ttu-id="c5154-501">'New-AzADAppCredential' 및 'New-AzADSpCredential' 참조 설명서의 잘못된 예제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-501">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="c5154-502">리소스 그룹 배포 cmdlet 실행 전 '-TemplateFile' 매개 변수 경로가 확인되지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-502">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="c5154-503">Az.Resources: New-AzureRmPolicyDefinition -Mode 기본값에 대한 올바른 설명서</span><span class="sxs-lookup"><span data-stu-id="c5154-503">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="c5154-504">Az.Resources: 문제 https://github.com/Azure/azure-powershell/issues/7522 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-504">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="c5154-505">Az.Resources: 문제 https://github.com/Azure/azure-powershell/issues/5747 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-505">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="c5154-506">'PSResourceGroupDeployment' 개체의 서식 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-506">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="c5154-507">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/2123를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-507">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c5154-508">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c5154-508">Az.ServiceFabric</span></span>
* <span data-ttu-id="c5154-509">인증서가 VMSS 모델에 추가되었는데도 예외가 발생할 경우 롤백합니다. 이는 버그 https://github.com/Azure/service-fabric-issues/issues/932를 수정하기 위함입니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-509">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="c5154-510">일부 오류 메시지를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-510">Fix some error messages.</span></span>
* <span data-ttu-id="c5154-511">Az로의 마이그레이션을 통해서는 작동하지 않는 New-AzServiceFabriCluster를 위해 기본값 ARM 템플릿을 가진 클러스터 만들기를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-511">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="c5154-512">확장에서 클러스터 id를 확인하여 클러스터에 해당하는 VMSS에만 추가되도록 클러스터/애플리케이션 인증서 추가를 수정하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-512">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c5154-513">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c5154-513">Az.SignalR</span></span>
* <span data-ttu-id="c5154-514">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-514">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="c5154-515">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-515">Az.Sql</span></span>
* <span data-ttu-id="c5154-516">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-516">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c5154-517">가능한 값을 가진 LicenseType 매개 변수에 대한 매개 변수 설명이 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-517">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="c5154-518">유일하게 업데이트된 속성인데 작동하지 않는 관리되는 인스턴스 ID의 업데이트 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-518">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="c5154-519">관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-519">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c5154-520">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c5154-520">Az.Storage</span></span>
* <span data-ttu-id="c5154-521">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-521">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c5154-522">Premium Storage 계정이 클래식 로깅/메트릭을 지원하지 않기 때문에, Premium Storage 계정의 클래식 로깅/메트릭을 가져올/설정할 때 상세한 오류 메시지를 제공해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-522">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="c5154-523">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="c5154-523">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="c5154-524">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="c5154-524">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="c5154-525">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="c5154-525">Az.TrafficManager</span></span>
* <span data-ttu-id="c5154-526">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-526">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c5154-527">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c5154-527">Az.Websites</span></span>
* <span data-ttu-id="c5154-528">잘못된 온라인 도움말 URL 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-528">Update incorrect online help URLs</span></span>
* <span data-ttu-id="c5154-529">앱이 ASE에 호스팅되면 'New-AzWebAppSSLBinding'을 수정하여 올바른 resourcegroup+location에 인증서를 업로드합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-529">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="c5154-530">'New-AzWebAppSSLBinding'을 수정하여 SSL 인증서를 앱에 바인딩하는 데 붙는 태그를 덮어쓰지 않도록 합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-530">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="c5154-531">1.1.0 - 2019년 1월</span><span class="sxs-lookup"><span data-stu-id="c5154-531">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="c5154-532">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c5154-532">Az.Accounts</span></span>
* <span data-ttu-id="c5154-533">Enable-AzureRmAlias에 'Local' 범위 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-533">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-534">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-534">Az.Compute</span></span>
* <span data-ttu-id="c5154-535">이름이 Restart/Start/Stop/Remove/Set-AzVM과 Save-AzVMImage에 설정된 ID 매개 변수에서 선택 사항이 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-535">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="c5154-536">도움말 파일의 ID에 대한 설명이 업데이트 되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-536">Updated the description of ID in help files</span></span>
* <span data-ttu-id="c5154-537">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-537">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c5154-538">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c5154-538">Az.DataLakeStore</span></span>
* <span data-ttu-id="c5154-539">SDK 수정을 위해 데이터 평면의 SDK 버전을 1.1.14로 업데이트하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-539">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="c5154-540">getfilestatus 및 liststatus에 대한 음수 acesstime 및 modificationtime 수정, 비동기 취소 토큰 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-540">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="c5154-541">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="c5154-541">Az.EventGrid</span></span>
* <span data-ttu-id="c5154-542">2019-01-01 API 버전을 사용하도록 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-542">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="c5154-543">2019-01-01 API 버전에서 새 시나리오를 지원하도록 다음 cmdlet을 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-543">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="c5154-544">New-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-544">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="c5154-545">이벤트 Time-to-Live</span><span class="sxs-lookup"><span data-stu-id="c5154-545">Event Time-To-Live,</span></span>
        - <span data-ttu-id="c5154-546">이벤트에 대한 최대 배달 시도</span><span class="sxs-lookup"><span data-stu-id="c5154-546">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="c5154-547">배달 못한 편지의 엔드포인트입니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-547">Dead letter endpoint.</span></span>
    - <span data-ttu-id="c5154-548">Update-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-548">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="c5154-549">이벤트 Time-to-Live</span><span class="sxs-lookup"><span data-stu-id="c5154-549">Event Time-To-Live,</span></span>
        - <span data-ttu-id="c5154-550">이벤트에 대한 최대 배달 시도</span><span class="sxs-lookup"><span data-stu-id="c5154-550">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="c5154-551">배달 못한 편지의 엔드포인트입니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-551">Dead letter endpoint.</span></span>
* <span data-ttu-id="c5154-552">New-AzureRmEventGridSubscription 및 Update-AzureRmEventGridSubscription cmdlet의 EndpointType 옵션에 새 열거형 값(즉, storageQueue 및 hybridConnection)을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-552">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="c5154-553">이벤트 구독을 생성 또는 업데이트할 때 사용자가 직접 조치를 취해야 할 경우 경고 메시지를 표시합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-553">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="c5154-554">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="c5154-554">Az.IotHub</span></span>
* <span data-ttu-id="c5154-555">최신 버전의 Azure IotHub SDK로 업데이트됨</span><span class="sxs-lookup"><span data-stu-id="c5154-555">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="c5154-556">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="c5154-556">Az.LogicApp</span></span>
* <span data-ttu-id="c5154-557">지정된 이름이 없는 모든 Get-AzLogicApp 목록</span><span class="sxs-lookup"><span data-stu-id="c5154-557">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="c5154-558">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-558">Az.Resources</span></span>
* <span data-ttu-id="c5154-559">'Get-AzResource'에 '-ODataQuery'및 '-ResourceId' 매개 변수를 제공할 때 매개 변수 집합 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-559">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="c5154-560">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7875를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-560">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="c5154-561">New/Set-AzPolicyDefinition에서 -Custom 매개 변수 처리 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-561">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="c5154-562">New-AzDeployment 설명서에서 오타 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-562">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="c5154-563">'New-AzADUser'에 '-MailNickname'매개 변수가 필수 항목으로 지정됨</span><span class="sxs-lookup"><span data-stu-id="c5154-563">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="c5154-564">자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8220를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-564">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="c5154-565">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="c5154-565">Az.SignalR</span></span>
* <span data-ttu-id="c5154-566">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-566">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="c5154-567">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-567">Az.Sql</span></span>
* <span data-ttu-id="c5154-568">Storage 관리 클라이언트 종속성을 일반적인 SDK 구현으로 변환했습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-568">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="c5154-569">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c5154-569">Az.Storage</span></span>
* <span data-ttu-id="c5154-570">Sas Token, OAuth 또는 Anonymous를 사용하여 스토리지 컨텍스트의 StorageAccountName을 실제 스토리지 계정 이름으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-570">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="c5154-571">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="c5154-571">New-AzStorageContext</span></span>
* <span data-ttu-id="c5154-572">'-FullUri' 매개 변수를 사용하여 BLOB 스냅숏 개체의 Sas Token을 생성하고 반환된 Uri를 스냅숏 Uri로 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-572">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="c5154-573">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="c5154-573">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c5154-574">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c5154-574">Az.Websites</span></span>
* <span data-ttu-id="c5154-575">'Get-AzDeletedWebApp'의 날짜 구문 분석 버그를 수정했습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-575">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="c5154-576">Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-576">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="c5154-577">1.0.0 - 2018년 12월</span><span class="sxs-lookup"><span data-stu-id="c5154-577">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="c5154-578">일반</span><span class="sxs-lookup"><span data-stu-id="c5154-578">General</span></span>

- <span data-ttu-id="c5154-579">Az 모듈 일반 공급</span><span class="sxs-lookup"><span data-stu-id="c5154-579">General Availability of Az Module</span></span>
- <span data-ttu-id="c5154-580">각 모듈에 대 한 온라인 도움말</span><span class="sxs-lookup"><span data-stu-id="c5154-580">Online help for each module</span></span>
- <span data-ttu-id="c5154-581">자세한 내용과 로드맵은 [Az 알림 페이지](https://aka.ms/azps-announce)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-581">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="c5154-582">AzureRM에서 마이그레이션하는 것에 대한 정보는 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-582">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="c5154-583">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="c5154-583">Az.Accounts</span></span>
- <span data-ttu-id="c5154-584">Az.Profile에서 변경</span><span class="sxs-lookup"><span data-stu-id="c5154-584">Changed from Az.Profile</span></span>
- <span data-ttu-id="c5154-585">프로필 및 컨텍스트 형식에 대한 표 형식 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-585">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="c5154-586">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c5154-586">Az.ApiManagement</span></span>
- <span data-ttu-id="c5154-587">#7002에 대한 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-587">Fixes for #7002</span></span>
- <span data-ttu-id="c5154-588">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-588">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="c5154-589">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="c5154-589">Az.Batch</span></span>
- <span data-ttu-id="c5154-590">`PSComputeNode`의 새로운 `NodeAgentInformation` 속성을 통해 풀의 각 VM에서 실행 중인 Azure Batch 노드 에이전트의 버전을 확인하는 기능이 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-590">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="c5154-591">`PSDataDisk`에 대한 `Caching` 기본 값은 이제 `None` 대신 `ReadWrite`입니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-591">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="c5154-592">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-592">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="c5154-593">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="c5154-593">Az.Billing</span></span>
- <span data-ttu-id="c5154-594">청구, 소비 및 UsageAggregates cmdlet 결합 cmdlet에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-594">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="c5154-595">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="c5154-595">Az.CognitivServices</span></span>
- <span data-ttu-id="c5154-596">New-AzureRmCognitiveServicesAccount 작업에서 사용 가능한 SkuName 및 Typem에 대한 완성자 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-596">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="c5154-597">Get-AzCognitiveServicesAccountSkus에서 GetSkusWithAccountParamSetName 매개 변수 집합을 제거</span><span class="sxs-lookup"><span data-stu-id="c5154-597">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="c5154-598">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c5154-598">Az.ContainerInstance</span></span>
- <span data-ttu-id="c5154-599">ManagedIdentity 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="c5154-599">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="c5154-600">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="c5154-600">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="c5154-601">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-601">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="c5154-602">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c5154-602">Az.DataLakeStore</span></span>
- <span data-ttu-id="c5154-603">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-603">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="c5154-604">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="c5154-604">Az.Monitor</span></span>
- <span data-ttu-id="c5154-605">Az.Monitor 이름 변경 및 기타 사소한 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-605">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="c5154-606">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="c5154-606">Az.KeyVault</span></span>
- <span data-ttu-id="c5154-607">출력 형식에서 사용되지 않는 'PurgeDisabled' 속성 제거</span><span class="sxs-lookup"><span data-stu-id="c5154-607">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="c5154-608">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="c5154-608">Az.MachineLearning</span></span>
- <span data-ttu-id="c5154-609">Az.MachineLearningCompute 모듈의 cmdlet 포함</span><span class="sxs-lookup"><span data-stu-id="c5154-609">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="c5154-610">Az.Media</span><span class="sxs-lookup"><span data-stu-id="c5154-610">Az.Media</span></span>
- <span data-ttu-id="c5154-611">New-AzMediaService에서 사용되지 않는 -Tags 별칭이 제거됨</span><span class="sxs-lookup"><span data-stu-id="c5154-611">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="c5154-612">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-612">Az.Network</span></span>
<span data-ttu-id="c5154-613">Application Gateway에서 RewriteRuleSets를 구성하는 것에 대한 지원이 추가됨</span><span class="sxs-lookup"><span data-stu-id="c5154-613">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="c5154-614">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-614">New cmdlets added:</span></span>
        - <span data-ttu-id="c5154-615">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c5154-615">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c5154-616">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c5154-616">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c5154-617">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c5154-617">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c5154-618">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c5154-618">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c5154-619">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c5154-619">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="c5154-620">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="c5154-620">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="c5154-621">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="c5154-621">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="c5154-622">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="c5154-622">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="c5154-623">선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -RewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="c5154-623">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="c5154-624">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="c5154-624">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="c5154-625">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="c5154-625">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="c5154-626">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="c5154-626">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="c5154-627">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="c5154-627">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="c5154-628">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="c5154-628">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="c5154-629">New-AzureRmApplicationGatewayUrlPathMapConfig로 ID를 사용하여 Application Gateway에 KeyVault 지원을 추가했습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-629">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="c5154-630">선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -KeyVaultSecretId, -KeyVaultSecret</span><span class="sxs-lookup"><span data-stu-id="c5154-630">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="c5154-631">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c5154-631">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="c5154-632">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c5154-632">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="c5154-633">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="c5154-633">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="c5154-634">New-AzApplicationGateway cmdlet이 선택적 매개 변수를 사용하도록 업데이트됨 -UserAssignedIdentity</span><span class="sxs-lookup"><span data-stu-id="c5154-634">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="c5154-635">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-635">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="c5154-636">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="c5154-636">Az.OperationalInsights</span></span>
- <span data-ttu-id="c5154-637">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-637">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="c5154-638">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c5154-638">Az.Profile</span></span>
- <span data-ttu-id="c5154-639">Az.Accounts에 모듈 이름이 변경됨</span><span class="sxs-lookup"><span data-stu-id="c5154-639">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="c5154-640">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c5154-640">Az.RecoveryServices</span></span>
- <span data-ttu-id="c5154-641">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-641">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="c5154-642">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-642">Az.Resources</span></span>
- <span data-ttu-id="c5154-643">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-643">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="c5154-644">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c5154-644">Az.ServiceFabric</span></span>
- <span data-ttu-id="c5154-645">일반 이름과 지문으로 지정 인증서 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-645">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="c5154-646">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-646">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="c5154-647">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="c5154-647">Az.SIgnalR</span></span>
- <span data-ttu-id="c5154-648">SIgnalR에 대한 PowerShell cmdlet에 대한 일반 공급</span><span class="sxs-lookup"><span data-stu-id="c5154-648">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="c5154-649">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-649">Az.Sql</span></span>
- <span data-ttu-id="c5154-650">위협 탐지의 cmdlet에 새로운 Data_Exfiltration 및 Unsafe_Action 검색 유형 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-650">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="c5154-651">Sql 감사 cmdlet에 대한 설명서 예제 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-651">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="c5154-652">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-652">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="c5154-653">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c5154-653">Az.Storage</span></span>
- <span data-ttu-id="c5154-654">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-654">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="c5154-655">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c5154-655">Az.Websites</span></span>
- <span data-ttu-id="c5154-656">부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="c5154-656">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="c5154-657">0.7.0 - 2018년 12월</span><span class="sxs-lookup"><span data-stu-id="c5154-657">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="c5154-658">일반</span><span class="sxs-lookup"><span data-stu-id="c5154-658">General</span></span>

* <span data-ttu-id="c5154-659">AzureRM에서 Az 전환 예정에 대한 사소한 변경</span><span class="sxs-lookup"><span data-stu-id="c5154-659">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="c5154-660">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-660">Az.Compute</span></span>

* <span data-ttu-id="c5154-661">`New-AzVm(ss)` cmdlet에 대한 간단한 매개 변수 집합에 UltraSSD 및 갤러리 이미지에 대한 지원을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-661">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="c5154-662">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c5154-662">Az.DataLakeStore</span></span>

* <span data-ttu-id="c5154-663">ADLS 계정의 도메인의 후행 슬래시를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-663">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="c5154-664">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="c5154-664">Az.FrontDoor</span></span>

* <span data-ttu-id="c5154-665">일부 끊어진 링크 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-665">Fixed some broken links</span></span>
    - <span data-ttu-id="c5154-666">New-AzureRmFrontDoor 및 Set-AzureRmFrontDoor 아티클에서 New-AzureRmFrontDoorHealthProbeSettingObject cmdlet 아티클에 대한 링크가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-666">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="c5154-667">New-AzureRmFrontDoorManagedRuleObject 아티클에서 New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet 아티클에 대한 링크가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-667">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="c5154-668">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="c5154-668">Az.RecoveryServices</span></span>

* <span data-ttu-id="c5154-669">Azure File Share 복원 작업에 클라이언트 측 유효성 검사가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-669">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="c5154-670">afs 복원의 경우 storageAccountName 및 storageAccountResourceGroupName을 선택적으로 만들었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-670">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="c5154-671">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-671">Az.Resources</span></span>

* <span data-ttu-id="c5154-672">에 대 한 수정 https://github.com/Azure/azure-powershell/issues/7679</span><span class="sxs-lookup"><span data-stu-id="c5154-672">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="c5154-673">기본 관리자를 요청할 때 구독 범위가 제공되는 경우 Get-AzureRmRoleAssignment를 업데이트하여 구독 범위를 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-673">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="c5154-674">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-674">Az.Sql</span></span>

* <span data-ttu-id="c5154-675">AzureRM에서 Az 전환 예정에 대한 사소한 변경</span><span class="sxs-lookup"><span data-stu-id="c5154-675">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="c5154-676">DotNet 코어에서 Get-AzureRmSqlDatabaseVulnerabilityAssessment를 사용하는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="c5154-676">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="c5154-677">SQL 감사 cmdlet과 관련된 도움말 메시지의 설명서가 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-677">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="c5154-678">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="c5154-678">Az.Storage</span></span>

* <span data-ttu-id="c5154-679">New-AzureRmStorageAccount에 -EnableHierarchicalNamespace 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-679">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="c5154-680">파일 복사 cmdlet이 -DestContext 입력이 없을 때 대상의 원본 컨텍스트를 다시 사용할 수 없는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-680">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="c5154-681">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="c5154-681">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="c5154-682">고정적인 웹 사이트 구성 지원</span><span class="sxs-lookup"><span data-stu-id="c5154-682">Support Static Website configuration</span></span>
    - <span data-ttu-id="c5154-683">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c5154-683">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="c5154-684">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="c5154-684">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="c5154-685">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c5154-685">Az.Websites</span></span>

* <span data-ttu-id="c5154-686">Set-AzureRmWebApp 및 Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="c5154-686">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="c5154-687">Windows 및 Linux 컨테이너 응용 프로그램에 탑재할 Azure Storage 경로를 지정하기 위해 새 매개 변수(-AzureStoragePath)가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-687">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="c5154-688">새 cmdlet New-AzureRmWebAppAzureStoragePath의 출력을 매개 변수로 사용하여 Azure Storage 경로를 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-688">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="c5154-689">0.6.1 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="c5154-689">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="c5154-690">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="c5154-690">Az.ApiManagement</span></span>
* <span data-ttu-id="c5154-691">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-691">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="c5154-692">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="c5154-692">Az.Automation</span></span>
* <span data-ttu-id="c5154-693">Azure Automation cmdlet 기반 Swagger</span><span class="sxs-lookup"><span data-stu-id="c5154-693">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="c5154-694">업데이트 관리 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-694">Added Update Management cmdlets</span></span>
* <span data-ttu-id="c5154-695">소스 제어 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-695">Added Source Control cmdlets</span></span>
* <span data-ttu-id="c5154-696">Remove-AzureRmAutomationHybridWorkerGroup cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-696">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="c5154-697">DSC 노드 등록 명령 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-697">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="c5154-698">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-698">Az.Compute</span></span>
* <span data-ttu-id="c5154-699">SystemAssigned ID에 대한 ID 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-699">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="c5154-700">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-700">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="c5154-701">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="c5154-701">Az.ContainerInstance</span></span>
* <span data-ttu-id="c5154-702">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-702">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="c5154-703">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="c5154-703">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="c5154-704">마켓플레이스 cmdlet에 대한 예제 설명 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-704">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="c5154-705">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-705">Az.Network</span></span>
* <span data-ttu-id="c5154-706">New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-706">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="c5154-707">지원되는 AzureFirewall 네트워크 프로토콜에 ICMP 다시 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-707">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="c5154-708">Test-AzureRmNetworkWatcherConnectivity cmdlet을 업데이트하여 대상 ID, 주소 및 포트 유효성 검사를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-708">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="c5154-709">VirtualNetwork 맵의 메모리 사용 문제 해결</span><span class="sxs-lookup"><span data-stu-id="c5154-709">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="c5154-710">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="c5154-710">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="c5154-711">보호된 파일 공유에 대한 정책을 수정하는 것에 대해 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-711">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="c5154-712">정책 표준 시간대를 대문자로 변환했습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-712">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="c5154-713">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="c5154-713">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="c5154-714">New-AzureRmRecoveryServicesAsrProtectableItem의 예제 정정</span><span class="sxs-lookup"><span data-stu-id="c5154-714">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="c5154-715">형식 매핑 문제에 대한 종속성 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-715">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="c5154-716">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="c5154-716">Az.Relay</span></span>
* <span data-ttu-id="c5154-717">선택적 매개 변수 -KeyValue를 New-AzureRmRelayKey cmdlet에 추가하여 사용자가 KeyValue를 제공할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-717">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="c5154-718">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-718">Az.Resources</span></span>
* <span data-ttu-id="c5154-719">`New-AzureRmPolicyAssignment` 및 `Set-AzureRmPolicyAssignment`의 자원 ID 관련 매개 변수에 대한 도움말 문서를 업데이트함</span><span class="sxs-lookup"><span data-stu-id="c5154-719">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="c5154-720">-Metadata를 사용하는 New-AzureRmPolicyDefinition에 대한 예제 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-720">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="c5154-721">NetStandard의 태그 키에서 대소문자 보존을 허용하도록 수정: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="c5154-721">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="c5154-722">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c5154-722">Az.ServiceFabric</span></span>
* <span data-ttu-id="c5154-723">향후 호환성이 손상되는 변경에 대한 사용 중단 메시지 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-723">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="c5154-724">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-724">Az.Sql</span></span>
* <span data-ttu-id="c5154-725">Azure Sql Database Managed Instance 및 Azure Sql Managed Database에 CRUD 작업을 위한 새 cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-725">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="c5154-726">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c5154-726">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c5154-727">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c5154-727">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c5154-728">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c5154-728">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c5154-729">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="c5154-729">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="c5154-730">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c5154-730">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c5154-731">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c5154-731">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c5154-732">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c5154-732">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="c5154-733">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="c5154-733">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="c5154-734">서버 또는 데이터베이스에서 확장 감사 정책 관리를 활성화했습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-734">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="c5154-735">새 매개 변수(PredicateExpression)가 감사 로그 필터링을 사용하도록 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-735">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="c5154-736">Cmdlet이 레거시 클라이언트 대신 SQL 클라이언트를 사용하도록 수정되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-736">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="c5154-737">Set-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="c5154-737">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="c5154-738">Get-AzureRmSqlServerAuditing.</span><span class="sxs-lookup"><span data-stu-id="c5154-738">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="c5154-739">Set-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="c5154-739">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="c5154-740">Get-AzureRmSqlDatabaseAuditing.</span><span class="sxs-lookup"><span data-stu-id="c5154-740">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="c5154-741">스토리지 계정 이름 매개 변수가 설정된 Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings를 사용할 때의 문제 해결</span><span class="sxs-lookup"><span data-stu-id="c5154-741">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="c5154-742">0.5.0 - 2018년 11월</span><span class="sxs-lookup"><span data-stu-id="c5154-742">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="c5154-743">일반</span><span class="sxs-lookup"><span data-stu-id="c5154-743">General</span></span>
* <span data-ttu-id="c5154-744">많은 핵심 cmdlet에 Resource Completers를 추가하여 대화형으로 cmdlet을 호출할 때 기존 리소스 이름을 탭으로 이동할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-744">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="c5154-745">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c5154-745">Az.Profile</span></span>
* <span data-ttu-id="c5154-746">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-746">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="c5154-747">Connect-AzAccount cmdlet의 매개 변수 TenantId 이름을 Tenant로 바꾸고 TenantId의 별칭을 추가합니다</span><span class="sxs-lookup"><span data-stu-id="c5154-747">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="c5154-748">Connect-AzAccount의 업데이트된 TenantId 설명</span><span class="sxs-lookup"><span data-stu-id="c5154-748">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="c5154-749">테넌트 도메인을 제공할 때 실패한 로그인에 대한 오류 메시지 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-749">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="c5154-750">테넌트에 구독이 없는 계정의 컨텍스트 이름 충돌 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-750">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="c5154-751">MSI를 사용할 때 DataLake 엔드포인트 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-751">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="c5154-752">연결되지 않은 경우 'Disconnect-AzAccount'가 throw하는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-752">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="c5154-753">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c5154-753">Az.CognitiveServices</span></span>
* <span data-ttu-id="c5154-754">Get-AzCognitiveServicesAccountSkus 작업을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-754">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-755">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-755">Az.Compute</span></span>
* <span data-ttu-id="c5154-756">Add-AzVmssVMDataDisk 및 Remove-AzVmssVMDataDisk cmdlet를 추가합니다</span><span class="sxs-lookup"><span data-stu-id="c5154-756">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="c5154-757">Get-AzVMImage는 AutomaticOSUpgradeProperties를 표시합니다</span><span class="sxs-lookup"><span data-stu-id="c5154-757">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="c5154-758">수정된 SetAzVMChefExtension -BootstrapOptions 및 -JsonAttribute option 값이 json 형식으로 설정하지 않습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-758">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c5154-759">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c5154-759">Az.DataLakeStore</span></span>
* <span data-ttu-id="c5154-760">DataLake 패키지를 1.1.10으로 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-760">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="c5154-761">기본 동시성을 다중 스레드 작업에 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-761">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="c5154-762">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="c5154-762">Az.Insights</span></span>
* <span data-ttu-id="c5154-763">해결된 문제 #7267(자동 크기 조정 영역)</span><span class="sxs-lookup"><span data-stu-id="c5154-763">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="c5154-764">열거된 매개 변수를 제대로 설정하지 않은 새 자동 크기 조정 규칙을 만드는 데 문제가 있습니다(이를 항상 기본값으로 설정함).</span><span class="sxs-lookup"><span data-stu-id="c5154-764">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="c5154-765">해결된 문제 # 7513[자세한 정보] Set-AzDiagnosticSetting은 설정을 생성하는 동안 범주를 명시적으로 지정해야 합니다</span><span class="sxs-lookup"><span data-stu-id="c5154-765">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="c5154-766">이제 cmdlet은 생성 중에 사용할 범주를 명시적으로 표시할 필요가 없습니다. 즉, 문서화된대로 작동합니다</span><span class="sxs-lookup"><span data-stu-id="c5154-766">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c5154-767">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-767">Az.Network</span></span>
* <span data-ttu-id="c5154-768">다음 cmdlet에 대해 PeeringType을 필수 매개 변수로 변경했습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-768">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="c5154-769">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="c5154-769">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="c5154-770">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="c5154-770">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="c5154-771">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="c5154-771">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="c5154-772">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="c5154-772">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="c5154-773">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="c5154-773">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="c5154-774">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="c5154-774">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="c5154-775">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="c5154-775">Az.PolicyInsights</span></span>
* <span data-ttu-id="c5154-776">추가된 정책 재구성 cmdlet</span><span class="sxs-lookup"><span data-stu-id="c5154-776">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="c5154-777">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-777">Az.Resources</span></span>
* <span data-ttu-id="c5154-778">에 대 한 수정 https://github.com/Azure/azure-powershell/issues/7402</span><span class="sxs-lookup"><span data-stu-id="c5154-778">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="c5154-779">'Get-AzResource'에 대해 '-ResourceId' 매개 변수를 사용하여 리소스 나열 허용</span><span class="sxs-lookup"><span data-stu-id="c5154-779">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="c5154-780">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="c5154-780">Az.ServiceBus</span></span>
* <span data-ttu-id="c5154-781">마이그레이션 상태를 알 수 있도록 PSServiceBusMigrationConfigurationAttributes에 MigrationState 읽기 전용 속성 추가.</span><span class="sxs-lookup"><span data-stu-id="c5154-781">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="c5154-782">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="c5154-782">Az.ServiceFabric</span></span>
* <span data-ttu-id="c5154-783">Linux Vmss에 인증서 추가 수정.</span><span class="sxs-lookup"><span data-stu-id="c5154-783">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="c5154-784">Add-AzServiceFabricClusterCertificate 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-784">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="c5154-785">새 인증서(Azure/service-fabric-issues#932)에서 올바른 지문을 사용.</span><span class="sxs-lookup"><span data-stu-id="c5154-785">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="c5154-786">올바르게 예외 표시(Azure/service-fabric-issues#1054).</span><span class="sxs-lookup"><span data-stu-id="c5154-786">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="c5154-787">Vmss CreateOrUpdate 작업을 시작하기 전에 'Update-AzServiceFabricDurability'를 수정하여 클러스터 구성 업데이트.</span><span class="sxs-lookup"><span data-stu-id="c5154-787">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="c5154-788">0.4.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="c5154-788">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="c5154-789">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="c5154-789">Az.Profile</span></span>
* <span data-ttu-id="c5154-790">CloudShell에서 Get-AzSubscription을 사용하여 문제를 해결합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-790">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="c5154-791">ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-791">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-792">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-792">Az.Compute</span></span>
* <span data-ttu-id="c5154-793">'New-AzVm'에 대해 간단한 매개 변수를 사용하는 경우 가속화된 네트워킹을 설정하기 위해 새 크기가 VM 크기의 허용 목록에 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-793">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="c5154-794">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-794">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="c5154-795">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="c5154-795">Az.DataLakeStore</span></span>
* <span data-ttu-id="c5154-796">Virtual Network 규칙에 대한 지원 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-796">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="c5154-797">Get-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 가져오거나 나열합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-797">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="c5154-798">Add-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 가상 네트워크 규칙을 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-798">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="c5154-799">Set-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 지정된 가상 네트워크 규칙을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-799">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="c5154-800">Remove-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-800">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c5154-801">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-801">Az.Network</span></span>
* <span data-ttu-id="c5154-802">Test-AzNetworkWatcherConnectivity cmdlet을 업데이트하고, 백 엔드에 프로토콜 값을 전달합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-802">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="c5154-803">모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-803">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="c5154-804">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-804">Az.Resources</span></span>
* <span data-ttu-id="c5154-805">(기본 프로필에 구독이 없고 범위가 지정되지 않은 경우) 시나리오에서 의미 있는 예외를 추가하여 Get-AzRoleDefinition이 인식할 수 없는 예외를 throw하는 문제를 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-805">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="c5154-806">또한 기본 매개 변수 집합을 'RoleDefinitionNameParameterSet'으로 설정합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-806">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="c5154-807">0.3.0 - 2018년 10월</span><span class="sxs-lookup"><span data-stu-id="c5154-807">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="c5154-808">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="c5154-808">Azure.Storage</span></span>
* <span data-ttu-id="c5154-809">대상에 메타데이터가 있을 때 Blob/파일이 메타 데이터를 복사하지 않는 문제 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-809">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="c5154-810">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="c5154-810">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="c5154-811">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="c5154-811">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="c5154-812">특정 위치의 저장소 리소스 사용을 지원하고 글로벌 저장소 리소스 사용 가져오기는 더 이상 사용되지 않는다는 경고 메시지를 추가합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-812">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="c5154-813">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="c5154-813">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="c5154-814">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="c5154-814">Az.CognitiveServices</span></span>
* <span data-ttu-id="c5154-815">기존 계정이 없는 Get-AzCognitiveServicesAccountSkus를 지원합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-815">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="c5154-816">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="c5154-816">Az.Compute</span></span>
* <span data-ttu-id="c5154-817">Get-AzVM -ResourceGroupName <rg>가 필요한 경우 50개가 넘는 결과를 반환하도록 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-817">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="c5154-818">'SimpleParameterSet' 예제가 New-AzVmss cmdlet 도움말에 추가됨</span><span class="sxs-lookup"><span data-stu-id="c5154-818">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="c5154-819">Azure Disk Encryption 진행률 메시지의 오타를 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-819">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="c5154-820">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="c5154-820">Az.DataFactoryV2</span></span>
* <span data-ttu-id="c5154-821">ADF.Net SDK 버전을 2.3.0으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="c5154-821">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="c5154-822">Az.Network</span><span class="sxs-lookup"><span data-stu-id="c5154-822">Az.Network</span></span>
* <span data-ttu-id="c5154-823">NetworkProfile 기능 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-823">Added NetworkProfile functionality.</span></span> <span data-ttu-id="c5154-824">추가된 새 cmdlet은 다음과 같습니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-824">new cmdlets added</span></span>
    - <span data-ttu-id="c5154-825">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c5154-825">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="c5154-826">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c5154-826">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="c5154-827">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c5154-827">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="c5154-828">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="c5154-828">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="c5154-829">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="c5154-829">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="c5154-830">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="c5154-830">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="c5154-831">서브넷 모델에 서비스 연결 링크 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-831">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="c5154-832">New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-832">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="c5154-833">Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig cmdlet 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-833">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="c5154-834">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="c5154-834">Az.RedisCache</span></span>
* <span data-ttu-id="c5154-835">모든 문자열을 Size 매개 변수로 진행되도록 허용</span><span class="sxs-lookup"><span data-stu-id="c5154-835">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="c5154-836">PSArgumentCompleter 팝업에 P5 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-836">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="c5154-837">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="c5154-837">Az.Resources</span></span>
* <span data-ttu-id="c5154-838">-Mode 매개 변수를 Set-AzPolicyDefinition에 추가</span><span class="sxs-lookup"><span data-stu-id="c5154-838">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="c5154-839">사용자가 포함된 Origin 작업에서 Get-AzProviderOperation commandlet 버그 수정</span><span class="sxs-lookup"><span data-stu-id="c5154-839">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="c5154-840">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="c5154-840">Az.Sql</span></span>
* <span data-ttu-id="c5154-841">일부 백업 cmdlet이 현재 azure 구독을 인식하지 않는 문제 해결</span><span class="sxs-lookup"><span data-stu-id="c5154-841">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="c5154-842">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="c5154-842">Az.Websites</span></span>
* <span data-ttu-id="c5154-843">새 cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - 컨테이너 지속적인 배포 Webhook URL을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-843">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="c5154-844">새 cmdlet New-AzWebAppContainerPSSession 및 Enter-WebAppContainerPSSession -  windows 컨테이너 앱에 PowerShell 원격 세션을 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="c5154-844">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="c5154-845">0.2.0 - 2018년 9월</span><span class="sxs-lookup"><span data-stu-id="c5154-845">0.2.0 - September 2018</span></span>
 <span data-ttu-id="c5154-846">최초 릴리스</span><span class="sxs-lookup"><span data-stu-id="c5154-846">Initial Release</span></span>