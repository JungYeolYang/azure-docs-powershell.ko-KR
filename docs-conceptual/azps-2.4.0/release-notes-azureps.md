---
ms.openlocfilehash: ac8513b3eee4adfcaf0be8bf7b4e8d09190811df
ms.sourcegitcommit: a4e527d3deba004007cfa22fa536e8255dd23b37
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 07/02/2019
ms.locfileid: "67516643"
---
## <a name="240---july-2019"></a>2.4.0 - 2019년 7월
#### <a name="azaccounts"></a>Az.Accounts
* 프로필 cmdlet에 대한 지원 추가
* 생성된 cmdlet에서 환경 및 데이터 평면에 대한 지원 추가
* Windows PowerShell의 데이터 평면 cmdlet에대해 일부 경우 잘못된 엔드포인트가 사용되는 버그 수정

#### <a name="azadvisor"></a>Az.Advisor
* Az.Advisor의 GA 릴리스
* 이 모듈은 이제 롤업 `Az` 모듈의 일부로 포함됩니다.

#### <a name="azapimanagement"></a>Az.ApiManagement
* 문제 https://github.com/Azure/azure-powershell/issues/8671 수정
    - **Get-AzApiManagementSubscription**
        - 사용자 및 제품별 구독을 쿼리하기 위한 지원이 추가됨
        - 범위 '/', '/ api, '/ api/echo api'를 사용하여 쿼리하기 위한 지원이 추가됨
* https://github.com/Azure/azure-powershell/issues/9307 및 https://github.com/Azure/azure-powershell/issues/8432 문제 수정
    - **Import-AzApiManagementApi**
        - Apis를 가져올 때 'ApiVersion' 및 'ApiVersionSetId'를 지정하기 위한 지원이 추가됨

#### <a name="azautomation"></a>Az.Automation
* 문자열 값을 처리하기 위해 Set-AzAutomationConnectionFieldValue cmdlet 버그를 수정했습니다.

#### <a name="azcompute"></a>Az.Compute
* New-AzImageConfig에 HyperVGeneration 매개 변수 추가

#### <a name="azdatafactory"></a>Az.DataFactory
* get activity runs, get pipeline runs, get trigger runs ADF cmdlet의 출력을 업데이트하여 Select-Object pipe를 지원합니다.

#### <a name="azeventgrid"></a>Az.EventGrid
* 'New-AzEventGridSubcription' 설명서의 오타 수정

#### <a name="aziothub"></a>Az.IotHub
* 권한 부여 정책 키를 다시 생성하기 위한 지원 추가

#### <a name="aznetwork"></a>Az.Network
* 'RoutingPreference'를 공용 IP 태그에 추가함
* 'Get-AzNetworkServiceTag' 참조 설명서의 예제 개선

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Get-AzPolicyState의 null 참조 문제 해결
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/9446 를 참조하세요.

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* Get-AzOperationalInsightsDataSource에 반환된 CustomLog datasource 모델 수정됨

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* IaaSVMs에 대한 get-policy 명령 수정

#### <a name="azresources"></a>Az.Resources
    - Get-AzPolicyState -Top 매개 변수에 대한 도움말 텍스트 수정
    - Get-AzPolicyAlias에 대한 클라이언트 쪽 페이징 지원 추가
    - Set-AzPolicyAssignment, -PolicyParameters 및 -PolicyParametersObject에 대한 새 매개 변수 추가
    - Policy cmdlet에 대한 몇 가지 문서 및 예제 업데이트

#### <a name="azservicebus"></a>Az.ServiceBus
* 문제 #4938 수정 - MaxSizeInMegabytes를 설정할 때 New-AzureRmServiceBusQueue가 BadRequest 반환

#### <a name="azsql"></a>Az.Sql
* 미리 보기 릴리스에서 공개 릴리스로 인스턴스 장애 조치(Failover) 그룹 cmdlet 추가
* 새 cmdlet으로 Azure SQL Server\Database Auditing을 지원하세요.
    - Set-AzSqlServerAudit
    - Get-AzSqlServerAudit
    - Remove-AzSqlServerAudit
    - Set-AzSqlDatabaseAudit
    - Get-AzSqlDatabaseAudit
    - Remove-AzSqlDatabaseAudit
* 취약성 평가 설정에서 이메일 제약 조건 제거

#### <a name="azstorage"></a>Az.Storage
* 다음 cmdlet에서 2개의 매개 변수 '-IndexDocument' 및 '-ErrorDocument404Path'를 필수에서 선택으로 변경하세요.
    -  Enable-AzStorageStaticWebsite
* 예제를 추가하여 Get-AzStorageBlobContent의 도움말 업데이트
* StorageException으로 cmdlet이 실패한 경우 자세한 오류 정보 표시
* Azure Files AAD DS 인증으로 스토리지 계정 생성 또는 업데이트 지원
    -  New-AzStorageAccount
    -  Set-AzStorageAccount
* 파일 공유, 파일 디렉터리 또는 파일의 목록 지원 또는 파일 핸들 닫기
    - Get-AzStorageFileHandle
    - Close-AzStorageFileHandle

#### <a name="azstoragesync"></a>Az.StorageSync
* 이 모듈은 이제 롤업 `Az` 모듈의 일부로 포함됩니다.

## <a name="232---june-2019"></a>2.3.2 - 2019년 6월
#### <a name="azaccounts"></a>Az.Accounts
* 함수 호출에 대해 일부 경우 잘못된 URL이 사용되는 버그 수정
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8983 를 참조하세요.
* AzureRM에서 Az cmdlet으로의 별칭 문제 해결
  - Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic
  - Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest

#### <a name="azcompute"></a>Az.Compute
* New-AzVm 및 New-AzVmss 단순 매개 변수 집합은 이제 'ProximityPlacementGroup'매개 변수를 허용합니다.
* 'New-AzVM' 참조 설명서에서 오타 수정

#### <a name="azdns"></a>Az.Dns
* 'Set-AzDnsZone' 도움말 예제의 오타가 수정되었습니다.

#### <a name="azeventgrid"></a>Az.EventGrid
* 2019-06-01 API 버전을 사용하도록 업데이트되었습니다.
* 새 cmdlet:
    - New-AzureRmEventGridDomain
        - 새 Azure Event Grid 도메인을 만듭니다.
    - Get-AzureRmEventGridDomain
        - Event Grid 도메인의 세부 정보를 가져오거나 현재 Azure 구독의 모든 Event Grid 도메인 목록을 가져옵니다.
    - Remove-AzureRmEventGridDomain
        - Azure Event Grid 도메인을 제거합니다.
    - New-AzureRmEventGridDomainKey
        - Azure Event Grid 도메인에 대한 공유 액세스 키를 다시 생성합니다.
    - Get-AzureRmEventGridDomainKey
        - Event Grid 도메인 이벤트를 게시하는 데 사용되는 공유 액세스 키를 가져옵니다.
    - New-AzureRmEventGridDomainTopic:
        - 새 Azure Event Grid 도메인 토픽을 만듭니다.
    - Get-AzureRmEventGridDomainTopic
        - Event Grid 도메인 토픽의 세부 사항을 가져오거나, 현재 Azure의 특정 Event Grid 도메인 아래의 모든 Event Grid 도메인 토픽 목록을 가져옵니다. 
    - Remove-AzureRmEventGridDomainTopic:
        - 기존 Azure Event Grid 도메인 토픽을 제거합니다.
* 다음 Cmdlet이 업데이트 되었습니다.
    - New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:
        - 새로운 Event Grid 도메인 및 Event Grid 도메인 토픽에 대한 파이핑을 지원하기 위해 새로운 필수 매개 변수를 추가하여 이러한 리소스 아래에 새 이벤트 구독을 만들 수 있습니다.
        - 새로운 Event Grid 도메인 이름 및 Event Grid 도메인 토픽 이름을 지정하기 위해 새로운 필수 매개 변수를 추가하여 이러한 리소스 아래에 새 이벤트 구독을 만들 수 있습니다.
        - 기존 매개 변수(예: EndPointType, SubjectBeginsWith 등)를 재사용할 수 있도록 도메인 및 도메인 토픽에 대한 새로운 매개 변수 집합을 추가합니다.
        - 지정을 위한 새로운 선택적 매개 변수를 추가
            - 이벤트 구독 만료 날짜,
            - 고급 필터링 매개 변수.
        - 대상으로 servicebusqueue에 대한 새 열거형을 추가합니다.
        - -IncludedEventType 옵션에서 'All' 사용을 허용하지 않고 다음으로 대체함 
    - Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:
        - 결과 페이지 매김 및 필터링을 지원하는 새로운 선택적 매개 변수(Top, ODataQuery 및 NextLink)를 추가합니다.
    - Remove-AzureRmEventGridSubscription
        - Event Grid 도메인 및 Event Grid 도메인 토픽에 대한 파이핑을 지원하기 위해 새로운 필수 매개 변수를 추가하여 이러한 리소스 아래에 기존 이벤트 구독을 제거할 수 있습니다.
        - Event Grid 도메인 이름 및 Event Grid 도메인 토픽 이름을 지정하기 위해 새로운 필수 매개 변수를 추가하여 이러한 리소스 아래에 기존 이벤트 구독을 제거할 수 있습니다.

#### <a name="azfrontdoor"></a>Az.FrontDoor
* New-AzFrontDoorWafMatchConditionObject
    - 변환 지원 및 새 연산자 자동 완성 값(RegEx)을 추가합니다.
* New-AzFrontDoorWafManagedRuleObject
    - 새 자동 완성 값 추가

#### <a name="aznetwork"></a>Az.Network
* Microsoft Azure Virtual Network 게이트웨이 리소스에 대한 지원 추가
    - 새 cmdlet
        - Get-AzVirtualNetworkGatewayVpnClientConnectionHealth
* AvailablePrivateEndpointType 추가
    - 새 cmdlet 
        - Get-AzAvailablePrivateEndpointType
* PrivatePrivateLinkService 추가
    - 새 cmdlet 
        - Get-AzPrivateLinkService 
        - New-AzPrivateLinkService
        - Remove-AzPrivateLinkService
        - New-AzPrivateLinkServiceIpConfig
        - Set-AzPrivateEndpointConnection
* PrivateEndpoint 추가
    - 새 cmdlet
        - Get-AzPrivateEndpoint
        - New-AzPrivateEndpoint
        - Remove-AzPrivateEndpoint
        - New-AzPrivateLinkServiceConnection
* 기능에 대한 새로운 명령이 업데이트됨: VpnConnection 상의 UseLocalAzureIpAddress 플래그
    - New-AzVpnConnection이 업데이트됨: 선택적 매개 변수 -UseLocalAzureIpAddress를 추가하여 로컬 Azure IP 주소가 연결을 시작하는 동안 소스 주소로 사용되어야 함을 나타냅니다.
    - Set-AzVpnConnection이 업데이트됨: 선택적 매개 변수 -UseLocalAzureIpAddress를 추가하여 로컬 Azure IP 주소가 연결을 시작하는 동안 소스 주소로 사용되어야 함을 나타냅니다.
* ExpressRoute 피어링에 읽기 전용 필드 PeeredConnections가 추가되었습니다.
* ExpressRoute에 읽기 전용 필드 GlobalReachEnabled가 추가되었습니다.
* ExpressRouteCircuit 모델에서 AllowGlobalReach 필드의 사용 중단을 부르는 호환성이 손상되는 변경 속성이 추가됨
* AzApplicationGatewayRedirectConfiguration cmdlet에서 TargetListenerID를 사용하는 중의 8756 오류 문제가 해결됨
* 다시 쓰기 규칙 세트가 설정되지 못하게 하는 New-AzApplicationGatewayPathRuleConfig의 버그를 수정했습니다.
* NetworkInterfaceIpConfiguration에 VirtualNetworkTaps가 표시되는 방식이 수정됨
* 모든 파트를 나열하도록 Cortex Get cmdlet이 수정됨
* ExpressRouteGateways, VpnGateway에 대한 VirtualHub 참조 생성 수정됨
* AzureFirewall 및 NatGateway의 가용성 영역에 대한 지원 추가됨
* Get-AzNetworkServiceTag cmdlet 추가됨
* Azure Firewall에 대한 여러 공용 IP 주소에 대한 지원 추가
    - New-AzFirewall cmdlet이 업데이트됨:
        - 하나 이상의 공용 IP 주소 개체를 허용하는 매개 변수 -PublicIpAddress 추가됨
        - Virtual Network 개체를 허용하는 매개 변수 -VirtualNetwork 추가됨
        - 방화벽 개체에 AddPublicIpAddress 및 RemovePublicIpAddress 메서드 추가됨 - 공용 IP 주소 개체를 입력으로 허용
        - 매개 변수 -PublicIpName 및 -VirtualNetworkName이 더 이상 사용되지 않음 
* 기능에 대한 새로운 명령이 업데이트됨: VpnClient AAD 인증 옵션을 가상 네트워크 게이트웨이 리소스로 설정했습니다. 
    - New-AzVirtualNetworkGateway가 업데이트됨: 게이트웨이에서 VpnClient AAD 인증 옵션을 설정할 수 있도록 선택적 매개 변수 AadTenantUri, AadAudienceId, AadIssuerUri가 추가되었습니다.
    - Set-AzVirtualNetworkGateway가 업데이트됨: 게이트웨이에서 VpnClient AAD 인증 옵션을 설정할 수 있도록 선택적 매개 변수 AadTenantUri, AadAudienceId, AadIssuerUri가 추가되었습니다.
    - Set-AzVirtualNetworkGateway가 업데이트됨: 게이트웨이에서 VpnClient AAD 인증 옵션을 제거할 수 있도록 선택적인 스위치 매개 변수 RemoveAadAuthentication이 추가되었습니다.

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* 'New-AzureRmOperationalInsightsWorkspace' 명령에서 **pergb2018** 가격 책정 계층 사용

#### <a name="azresources"></a>Az.Resources
* 추가 템플릿 내보내기 옵션 지원
    - Export-AzResourceGroup에 '-SkipResourceNameParameterization' 매개 변수 추가
    - Export-AzResourceGroup에 '-SkipAllParameterization' 매개 변수 추가
    - 내보낸 리소스 필터링을 위해 Export-AzResourceGroup에 '-Resource' 매개 변수 추가

#### <a name="azservicefabric"></a>Az.ServiceFabric
* 일부 경우 잘못된 지문을 가져오는 추가 인증서 ByExistingKeyVault 수정

#### <a name="azsql"></a>Az.Sql
* Advanced Threat Protection 스토리지 엔드포인트 접미사 수정
* Advanced Data Security가 Advanced Threat Protection 정책을 재정의하는 것을 수정
* 고객이 TDE 키를 추가하고 관리되는 인스턴스에 TDE 보호기를 설정할 수 있도록 Management.Sql용 새 Cmdlet 추가
   - Add-AzSqlInstanceKeyVaultKey
   - Get-AzSqlInstanceKeyVaultKey
   - Remove-AzSqlInstanceKeyVaultKey
   - Get-AzSqlInstanceTransparentDataEncryptionProtector
   - Set-AzSqlInstanceTransparentDataEncryptionProtector

#### <a name="azstorage"></a>Az.Storage
* 스토리지 계정 생성 시 종류 FileStorage 및 SkuName Premium_ZRS 지원
    - New-AzStorageAccount
* BLOB immutability cmdlet의 설명 명확화
    -  Remove-AzRmStorageContainerImmutabilityPolicy

#### <a name="azwebsites"></a>Az.Websites
* Get-AzWebAppCertificate를 클라이언트 대신 서버의 리소스 그룹별로 필터링하도록 최적화
* Get-AzWebAppSnapshot에 -UseDisasterRecovery 스위치 매개 변수 추가

## <a name="220---june-2019"></a>2.2.0 - 2019년 6월
#### <a name="azcdn"></a>Az.Cdn
* cmdlet에서 2019-04-15 API 버전 기반의 rulesEngine 기능을 지원하도록 업데이트되었습니다.

#### <a name="azcompute"></a>Az.Compute
* 작업을 시작하여 완료되기 전에 즉시 반환하는 `NoWait` 매개 변수가 추가되었습니다.
    - 다음 Cmdlet이 업데이트 되었습니다.   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM

#### <a name="azeventhub"></a>Az.EventHub
* #9231 수정 - Get-AzEventHubNamespace에서 태그를 반환하지 않음
* #9230 수정 - Get-AzEventHubNamespace에서 ResourceGroupName 대신 ResourceGroup을 반환함

#### <a name="aznetwork"></a>Az.Network
* Nat Gateway에 대한 ResourceId 및 InputObject 업데이트
    - ResourceId 및 InputObject에 대한 별칭 추가

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Get-AzPolicyEvent에서 Null 참조 문제 해결

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* IaaSVM 정책 최소 보존 기간(일)이 1에서 7로 변경됨

#### <a name="azservicebus"></a>Az.ServiceBus
* #9182 문제 해결 - Get-AzServiceBusNamespace에서 ResourceGroupName 대신 ResourceGroup을 반환

#### <a name="azservicefabric"></a>Az.ServiceFabric
* 'Update-AzServiceFabricReliability' 오류 메시지의 오타 수정
* Service Fabric 명령줄에서 누락된 문자 수정

#### <a name="azsql"></a>Az.Sql
* Managed Instance에 대한 AutoDr을 지원하기 위해 New-AzureSqlInstance cmdlet에 대한 DnsZonePartner 매개 변수를 추가합니다.
* Get-AzSqlDatabaseSecureConnectionPolicy cmdlet 사용 중단
* Threat Detection(위협 탐지) cmdlet 이름을 Advanced Threat Protection으로 변경함
* 새 AzSqlInstance -StorageSizeInGB 및 -LicenseType 매개 변수는 이제 선택 사항입니다.

#### <a name="azwebsites"></a>Az.Websites
* -WebApp 속성에서 Set-AzWebApp 및 Set-AzWebAppSlot을 사용하면 태그가 제거되는 문제를 해결함

## <a name="210---may-2019"></a>2.1.0 - 2019년 5월
#### <a name="azapimanagement"></a>Az.ApiManagement
* 글로벌 및 API 범위에서 진단을 관리하기 위한 새 cmdlet을 만들었습니다.
    - **Get-AzApiManagementDiagnostic** - 글로벌 또는 API 범위가 구성된 진단 가져오기
    - **New-AzApiManagementDiagnostic** - 글로벌 범위 또는 API 범위에서 새 진단 만들기
    - **New-AzApiManagementHttpMessageDiagnostic** - 기록할 Headers(헤더) 및 Body Bytes(본문 바이트 수) 크기에 대한 진단 설정 만들기
    - **New-AzApiManagementPipelineDiagnosticSetting** - 게이트웨이로 들어오고 나가는 HTTP 메시지에 대한 진단 설정 만들기
    - **New-AzApiManagementSamplingSetting** - 진단 요청/응답에 대한 샘플링 설정 만들기
    - **Remove-AzApiManagementDiagnostic** - 글로벌 또는 API 범위에서 진단 엔터티 제거
    - **Set-AzApiManagementDiagnostic** - 글로벌 또는 API 범위에서 진단 엔터티 업데이트
* ApiManagement 서비스에서 캐시를 관리하기 위한 새 cmdlet을 만들었습니다.
    - **Get-AzApiManagementCache** - 식별자 또는 모든 캐시로 지정된 캐시의 세부 정보 가져오기
    - **New-AzApiManagementCache** - 특정 Azure 'region'(지역)에 새 'default'(기본) 캐시 만들기
    - **Remove-AzApiManagementCache** - 캐시 제거
    - **Update-AzApiManagementCache** - 캐시 업데이트
* API 스키마 관리하기 위한 새 cmdlet을 만들었습니다.
    - **New-AzApiManagementSchema** - API에 대한 새 스키마 만들기
    - **Get-AzApiManagementSchema** - API에 구성된 스키마 가져오기
    - **Remove-AzApiManagementSchema** - API에 구성된 스키마 제거
    - **Set-AzApiManagementSchema** - API에 구성된 스키마 업데이트
* 사용자 토큰을 생성하기 위한 새 cmdlet을 만들었습니다. 
    - **New-AzApiManagementUserToken** - 기본적으로 8시간 동안 유효한 새 사용자 토큰을 생성합니다. 'GIT' 사용자에 대한 토큰은 이 cmdlet을 사용하여 생성할 수 있습니다.
* 네트워크 상태를 검색하기 위한 새 cmdlet을 만들었습니다.
    - **Get-AzApiManagementNetworkStatus** - API Management 서비스에서 사용하는 리소스의 네트워크 상태 연결을 가져옵니다. ApiManagement 서비스를 가상 네트워크에 배포하고 종속성이 손상되었는지 여부를 확인할 때 유용합니다.
* **New-AzApiManagement** cmdlet에서 ApiManagement 서비스를 관리하도록 업데이트했습니다. 
    - 새 '소비' SKU 지원이 추가됨
    - '소비' SKU에 대해 'EnableClientCertificate' 플래그를 설정하기 위한 지원이 추가됨
    - 새 **New-AzApiManagementSslSetting** cmdlet을 사용하면 'Backend(백 엔드)' 및 'Frontend'(프런트 엔드)에서 'TLS/SSL' 설정을 구성할 수 있습니다. 또한 ApiManagement 서비스의 'Frontend'에서 '3DES'와 같은 'Ciphers'와 'Http2'와 같은 'ServerProtocols'를 구성하는 데 사용할 수 있습니다.
    - ApiManagement 서비스에서 'DeveloperPortal' 호스트 이름을 구성하기 위한 지원이 추가됨
* **Get-AzApiManagementSsoToken** cmdlet에서 'PsApiManagement' 개체를 입력으로 사용하도록 업데이트했습니다.
* cmdlet에서 오류 메시지를 인라인으로 표시하도록 업데이트했습니다. 
     > PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : 오류 코드: ValidationError 오류 메시지: 하나 이상의 필드에 잘못된 값이 있습니다. 오류 세부 정보:    [Code=ValidationError, Message=줄 3, 열 10의 'log-to-eventhub' 요소에 오류가 있습니다.: 로거를 찾지 못함, Target=log-to-eventhub]
* **Export-AzApiManagementApi** cmdlet에서 API를 'OpenApi 3.0' 형식으로 내보내도록 업데이트했습니다.
* **Import-AzApiManagementApi** cmdlet을 업데이트했습니다.
    - 'OpenApi 3.0' 문서 사양에서 API 가져오기
    - 문서('Swagger', 'Wadl', 'Wsdl', 'OpenApi')에 지정된 'PsApiManagementSchema' 속성 재정의
    - 문서에 지정된 'ServiceUrl' 속성 재정의
* **Get-AzApiManagementPolicy** cmdlet에서 'rawxml'을 사용하여 이스케이프된 비 Xml 'format'(형식)의 정책을 반환하도록 업데이트했습니다.
* **Set-AzApiManagementPolicy** cmdlet에서 'rawxml'을 사용하여 이스케이프된 비 Xml 'format'의 정책을 수락하고, 'xml'을 사용하여 이스케이프된 Xml 'format'의 정책을 수락하도록 업데이트했습니다.
* **New-AzApiManagementApi** cmdlet을 업데이트했습니다. 
    - 'OpenId' 권한 부여 서버를 사용하여 API 구성
    - 'ApiVersionSet'에서 API 만들기
    - 'SourceApiId' 및 'SourceApiRevision'을 사용하여 API 복제
    - API 범위에서 'SubscriptionRequired' 구성 가능 
* **Set-AzApiManagementApi** cmdlet을 업데이트했습니다.
    - 'OpenId' 권한 부여 서버를 사용하여 API 구성
    - API를 'ApiVersionSet'으로 업데이트    
    - API 범위에서 'SubscriptionRequired' 구성 가능 
* **New-AzApiManagementRevision** cmdlet을 업데이트했습니다.
    - 'SourceApiRevision'을 사용하여 기존 수정 버전 복제(태그, 제품, 작업 및 정책 복사). 새 수정 버전은 부모의 'ApiId'를 가정합니다.
    - 'ApiRevisionDescription' 제공
    - API 복제 시 'ServiceUrl' 재정의
* **New-AzApiManagementIdentityProvider** cmdlet을 업데이트했습니다.
    - 'Authority'를 사용하여 'AAD' 또는 'AADB2C' 구성
    - 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' 및 'PasswordResetPolicy' 설정
* **New-AzApiManagementSubscription** cmdlet을 업데이트했습니다.
    - 'Scope' 및 'UserId'를 사용하여 새 SubscriptonModel 설명
    - 'ProductId' 및 'UserId'를 사용하여 이전 구독 모델 설명
    - 구독 수준에서 'AllowTracing'을 사용하도록 설정하는 지원 추가
* **Set-AzApiManagementSubscription** cmdlet을 업데이트했습니다.
    - 'Scope' 및 'UserId'를 사용하여 새 SubscriptonModel 설명
    - 'ProductId' 및 'UserId'를 사용하여 이전 구독 모델 설명
    - 구독 수준에서 'AllowTracing'을 사용하도록 설정하는 지원 추가
* 다음 cmdlet에서 'ResourceId'를 입력으로 수락하도록 업데이트했습니다
    - 'New-AzApiManagementContext'
        > New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso
    - 'Get-AzApiManagementApiRelease'
        > Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId
    - 'Get-AzApiManagementApiVersionSet'
        > Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset
    - 'Get-AzApiManagementAuthorizationServer'
    - 'Get-AzApiManagementBackend'
        > Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric
    - 'Get-AzApiManagementCertificate' 
    - 'Remove-AzApiManagementApiVersionSet'
    - 'Remove-AzApiManagementSubscription'

#### <a name="azautomation"></a>Az.Automation
* Get-AzAutomationJobOutputRecord에서 JSON 및 Text 레코드 값을 처리하도록 업데이트했습니다.
    - 문제 https://github.com/Azure/azure-powershell/issues/7977 수정
    - 문제 https://github.com/Azure/azure-powershell/issues/8600 수정
* Start-AzAutomationDscCompilationJob에서 완료될 때까지 기다리지 않고 작업을 바로 시작하도록 변경했습니다.
    * 문제 https://github.com/Azure/azure-powershell/issues/8347 수정
* -Name을 사용하면 모든 노드를 반환하는 Get-AzAutomationDscNode 수정. 이제 일치하는 노드만 반환합니다.

#### <a name="azcompute"></a>Az.Compute
* ProtectFromScaleIn 및 ProtectFromScaleSetAction 매개 변수를 Update-AzVmssVM cmdlet에 추가합니다.
* 'East US'(미국 동부)가 지원되지 않는 경우 이제 New-AzVM wimple 매개 변수 집합에서 기본적으로 사용 가능한 위치를 사용합니다.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* ADLS SDK에서 httpclient를 사용하도록 업데이트하고, 데이터 평면 테스트를 Azure 프레임워크와 통합합니다.

#### <a name="azmonitor"></a>Az.Monitor
* 도움말 예제에서 잘못된 매개 변수 이름을 수정했습니다.

#### <a name="aznetwork"></a>Az.Network
* DisableBgpRoutePropagation 플래그를 유효 경로 테이블 출력에 추가합니다.
    - 업데이트된 cmdlet:
        - Get-AzEffectiveRouteTable
* New-AzApplicationGatewayTrustedRootCertificate 설명서에서 이중 파선을 수정합니다.

#### <a name="azresources"></a>Az.Resources
* 할당 거부를 검색하기 위한 새 Get-AzureRmDenyAssignment cmdlet을 추가합니다.

#### <a name="azsql"></a>Az.Sql
* Advanced Threat Protection cmdlet의 이름을 Advanced Data Security로 변경하고, 취약성 평가를 기본적으로 사용하도록 설정합니다.

## <a name="200---may-2019"></a>2.0.0 - 2019년 5월
#### <a name="azaccounts"></a>Az.Accounts
* 사용자 이름/비밀번호 인증을 사용하여 ADFS 문제를 해결하도록 인증 라이브러리 업데이트

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Bing Search 서비스에 대해서만 Bing 면책 조항을 표시하세요.
* 계정 생성 실패 시 오류 개선.

#### <a name="azcompute"></a>Az.Compute
* 근접 배치 그룹 기능
    - 다음과 같은 새 cmdlet을 추가했습니다.   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup
    - 새 매개 변수 ProximityPlacementGroupId가 다음 cmdlet에 추가됩니다.   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig
* New-AzGalleryImageVersion에 StorageAccountType 매개 변수가 추가됩니다.
* New-AzGalleryImageVersion의 TargetRegion이 StorageAccountType를 포함할 수 있습니다.
* SkipShutdown 스위치 매개 변수가 Stop-AzVM 및 Stop-AzVmss에 추가되었습니다.       
* 주요 변경 내용
    - Set-AzVMBootDiagnostics이 Set-AzVMBootDiagnostic으로 변경됩니다.
    - Export-AzLogAnalyticThrottledRequests이 Export-AzLogAnalyticThrottledRequests로 변경되었습니다.

#### <a name="azdeploymentmanager"></a>Az.DeploymentManager
* Azure 배포 관리자 cmdlet의 일반적으로 사용 가능한 첫 번째 릴리스

#### <a name="azdns"></a>Az.Dns
* 자동 DNS 이름 서버 위임
    - DNS 영역 만들기 cmdlet은 추가 선택적 매개 변수로 부모 영역 이름을 허용합니다.
    - 새로 생성 된 자식 영역의 부모 영역에 NS 레코드를 추가합니다.

#### <a name="azfrontdoor"></a>Az.FrontDoor
* Azure FrontDoor cmdlet의 일반적으로 사용 가능한 첫 번째 릴리스
* 'Waf'를 포함하도록 WAF cmdlet의 이름 바꾸기
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a>Az.HDInsight
* 두 개의 cmdlet을 제거합니다.
    - Grant-AzHDInsightHttpServicesAccess
    - Revoke-AzHDInsightHttpServicesAccess
* Grant-AzHDInsightHttpServicesAccess를 대체할 새 cmdlet Set-AzHDInsightGatewayCredential을 추가했습니다.
* reader 역할과 HDInsight 운영자 역할을 구분하도록 cmdlet Get-AzHDInsightJobOutput 업데이트:
    - reader 역할을 가진 사용자는 'DefaultStorageAccountKey'매개 변수를 명시적으로 지정해야 합니다. 그렇지 않으면 오류가 발생합니다.
    - Hdinsight 운영자 역할을 가진 사용자를 영향을 받지 않습니다.

#### <a name="azmonitor"></a>Az.Monitor
* SQR API(예약 쿼리 규칙)용 새 cmdlet  
    - New-AzScheduledQueryRuleAlertingAction
    - New-AzScheduledQueryRuleAznsActionGroup
    - New-AzScheduledQueryRuleLogMetricTrigger
    - New-AzScheduledQueryRuleSchedule
    - New-AzScheduledQueryRuleSource
    - New-AzScheduledQueryRuleTriggerCondition
    - New-AzScheduledQueryRule
    - Get-AzScheduledQueryRule
    - Set-AzScheduledQueryRule
    - Update-AzScheduledQueryRule
    - Remove-AzScheduledQueryRule
    - SQR API에 대한 [자세한 내용](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules)
    - GenV2(비 클래식) 메트릭 기반 경고 규칙에 대한 cmdlet을 포함하도록 Az.Monitor.md가 업데이트됨

#### <a name="aznetwork"></a>Az.Network
* Nat 게이트웨이 리소스에 대한 지원 추가
    - 새 cmdlet
        - New-AzNatGateway
        - Get-AzNatGateway
        - Set-AzNatGateway
        - Remove-AzNatGateway
   - 다음 Cmdlet이 업데이트 되었습니다.
        - New-AzureVirtualNetworkSubnetConfigCommand
        - Add-AzureVirtualNetworkSubnetConfigCommand
* 기능에 대한 새로운 명령이 업데이트됨: Brooklyn Gateway에서 사용자 지정 경로 설정/제거.
    - New-AzVirtualNetworkGateway가 업데이트됨: 선택적 매개 변수 -CustomRoute를 추가하여 게이트웨이에서 설정할 사용자 지정 경로로 주소 접두사를 설정합니다.
    - Set-AzVirtualNetworkGateway가 업데이트됨: 선택적 매개 변수 -CustomRoute를 추가하여 게이트웨이에서 설정할 사용자 지정 경로로 주소 접두사를 설정합니다.

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* 정책 평가 세부 정보 쿼리 지원
    - Get-AzPolicyState에 '-Expand'매개 변수 추가 '-Expand PolicyEvaluationDetails' 지원

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* 크로스 구독 Azure에서 Azure 사이트 복구 지원
* Azure Site Recovery에 대한 호환성이 손상되는 변경 표시
* Azure Site Recovery 복구 계획 최종 실행 계획에 대한 수정
* Azure에서 Azure에 대한 Azure Site Recovery 업데이트 네트워크 매핑 수정
* 관리 디스크에 대한 Azure에서 Azure에 대한 Azure Site Recovery 업데이트 보호 방향 수정
* 기타 사소한 수정.

#### <a name="azrelay"></a>Az.Relay
* 고객 관련 메시지의 철자 오류 수정

#### <a name="azservicebus"></a>Az.ServiceBus
* 네임스페이스의 NetworkRuleSet에 대한 새 cmdlet가 추가되었습니다

#### <a name="azstorage"></a>Az.Storage
* 저장소 클라이언트 라이브러리 10.0.1로 업그레이드(이 SDK의 모든 개체의 네임스페이스가 'Microsoft.WindowsAzure.Storage. *'에서 'Microsoft.Azure.Storage.* '로 변경됨)
* 새로운 API 버전 2019-04-01을 지원하기 위해 Microsoft.Azure.Management.Storage 11.0.0으로 업그레이드합니다.
* 스토리지 생성 계정의 기본 스토리지 계정 종류가 'Storage'에서 'StorageV2'로 변경됩니다.
    - New-AzStorageAccount
* 'StandardLRS'가 'Standard_LRS'로 변경되는 것과 같이 '-'을 추가하여 입력 SkuName과 정렬되도록 스토리지 계정 cmdlet 출력 Sku.Name을 변경합니다.
    - New-AzStorageAccount
    - Get-AzStorageAccount
    - Set-AzStorageAccount

#### <a name="azwebsites"></a>Az.Websites
* Get-AzWebApp에서 반환한 PSSite 개체에 대해 'Kind'속성이 설정됩니다.
* Get-AzWebApp* 메트릭 및 Get-AzAppServicePlanMetrics가 사용되지 않음으로 표시되었습니다.

## <a name="180---april-2019"></a>1.8.0 - 2019년 4월
### <a name="highlights-since-the-last-major-release"></a>마지막 주 릴리스 이후의 주요 사항
* `Az` 모듈 일반 공급
* `Az` 모듈에 대한 자세한 내용은 https://aka.ms/azps-announce 를 방문하세요.
* Location, ResourceGroup 및 ResourceName 완성자가 추가되었습니다(https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/ ).
* 와일드카드 지원이 Az.Compute 및 Az.Network에 대한 Get cmdlet에 추가되었습니다.
* Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증이 추가되었습니다.
* Python 2 Runbook 지원이 Az.Automation에 추가되었습니다.
* Az.LogicApp: 통합 계정 어셈블리 및 일괄 처리 구성을 위한 새로운 cmdlet입니다.

#### <a name="azaccounts"></a>Az.Accounts
* Mac에서 모듈을 올바르게 삭제하기 위해 Uninstall-AzureRm을 업데이트합니다.

#### <a name="azbatch"></a>Az.Batch
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azcdn"></a>Az.Cdn
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azcompute"></a>Az.Compute
* 디스크의 리소스 ID에 리소스 ID의 소문자 resourcegroups가 있는 경우 AEM 설치 문제 수정
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.
* 와일드 카드에 대한 설명서 수정

#### <a name="azdatafactory"></a>Az.DataFactory
* NodeCount가 관리형 통합 런타임에 대해 Null이 아닌 경우 SsisProperties를 추가합니다.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azeventgrid"></a>Az.EventGrid
* 이벤트 구독 cmdlet 만들기/업데이트를 사용하기 전에 리소스를 만들어야 함을 나타내기 위해 엔드포인트의 도움말 텍스트가 업데이트되었습니다.

#### <a name="azeventhub"></a>Az.EventHub
* 네임스페이스의 NetworkRuleSet에 대한 새 cmdlet가 추가되었습니다 

#### <a name="azhdinsight"></a>Az.HDInsight
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="aziothub"></a>Az.IotHub
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azkeyvault"></a>Az.KeyVault
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.
* 와일드 카드에 대한 설명서 수정

#### <a name="azmachinelearning"></a>Az.MachineLearning
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azmedia"></a>Az.Media
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azmonitor"></a>Az.Monitor
  * GenV2(비 클래식) 메트릭 기반 경고 규칙에 대한 새 cmdlet
      - New-AzMetricAlertRuleV2DimensionSelection
      - New-AzMetricAlertRuleV2Criteria
      - Remove-AzMetricAlertRuleV2
      - Get-AzMetricAlertRuleV2
      - Add-AzMetricAlertRuleV2
  * 모니터 SDK가 버전 0.22.0-preview로 업데이트되었습니다.

#### <a name="aznetwork"></a>Az.Network
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.
* 와일드 카드에 대한 설명서 수정

#### <a name="aznotificationhubs"></a>Az.NotificationHubs
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azpowerbiembedded"></a>Az.PowerBIEmbedded
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.
* Azure VM의 SQL용 테이블 형식이 업데이트되었습니다.
* AzureFileShare에서 위치를 가져오는 대체 메서드가 추가되었습니다.
* 시간대에 따라 SchedulePolicy 개체의 ScheduleRunDays가 업데이트되었습니다.

#### <a name="azrediscache"></a>Az.RedisCache
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.

#### <a name="azresources"></a>Az.Resources
* 와일드 카드에 대한 설명서 수정

#### <a name="azsql"></a>Az.Sql
* Monitor SDK의 종속성을 공용 코드로 바꿉니다.
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.
* 다중 열 분류 프로세스가 향상되었습니다.
* 기본적으로 Get-AzSqlServerServiceObjective의 응답으로 SKU 속성(SKU 이름, 제품군, 용량)과 테이블 형식을 포함합니다.
* 해당 지역에 기존 서버 없이 위치별로 Get-AzSqlServerServiceObjective를 가져올 수 있습니다.
* 관리형 인스턴스 생성 시 표준 시간대 매개 변수를 지원합니다.
* 와일드 카드에 대한 설명서 수정

#### <a name="azwebsites"></a>Az.Websites
* 실행 시 태그를 제거하지 않도록 Set-AzWebApp 및 Set-AzWebAppSlot를 수정합니다.
* 복수 명사의 cmdlet가 단수로 업데이트되었고, 복수 이름이 사용되지 않았습니다.
* WebSites SDK가 업데이트되었습니다.
* PSAppServicePlan에서 AdminSiteName 속성을 제거했습니다.

## <a name="170---april-2019"></a>1.7.0 - 2019년 4월
### <a name="highlights-since-the-last-major-release"></a>마지막 주 릴리스 이후의 주요 사항
* `Az` 모듈 일반 공급
* `Az` 모듈에 대한 자세한 내용은 https://aka.ms/azps-announce 를 방문하세요.
* Location, ResourceGroup 및 ResourceName 완성자가 추가되었습니다(https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/ ).
* 와일드카드 지원이 Az.Compute 및 Az.Network에 대한 Get cmdlet에 추가되었습니다.
* Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증이 추가되었습니다.
* Python 2 Runbook 지원이 Az.Automation에 추가되었습니다.
* Az.LogicApp: 통합 계정 어셈블리 및 일괄 처리 구성을 위한 새로운 cmdlet입니다.

#### <a name="azaccounts"></a>Az.Accounts
* 매개 변수 AzureAnalysisServicesEndpointResourceId를 허용하도록 Add-AzEnvironment 및 Set-AzEnvironment 업데이트

#### <a name="azanalysisservices"></a>Az.AnalysisServices
* 데이터 평면 cmdlet에서 ServiceClient 사용 및 원본 인증 논리 제거
* 호환성이 손상되는 변경을 방지하기 위해 Add-AzureASAccount를 Connect-AzAccount의 래퍼로 만듦

#### <a name="azautomation"></a>Az.Automation
* 포함에 대한 New-AzAutomationSoftwareUpdateConfiguration cmdlet 버그 수정 이제 매개 변수 IncludedKbNumber 및 IncludedPackageNameMask가 작동함
* Azure 자동화 업데이트 관리 동적 그룹에 대한 버그 수정

#### <a name="azcompute"></a>Az.Compute
* New-AzDiskConfig 및 New-AzSnapshotConfig에 HyperVGeneration 매개 변수 추가
* 다른 테넌트의 갤러리 이미지를 사용하여 VM을 만들 수 있음 

#### <a name="azcontainerinstance"></a>Az.ContainerInstance
* 후행 빈 인수를 추가한 New-AzContainerGroup의 -Command 매개 변수의 문제 수정

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF .Net SDK 버전을 3.0.2로 업데이트
* RepoConfiguration 관련 설정에 대한 추가 매개 변수로 Set-AzDataFactoryV2 cmdlet을 업데이트

#### <a name="azresources"></a>Az.Resources
* '-ResourceId' 또는 '-ResourceGroupName', '-Name' 및 '-ResourceType' 매개 변수를 제공할 때 'Get-AzResource'에 대한 공급자 처리 개선
* 'Test-AzDeployment' 및 'Test-AzResourceGroupDeployment'에 대한 오류 처리 개선
    - 배포 유효성 검사 외부에서 발생한 오류를 처리하고 그 대신 명령의 출력에 포함
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/6856 를 참조하세요.
* 배포 cmdlet 세트에 스크립트 및 작업 시나리오에서 프롬프트를 건너뛰는 '-IgnoreDynamicParameters' 스위치 추가
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/6856 를 참조하세요.

#### <a name="azsql"></a>Az.Sql
* 데이터베이스 데이터 분류 지원

#### <a name="azstorage"></a>Az.Storage
* 매개 변수 -UseConnectedAccount를 사용하여 스토리지 컨텍스트를 만들 때 자세한 오류 보고(단, 로그인 Azure 계정 없이)
    - New-AzStorageContext
* 관리 평면 API를 사용하여 지정한 스토리지 계정의 BLOB 서비스 속성 관리 지원
    - Update-AzStorageBlobServiceProperty
    - Get-AzStorageBlobServiceProperty
    - Enable-AzStorageBlobDeleteRetentionPolicy
    - Disable-AzStorageBlobDeleteRetentionPolicy
* BLOB 및 파일 업로드/다운로드 cmdlet에 대한 -AsJob 지원
    - Get-AzStorageBlobContent
    - Set-AzStorageBlobContent
    - Get-AzStorageFileContent
    - Set-AzStorageFileContent

## <a name="160---march-2019"></a>1.6.0 - 2019년 3월
### <a name="highlights-since-the-last-major-release"></a>마지막 주 릴리스 이후의 주요 사항
* `Az` 모듈 일반 공급
* `Az` 모듈에 대한 자세한 내용은 https://aka.ms/azps-announce 를 방문하세요.
* Location, ResourceGroup 및 ResourceName 완성자가 추가되었습니다(https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/ ).
* 와일드카드 지원이 Az.Compute 및 Az.Network에 대한 Get cmdlet에 추가되었습니다.
* Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증이 추가되었습니다.
* Python 2 Runbook 지원이 Az.Automation에 추가되었습니다.
* Az.LogicApp: 통합 계정 어셈블리 및 일괄 처리 구성을 위한 새로운 cmdlet입니다.

#### <a name="azautomation"></a>Az.Automation
* Azure 자동화 업데이트 관리에서 변경된 지원 기능은 다음과 같습니다.
    * 동적 그룹화
    * 사전 스크립트
    * 다시 부팅 설정

#### <a name="azcompute"></a>Az.Compute
* Get-AzVmBootDiagnosticsData의 경로 확인 문제가 해결되었습니다.
* Compute 클라이언트 라이브러리가 25.0.0으로 업데이트되었습니다.

#### <a name="azkeyvault"></a>Az.KeyVault
* 와일드카드 지원이 KeyVault cmdlet에 추가되었습니다.

#### <a name="aznetwork"></a>Az.Network
* Azure Firewall에 대한 위협 인텔리전스 지원이 추가되었습니다.
* Application Gateway 방화벽 정책의 최상위 수준 리소스 및 사용자 지정 규칙이 추가되었습니다.

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* 인스턴트 RP를 지원하기 위해 SnapshotRetentionInDays가 Azure VM 정책에 추가되었습니다.
* 컨테이너 등록을 취소하는 파이프 지원이 추가되었습니다.

#### <a name="azresources"></a>Az.Resources
* Get-AzResource 및 Get-AzResourceGroup에 대한 와일드카드 지원을 업데이트합니다.
* ARM에 대한 일반 호출을 수행할 때 사용되는 자격 증명을 업데이트합니다.

#### <a name="azsql"></a>Az.Sql
* 위협 탐지의 cmdlet 매개 변수(ExcludeDetectionType)가 DetectionType에서 string[]으로 변경되어 새 DetectionType이 추가되면 이후의 증명이 되고 자동 완성도 지원합니다.

#### <a name="azstorage"></a>Az.Storage
* 스토리지 계정에 대한 관리 정책 가져오기/설정/제거를 지원합니다.
    - Set-AzStorageAccountManagementPolicy
    - Get-AzStorageAccountManagementPolicy
    - Remove-AzStorageAccountManagementPolicy
    - Add-AzStorageAccountManagementPolicyAction
    - New-AzStorageAccountManagementPolicyFilter
    - New-AzStorageAccountManagementPolicyRule

#### <a name="azwebsites"></a>Az.Websites
* 'New-AzWebApp -IncludeSourceWebAppSlots'를 사용하여 모든 슬롯의 복제를 중단하는 ARM 템플릿 버그가 수정되었습니다. 

## <a name="150---march-2019"></a>1.5.0 - 2019년 3월
#### <a name="azaccounts"></a>Az.Accounts
* 'Register-AzModule' 명령을 추가하여 AutoRest 생성 cmdlet을 지원
* Connect-AzAccount 예제 업데이트

#### <a name="azautomation"></a>Az.Automation
* 몇몇 Azure Automation cmdlet에서 특정 월별 일정을 검색할 때 발생하는 문제 수정
* 상위 20개 노드를 반환하도록 Get-AzAutomationDscNode를 수정합니다. 이제 모든 노드 반환

#### <a name="azcdn"></a>Az.Cdn
* 사용자 지정 도메인 Https 사용/사용 안 함에 대한 새 Powershell cmdlet이 추가되었으며 기존의 것은 사용되지 않았습니다.

#### <a name="azcompute"></a>Az.Compute
* Get cmdlet에 와일드 카드 지원 추가

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF.Net SDK 버전이 3.0.1로 업데이트되었습니다.

#### <a name="azlogicapp"></a>Az.LogicApp
* 첫 결과 페이지 검색 시에만 ListWorkflows 수정

#### <a name="aznetwork"></a>Az.Network
* Network cmdlet에 와일드 카드 지원 추가

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Azure VM 지원에 SQL 서버가 추가되었습니다.
* SDK 업데이트
* VMappContainer 체크 인 Get-ProtectableItem 제거
* Get ProtectableItem의 매개 변수로 Name과 ServerName이 추가되었습니다.

#### <a name="azresources"></a>Az.Resources
* `-TemplateObject` 매개 변수를 추가하여 cmdlet을 배포
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/2933 를 참조하세요.
* `Get-AzResource`의 결과를 `Set-AzResource`(으)로 파이프할 때 발생하는 문제 수정
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8240 를 참조하세요.
* 실행 시 JSON 데이터 형식 문제 해결 `Set-AzResource`
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7930 를 참조하세요.

#### <a name="azsql"></a>Az.Sql
* AuditingEndpointsCommunicator를 업데이트 합니다.
    - 새 진단 설정을 생성할 때 에지 사례의 동작을 수정합니다.

#### <a name="azstorage"></a>Az.Storage
* 스토리지 계정      - New-AzStorageAccount를 생성할 때 종류 BlockBlobStorage를 지원

## <a name="140---february-2019"></a>1.4.0 - 2019년 2월
#### <a name="azanalysisservices"></a>Az.AnalysisServices
* 사용되지 않는 AddAzureASAccount cmdlet

#### <a name="azautomation"></a>Az.Automation
* Import-AzAutomationDscNodeConfiguration 도움말 업데이트
* Import-AzAutomationDscConfiguration cmdlet 구성 이름 유효성 검사 추가
* Import-AzAutomationDscConfiguration cmdlet 오류 처리 개선

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* 리소스의 하위 도메인을 지정하는 데 사용되는 New-AzCognitiveServicesAccount에 대한 새 선택적 매개 변수로 CustomSubdomainName이 추가되었습니다.

#### <a name="azcompute"></a>Az.Compute
* ID 매개 변수 집합 문제 해결
* Name 매개 변수를 제공하지 않으면 Get-AzVMExtension이 설치된 모든 확장을 열거하도록 업데이트
* Update-AzImage cmdlet에 태그 및 ResourceId 매개 변수 추가
* 인스턴스 ID가 없는 Get-AzVmssVM과 InstanceView를 사용하면 인스턴스 보기가 있는 VMSS VM을 나열할 수 있습니다.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* ADL 삭제된 항목 열거 및 복원에 대한 cmdlet 추가

#### <a name="azeventhub"></a>Az.EventHub
* Eventhub의 CaptureDescription 클래스에서 빈 보관을 건너뛰는 새 부울 속성 SkipEmptyArchives가 추가되었습니다. 

#### <a name="azkeyvault"></a>Az.KeyVault
* Set-AzKeyVaultSecret 태그 지정 수정

#### <a name="azlogicapp"></a>Az.LogicApp
* 통합 계정에 대한 기본 sku 추가
* XSLT 2.0, XSLT 3.0, Liquid 맵 형식 추가
* 통합 계정 어셈블리에 대한 새 cmdlet
    - Get-AzIntegrationAccountAssembly
    - New-AzIntegrationAccountAssembly
    - Remove-AzIntegrationAccountAssembly
    - Set-AzIntegrationAccountAssembly
* 통합 계정 일괄 처리 구성에 대한 새 cmdlet
    - Get-AzIntegrationAccountBatchConfiguration
    - New-AzIntegrationAccountBatchConfiguration
    - Remove-AzIntegrationAccountBatchConfiguration
    - Set-AzIntegrationAccountBatchConfiguration
* 논리 앱 SDK를 버전 4.1.0으로 업데이트

#### <a name="azmonitor"></a>Az.Monitor
* Get-AzMetric에 대한 도움말 업데이트

#### <a name="aznetwork"></a>Az.Network
* Add-AzApplicationGatewayCustomError에 대한 도움말 예제 업데이트

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* New 및 Get ApplicationInsights 데이터 소스에 대한 지원 추가
    - 지정된 작업 영역에 대한 특정 또는 전체 ApplicationInsights 데이터 원본 가져오기를 지원하기 위한 새로운 'ApplicationInsights' 종류가 추가되었습니다. 
    - 지정된 Application-Insights 리소스 매개 변수(구독 ID, resourceGroupName 및 이름)별로 데이터 원본을 만들기 위한 New-AzOperationalInsightsApplicationInsightsDataSource cmdlet이 추가되었습니다. 

#### <a name="azresources"></a>Az.Resources
* 문제 https://github.com/Azure/azure-powershell/issues/8166 수정
* 문제 https://github.com/Azure/azure-powershell/issues/8235 수정
* 문제 https://github.com/Azure/azure-powershell/issues/6219 수정
* KeyCredentials 반복 만들기를 방지하기 위해 버그 수정

#### <a name="azsql"></a>Az.Sql
* SQL DB 하이퍼스케일에 대한 지원 추가
* 복원 요청에서 불필요한 속성을 설정하여 복원이 실패할 수 있는 버그 수정

#### <a name="azwebsites"></a>Az.Websites
* Get-AzWebAppSlotMetrics 내 올바른 예제

## <a name="130---february-2019"></a>1.3.0 - 2019년 2월
#### <a name="azaccounts"></a>Az.Accounts
* ClientRuntime 최신 버전 업데이트

#### <a name="azanalysisservices"></a>Az.AnalysisServices
Az.AnalysisServices 모듈의 전반적인 가용성.

#### <a name="azcompute"></a>Az.Compute
* AEM 확장: UltraSSD 및 P60, P70, P80 디스크에 대한 지원 추가
* Set-AzVMBootDiagnostics에 대한 도움말 업데이트
* Update-AzImage에 대한 도움말 및 예제 업데이트

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
Az.RecoveryServices 모듈의 전반적인 가용성.

#### <a name="azresources"></a>Az.Resources
* 리소스 그룹 관련 태그 수정 
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8166 를 참조하세요.
* `Get-AzureRmRoleAssignment`이(가) -ErrorAction을 준수하지 않는 문제 수정 
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8235 를 참조하세요.

#### <a name="azsql"></a>Az.Sql
* AzSqlDatabaseBackupShortTermRetentionPolicy 가져오기/설정하기 추가
* SQL cmdlet을 실행할 경우 Azure 계정에 로그인되어 있지 않은 것이 nullref 예외를 초래하는 문제 수정
* Get-AzSqlCapability의 nullref 예외 수정

## <a name="121---january-2019"></a>1.2.1 - 2019년 1월
#### <a name="azaccounts"></a>Az.Accounts
* 올바른 인증 버전을 사용하여 릴리스

#### <a name="azanalysisservices"></a>Az.AnalysisServices
* 업데이트된 인증 종속성을 사용하여 릴리스

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* 업데이트된 인증 종속성을 사용하여 릴리스

## <a name="120---january-2019"></a>1.2.0 - 2019년 1월
#### <a name="azaccounts"></a>Az.Accounts
* Windows PowerShell 5.1 전용 대화형 사용자 이름/암호 인증 추가
* 잘못된 온라인 도움말 URL 업데이트
* Uninstall-AzureRm 관련 PS Core에 경고 메시지 추가

#### <a name="azaks"></a>Az.Aks
* 잘못된 온라인 도움말 URL 업데이트

#### <a name="azautomation"></a>Az.Automation
* Python 2 Runbook에 대한 지원이 추가되었습니다.
* 잘못된 온라인 도움말 URL 업데이트

#### <a name="azcdn"></a>Az.Cdn
* 잘못된 온라인 도움말 URL 업데이트

#### <a name="azcompute"></a>Az.Compute
* Invoke-AzVMReimage cmdlet 추가
* Set-AzVmss에 TempDisk 매개 변수 추가
* New-AzVM 경고 메시지 수정

#### <a name="azcontainerregistry"></a>Az.ContainerRegistry
* 잘못된 온라인 도움말 URL 업데이트

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF.Net SDK 버전이 3.0.0으로 업데이트되었습니다.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* MSI를 사용할 때 ADLS 엔드포인트 문제 수정
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7462 를 참조하세요.
* 잘못된 온라인 도움말 URL 업데이트

#### <a name="aziothub"></a>Az.IotHub
* Add-IotHubRoutingEndpoint cmdlet에 인코딩 형식을 추가하세요.

#### <a name="azkeyvault"></a>Az.KeyVault
* 잘못된 온라인 도움말 URL 업데이트

#### <a name="aznetwork"></a>Az.Network
* 잘못된 온라인 도움말 URL 업데이트

#### <a name="azresources"></a>Az.Resources
* 'New-AzADAppCredential' 및 'New-AzADSpCredential' 참조 설명서의 잘못된 예제 수정
* 리소스 그룹 배포 cmdlet 실행 전 '-TemplateFile' 매개 변수 경로가 확인되지 않는 문제 수정
* Az.Resources: New-AzureRmPolicyDefinition -Mode 기본값에 대한 올바른 설명서
* Az.Resources: 문제 https://github.com/Azure/azure-powershell/issues/7522 수정
* Az.Resources: 문제 https://github.com/Azure/azure-powershell/issues/5747 수정
* 'PSResourceGroupDeployment' 개체의 서식 문제 수정
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/2123 를 참조하세요.

#### <a name="azservicefabric"></a>Az.ServiceFabric
* 인증서가 VMSS 모델에 추가되었는데도 예외가 발생할 경우 롤백합니다. 이는 버그 https://github.com/Azure/service-fabric-issues/issues/932 를 수정하기 위함입니다.
* 일부 오류 메시지를 수정하세요.
* Az로의 마이그레이션을 통해서는 작동하지 않는 New-AzServiceFabriCluster를 위해 기본값 ARM 템플릿을 가진 클러스터 만들기를 수정하세요.
* 확장에서 클러스터 id를 확인하여 클러스터에 해당하는 VMSS에만 추가되도록 클러스터/애플리케이션 인증서 추가를 수정하세요.

#### <a name="azsignalr"></a>Az.SignalR
* 잘못된 온라인 도움말 URL 업데이트

#### <a name="azsql"></a>Az.Sql
* 잘못된 온라인 도움말 URL 업데이트
* 가능한 값을 가진 LicenseType 매개 변수에 대한 매개 변수 설명이 업데이트되었습니다.
* 유일하게 업데이트된 속성인데 작동하지 않는 관리되는 인스턴스 ID의 업데이트 수정
* 관리되는 인스턴스에서의 사용자 지정 데이터 정렬에 대한 지원

#### <a name="azstorage"></a>Az.Storage
* 잘못된 온라인 도움말 URL 업데이트
* Premium Storage 계정이 클래식 로깅/메트릭을 지원하지 않기 때문에, Premium Storage 계정의 클래식 로깅/메트릭을 가져올/설정할 때 상세한 오류 메시지를 제공해야 합니다.
    - Get/Set-AzStorageServiceLoggingProperty
    - Get/Set-AzStorageServiceMetricsProperty

#### <a name="aztrafficmanager"></a>Az.TrafficManager
* 잘못된 온라인 도움말 URL 업데이트

#### <a name="azwebsites"></a>Az.Websites
* 잘못된 온라인 도움말 URL 업데이트
* 앱이 ASE에 호스팅되면 'New-AzWebAppSSLBinding'을 수정하여 올바른 resourcegroup+location에 인증서를 업로드합니다.
* 'New-AzWebAppSSLBinding'을 수정하여 SSL 인증서를 앱에 바인딩하는 데 붙는 태그를 덮어쓰지 않도록 합니다.

## <a name="110---january-2019"></a>1.1.0 - 2019년 1월
#### <a name="azaccounts"></a>Az.Accounts
* Enable-AzureRmAlias에 'Local' 범위 추가

#### <a name="azcompute"></a>Az.Compute
* 이름이 Restart/Start/Stop/Remove/Set-AzVM과 Save-AzVMImage에 설정된 ID 매개 변수에서 선택 사항이 되었습니다.
* 도움말 파일의 ID에 대한 설명이 업데이트 되었습니다.
* Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* SDK 수정을 위해 데이터 평면의 SDK 버전을 1.1.14로 업데이트하세요.
    - getfilestatus 및 liststatus에 대한 음수 acesstime 및 modificationtime 수정, 비동기 취소 토큰 수정

#### <a name="azeventgrid"></a>Az.EventGrid
* 2019-01-01 API 버전을 사용하도록 업데이트되었습니다.
* 2019-01-01 API 버전에서 새 시나리오를 지원하도록 다음 cmdlet을 업데이트
    - New-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가
        - 이벤트 Time-to-Live
        - 이벤트에 대한 최대 배달 시도
        - 배달 못한 편지의 엔드포인트입니다.
    - Update-AzureRmEventGridSubscription: 지정을 위한 새로운 선택적 매개 변수를 추가
        - 이벤트 Time-to-Live
        - 이벤트에 대한 최대 배달 시도
        - 배달 못한 편지의 엔드포인트입니다.
* New-AzureRmEventGridSubscription 및 Update-AzureRmEventGridSubscription cmdlet의 EndpointType 옵션에 새 열거형 값(즉, storageQueue 및 hybridConnection)을 추가합니다.
* 이벤트 구독을 생성 또는 업데이트할 때 사용자가 직접 조치를 취해야 할 경우 경고 메시지를 표시합니다.

#### <a name="aziothub"></a>Az.IotHub
* 최신 버전의 Azure IotHub SDK로 업데이트됨

#### <a name="azlogicapp"></a>Az.LogicApp
* 지정된 이름이 없는 모든 Get-AzLogicApp 목록

#### <a name="azresources"></a>Az.Resources
* 'Get-AzResource'에 '-ODataQuery'및 '-ResourceId' 매개 변수를 제공할 때 매개 변수 집합 문제 수정
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/7875 를 참조하세요.
* New/Set-AzPolicyDefinition에서 -Custom 매개 변수 처리 문제 수정
* New-AzDeployment 설명서에서 오타 수정
* 'New-AzADUser'에 '-MailNickname'매개 변수가 필수 항목으로 지정됨
    - 자세한 내용은 여기 https://github.com/Azure/azure-powershell/issues/8220 를 참조하세요.

#### <a name="azsignalr"></a>Az.SignalR
* Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.

#### <a name="azsql"></a>Az.Sql
* Storage 관리 클라이언트 종속성을 일반적인 SDK 구현으로 변환했습니다.

#### <a name="azstorage"></a>Az.Storage
* Sas Token, OAuth 또는 Anonymous를 사용하여 스토리지 컨텍스트의 StorageAccountName을 실제 스토리지 계정 이름으로 설정합니다.
    - New-AzStorageContext
* '-FullUri' 매개 변수를 사용하여 Blob 스냅샷 개체의 Sas Token을 생성하고 반환된 Uri를 스냅샷 Uri로 수정합니다.
    - New-AzStorageBlobSASToken

#### <a name="azwebsites"></a>Az.Websites
* 'Get-AzDeletedWebApp'의 날짜 구문 분석 버그를 수정했습니다.
* Az.Accounts 모듈을 사용할 때의 이전 버전과의 호환성 문제를 해결합니다.

## <a name="100---december-2018"></a>1.0.0 - 2018년 12월
### <a name="general"></a>일반

- Az 모듈 일반 공급
- 각 모듈에 대 한 온라인 도움말
- 자세한 내용과 로드맵은 [Az 알림 페이지](https://aka.ms/azps-announce)를 참조하세요.
- AzureRM에서 마이그레이션하는 것에 대한 정보는 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azaccounts"></a>Az.Accounts
- Az.Profile에서 변경
- 프로필 및 컨텍스트 형식에 대한 표 형식 수정

### <a name="azapimanagement"></a>Az.ApiManagement
- #7002에 대한 수정
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azbatch"></a>Az.Batch
- `PSComputeNode`의 새로운 `NodeAgentInformation` 속성을 통해 풀의 각 VM에서 실행 중인 Azure Batch 노드 에이전트의 버전을 확인하는 기능이 추가되었습니다.
- `PSDataDisk`에 대한 `Caching` 기본 값은 이제 `None` 대신 `ReadWrite`입니다.
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azbilling"></a>Az.Billing
- 청구, 소비 및 UsageAggregates cmdlet 결합 cmdlet에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azcognitivservices"></a>Az.CognitivServices
- New-AzureRmCognitiveServicesAccount 작업에서 사용 가능한 SkuName 및 Typem에 대한 완성자 추가
- Get-AzCognitiveServicesAccountSkus에서 GetSkusWithAccountParamSetName 매개 변수 집합을 제거

### <a name="azcontainerinstance"></a>Az.ContainerInstance
- ManagedIdentity 지원이 추가됨

### <a name="azdatalakeanalytics"></a>Az.DataLakeAnalytics
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azdatalakestore"></a>Az.DataLakeStore
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azmonitor"></a>Az.Monitor
- Az.Monitor 이름 변경 및 기타 사소한 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azkeyvault"></a>Az.KeyVault
- 출력 형식에서 사용되지 않는 'PurgeDisabled' 속성 제거

### <a name="azmachinelearning"></a>Az.MachineLearning
- Az.MachineLearningCompute 모듈의 cmdlet 포함

### <a name="azmedia"></a>Az.Media
- New-AzMediaService에서 사용되지 않는 -Tags 별칭이 제거됨

### <a name="aznetwork"></a>Az.Network
Application Gateway에서 RewriteRuleSets를 구성하는 것에 대한 지원이 추가됨
    - 추가된 새 cmdlet은 다음과 같습니다.
        - Add-AzureRmApplicationGatewayRewriteRuleSet
        - Get-AzureRmApplicationGatewayRewriteRuleSet
        - New-AzureRmApplicationGatewayRewriteRuleSet
        - Remove-AzureRmApplicationGatewayRewriteRuleSet
        - Set-AzureRmApplicationGatewayRewriteRuleSet
        - New-AzureRmApplicationGatewayRewriteRule
        - New-AzureRmApplicationGatewayRewriteRuleActionSet
        - New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration
    - 선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -RewriteRuleSet
        - New-AzureRmApplicationGateway
        - New-AzureRmApplicationGatewayRequestRoutingRule
        - Add-AzureRmApplicationGatewayRequestRoutingRule
        - New-AzureRmApplicationGatewayPathRuleConfig
        - Add-AzureRmApplicationGatewayUrlPathMapConfig
        - New-AzureRmApplicationGatewayUrlPathMapConfig로 ID를 사용하여 Application Gateway에 KeyVault 지원을 추가했습니다.
    - 선택적 매개 변수를 사용하도록 cmdlet이 업데이트됨 -KeyVaultSecretId, -KeyVaultSecret
        - Add-AzApplicationGatewaySslCertificate
        - New-AzApplicationGatewaySslCertificate
        - Set-AzApplicationGatewaySslCertificate
    - New-AzApplicationGateway cmdlet이 선택적 매개 변수를 사용하도록 업데이트됨 -UserAssignedIdentity
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azoperationalinsights"></a>Az.OperationalInsights
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azprofile"></a>Az.Profile
- Az.Accounts에 모듈 이름이 변경됨

### <a name="azrecoveryservices"></a>Az.RecoveryServices
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azresources"></a>Az.Resources
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azservicefabric"></a>Az.ServiceFabric
- 일반 이름과 지문으로 지정 인증서 지원
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azsignalr"></a>Az.SIgnalR
- SIgnalR에 대한 PowerShell cmdlet에 대한 일반 공급

### <a name="azsql"></a>Az.Sql
- 위협 탐지의 cmdlet에 새로운 Data_Exfiltration 및 Unsafe_Action 검색 유형 추가
- Sql 감사 cmdlet에 대한 설명서 예제 업데이트
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azstorage"></a>Az.Storage
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

### <a name="azwebsites"></a>Az.Websites
- 부수적인 호환성이 손상되는 변경에 대한 자세한 내용은 [마이그레이션 가이드](https://aka.ms/azps-migration-guide)를 참조하세요.

## <a name="070---december-2018"></a>0.7.0 - 2018년 12월

### <a name="general"></a>일반

* AzureRM에서 Az 전환 예정에 대한 사소한 변경

### <a name="azcompute"></a>Az.Compute

* `New-AzVm(ss)` cmdlet에 대한 간단한 매개 변수 집합에 UltraSSD 및 갤러리 이미지에 대한 지원을 추가합니다.

### <a name="azdatalakestore"></a>Az.DataLakeStore

* ADLS 계정의 도메인의 후행 슬래시를 수정합니다.

### <a name="azfrontdoor"></a>Az.FrontDoor

* 일부 끊어진 링크 수정
    - New-AzureRmFrontDoor 및 Set-AzureRmFrontDoor 아티클에서 New-AzureRmFrontDoorHealthProbeSettingObject cmdlet 아티클에 대한 링크가 수정되었습니다.
    - New-AzureRmFrontDoorManagedRuleObject 아티클에서 New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet 아티클에 대한 링크가 수정되었습니다.

### <a name="azrecoveryservices"></a>Az.RecoveryServices

* Azure File Share 복원 작업에 클라이언트 측 유효성 검사가 추가되었습니다.
* afs 복원의 경우 storageAccountName 및 storageAccountResourceGroupName을 선택적으로 만들었습니다.

### <a name="azresources"></a>Az.Resources

* 에 대 한 수정 https://github.com/Azure/azure-powershell/issues/7679
    - 기본 관리자를 요청할 때 구독 범위가 제공되는 경우 Get-AzureRmRoleAssignment를 업데이트하여 구독 범위를 사용합니다.

### <a name="azsql"></a>Az.Sql

* AzureRM에서 Az 전환 예정에 대한 사소한 변경
* DotNet 코어에서 Get-AzureRmSqlDatabaseVulnerabilityAssessment를 사용하는 문제 해결
* SQL 감사 cmdlet과 관련된 도움말 메시지의 설명서가 수정되었습니다.

### <a name="azstorage"></a>Az.Storage

* New-AzureRmStorageAccount에 -EnableHierarchicalNamespace 추가
* 파일 복사 cmdlet이 -DestContext 입력이 없을 때 대상의 원본 컨텍스트를 다시 사용할 수 없는 문제 수정
    - Start-AzureStorageFileCopy
* 고정적인 웹 사이트 구성 지원
    - Enable-AzureStorageStaticWebsite
    - Disable-AzureStorageStaticWebsite

### <a name="azwebsites"></a>Az.Websites

* Set-AzureRmWebApp 및 Set-AzureRmWebAppSlot 
    - Windows 및 Linux 컨테이너 응용 프로그램에 탑재할 Azure Storage 경로를 지정하기 위해 새 매개 변수(-AzureStoragePath)가 추가되었습니다. 새 cmdlet New-AzureRmWebAppAzureStoragePath의 출력을 매개 변수로 사용하여 Azure Storage 경로를 설정합니다.

## <a name="061---november-2018"></a>0.6.1 - 2018년 11월

### <a name="azapimanagement"></a>Az.ApiManagement
* 형식 매핑 문제에 대한 종속성 업데이트

### <a name="azautomation"></a>Az.Automation
* Azure Automation cmdlet 기반 Swagger
* 업데이트 관리 cmdlet 추가
* 소스 제어 cmdlet 추가
* Remove-AzureRmAutomationHybridWorkerGroup cmdlet 추가
* DSC 노드 등록 명령 수정

### <a name="azcompute"></a>Az.Compute
* SystemAssigned ID에 대한 ID 문제 수정
* 형식 매핑 문제에 대한 종속성 업데이트

### <a name="azcontainerinstance"></a>Az.ContainerInstance
* 형식 매핑 문제에 대한 종속성 업데이트

### <a name="azmarketplaceordering"></a>Az.MarketplaceOrdering
* 마켓플레이스 cmdlet에 대한 예제 설명 업데이트

### <a name="aznetwork"></a>Az.Network
* New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError cmdlet 추가
* 지원되는 AzureFirewall 네트워크 프로토콜에 ICMP 다시 추가
* Test-AzureRmNetworkWatcherConnectivity cmdlet을 업데이트하여 대상 ID, 주소 및 포트 유효성 검사를 추가합니다. 
* VirtualNetwork 맵의 메모리 사용 문제 해결

### <a name="azrecoveryservicesbackup"></a>Az.RecoveryServices.Backup
* 보호된 파일 공유에 대한 정책을 수정하는 것에 대해 수정합니다.
* 정책 표준 시간대를 대문자로 변환했습니다.

### <a name="azrecoveryservicessiterecovery"></a>Az.RecoveryServices.SiteRecovery
* New-AzureRmRecoveryServicesAsrProtectableItem의 예제 정정
* 형식 매핑 문제에 대한 종속성 업데이트

### <a name="azrelay"></a>Az.Relay
* 선택적 매개 변수 -KeyValue를 New-AzureRmRelayKey cmdlet에 추가하여 사용자가 KeyValue를 제공할 수 있습니다.

### <a name="azresources"></a>Az.Resources
* `New-AzureRmPolicyAssignment` 및 `Set-AzureRmPolicyAssignment`의 자원 ID 관련 매개 변수에 대한 도움말 문서를 업데이트함
* -Metadata를 사용하는 New-AzureRmPolicyDefinition에 대한 예제 추가
* NetStandard의 태그 키에서 대소문자 보존을 허용하도록 수정: #7678 #7703

### <a name="azservicefabric"></a>Az.ServiceFabric
* 향후 호환성이 손상되는 변경에 대한 사용 중단 메시지 추가

### <a name="azsql"></a>Az.Sql
* Azure Sql Database Managed Instance 및 Azure Sql Managed Database에 CRUD 작업을 위한 새 cmdlet 추가
    - Get-AzureRmSqlInstance
    - New-AzureRmSqlInstance
    - Set-AzureRmSqlInstance
    - Remove-AzureRmSqlInstance
    - Get-AzureRmSqlInstanceDatabase
    - New-AzureRmSqlInstanceDatabase
    - Restore-AzureRmSqlInstanceDatabase
    - Remove-AzureRmSqlInstanceDatabase
* 서버 또는 데이터베이스에서 확장 감사 정책 관리를 활성화했습니다.
    - 새 매개 변수(PredicateExpression)가 감사 로그 필터링을 사용하도록 추가되었습니다.
    - Cmdlet이 레거시 클라이언트 대신 SQL 클라이언트를 사용하도록 수정되었습니다.
    - Set-AzureRmSqlServerAuditing.
    - Get-AzureRmSqlServerAuditing.
    - Set-AzureRmSqlDatabaseAuditing.
    - Get-AzureRmSqlDatabaseAuditing.
* 스토리지 계정 이름 매개 변수가 설정된 Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings를 사용할 때의 문제 해결

## <a name="050---november-2018"></a>0.5.0 - 2018년 11월
#### <a name="general"></a>일반
* 많은 핵심 cmdlet에 Resource Completers를 추가하여 대화형으로 cmdlet을 호출할 때 기존 리소스 이름을 탭으로 이동할 수 있습니다.

#### <a name="azprofile"></a>Az.Profile
* ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.
* Connect-AzAccount cmdlet의 매개 변수 TenantId 이름을 Tenant로 바꾸고 TenantId의 별칭을 추가합니다
* Connect-AzAccount의 업데이트된 TenantId 설명
* 테넌트 도메인을 제공할 때 실패한 로그인에 대한 오류 메시지 수정
    - https://github.com/Azure/azure-powershell/issues/6936
* 테넌트에 구독이 없는 계정의 컨텍스트 이름 충돌 문제 수정
    - https://github.com/Azure/azure-powershell/issues/7453
* MSI를 사용할 때 DataLake 엔드포인트 문제 수정
    - https://github.com/Azure/azure-powershell/issues/7462
* 연결되지 않은 경우 'Disconnect-AzAccount'가 throw하는 문제 수정
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Get-AzCognitiveServicesAccountSkus 작업을 추가합니다.

#### <a name="azcompute"></a>Az.Compute
* Add-AzVmssVMDataDisk 및 Remove-AzVmssVMDataDisk cmdlet를 추가합니다
* Get-AzVMImage는 AutomaticOSUpgradeProperties를 표시합니다
* 수정된 SetAzVMChefExtension -BootstrapOptions 및 -JsonAttribute option 값이 json 형식으로 설정하지 않습니다.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* DataLake 패키지를 1.1.10으로 업데이트합니다.
* 기본 동시성을 다중 스레드 작업에 추가합니다.

#### <a name="azinsights"></a>Az.Insights
* 해결된 문제 #7267(자동 크기 조정 영역)
    - 열거된 매개 변수를 제대로 설정하지 않은 새 자동 크기 조정 규칙을 만드는 데 문제가 있습니다(이를 항상 기본값으로 설정함).
* 해결된 문제 # 7513[자세한 정보] Set-AzDiagnosticSetting은 설정을 생성하는 동안 범주를 명시적으로 지정해야 합니다
    - 이제 cmdlet은 생성 중에 사용할 범주를 명시적으로 표시할 필요가 없습니다. 즉, 문서화된대로 작동합니다

#### <a name="aznetwork"></a>Az.Network
* 다음 cmdlet에 대해 PeeringType을 필수 매개 변수로 변경했습니다.
    - Get-AzExpressRouteCircuitRouteTable
    - Get-AzExpressRouteCircuitARPTable
    - Get-AzExpressRouteCircuitRouteTableSummary
    - Get-AzExpressRouteCrossConnectionArpTable
    - Get-AzExpressRouteCrossConnectionRouteTable
    - Get-AzExpressRouteCrossConnectionRouteTableSummary

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* 추가된 정책 재구성 cmdlet

#### <a name="azresources"></a>Az.Resources
* 에 대 한 수정 https://github.com/Azure/azure-powershell/issues/7402
    - 'Get-AzResource'에 대해 '-ResourceId' 매개 변수를 사용하여 리소스 나열 허용

#### <a name="azservicebus"></a>Az.ServiceBus
* 마이그레이션 상태를 알 수 있도록 PSServiceBusMigrationConfigurationAttributes에 MigrationState 읽기 전용 속성 추가.

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Linux Vmss에 인증서 추가 수정.
* Add-AzServiceFabricClusterCertificate 수정
    - 새 인증서(Azure/service-fabric-issues#932)에서 올바른 지문을 사용.
    - 올바르게 예외 표시(Azure/service-fabric-issues#1054).
* Vmss CreateOrUpdate 작업을 시작하기 전에 'Update-AzServiceFabricDurability'를 수정하여 클러스터 구성 업데이트.

## <a name="040---october-2018"></a>0.4.0 - 2018년 10월
#### <a name="azprofile"></a>Az.Profile
* CloudShell에서 Get-AzSubscription을 사용하여 문제를 해결합니다.
* ClientRuntime의 최신 버전을 사용하도록 일반적인 코드를 업데이트합니다.

#### <a name="azcompute"></a>Az.Compute
* 'New-AzVm'에 대해 간단한 매개 변수를 사용하는 경우 가속화된 네트워킹을 설정하기 위해 새 크기가 VM 크기의 허용 목록에 추가되었습니다.
* 모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Virtual Network 규칙에 대한 지원 추가
    - Get-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 가져오거나 나열합니다.
    - Add-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 가상 네트워크 규칙을 추가합니다.
    - Set-AzDataLakeStoreVirtualNetworkRule: 지정된 Data Lake Store 계정에 지정된 가상 네트워크 규칙을 수정합니다.
    - Remove-AzDataLakeStoreVirtualNetworkRule: Azure Data Lake Store 가상 네트워크 규칙을 삭제합니다.

#### <a name="aznetwork"></a>Az.Network
* Test-AzNetworkWatcherConnectivity cmdlet을 업데이트하고, 백 엔드에 프로토콜 값을 전달합니다.
* 모든 cmdlet에 ResourceName 인수 완성자가 추가되었습니다.

#### <a name="azresources"></a>Az.Resources
* (기본 프로필에 구독이 없고 범위가 지정되지 않은 경우) 시나리오에서 의미 있는 예외를 추가하여 Get-AzRoleDefinition이 인식할 수 없는 예외를 throw하는 문제를 수정합니다. 또한 기본 매개 변수 집합을 'RoleDefinitionNameParameterSet'으로 설정합니다.

## <a name="030---october-2018"></a>0.3.0 - 2018년 10월
#### <a name="azurestorage"></a>Azure.Storage
* 대상에 메타데이터가 있을 때 Blob/파일이 메타 데이터를 복사하지 않는 문제 수정
    - Start-AzureStorageBlobCopy
    - Start-AzureStorageFileCopy
* 특정 위치의 저장소 리소스 사용을 지원하고 글로벌 저장소 리소스 사용 가져오기는 더 이상 사용되지 않는다는 경고 메시지를 추가합니다.
    - Get-AzStorageUsage
    
#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* 기존 계정이 없는 Get-AzCognitiveServicesAccountSkus를 지원합니다.

#### <a name="azcompute"></a>Az.Compute
* Get-AzVM -ResourceGroupName <rg>가 필요한 경우 50개가 넘는 결과를 반환하도록 수정
* 'SimpleParameterSet' 예제가 New-AzVmss cmdlet 도움말에 추가됨
* Azure Disk Encryption 진행률 메시지의 오타를 수정

#### <a name="azdatafactoryv2"></a>Az.DataFactoryV2
* ADF.Net SDK 버전을 2.3.0으로 업데이트

#### <a name="aznetwork"></a>Az.Network
* NetworkProfile 기능 추가 추가된 새 cmdlet은 다음과 같습니다.
    - Get-AzNetworkProfile
    - New-AzNetworkProfile
    - Remove-AzNetworkProfile
    - Set-AzNetworkProfile
    - New-AzContainerNicConfig
    - New-AzContainerNicConfigIpConfig
* 서브넷 모델에 서비스 연결 링크 추가
* New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap cmdlet 추가
* Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig cmdlet 추가

#### <a name="azrediscache"></a>Az.RedisCache
* 모든 문자열을 Size 매개 변수로 진행되도록 허용 PSArgumentCompleter 팝업에 P5 추가

#### <a name="azresources"></a>Az.Resources
* -Mode 매개 변수를 Set-AzPolicyDefinition에 추가
* 사용자가 포함된 Origin 작업에서 Get-AzProviderOperation commandlet 버그 수정

#### <a name="azsql"></a>Az.Sql
* 일부 백업 cmdlet이 현재 azure 구독을 인식하지 않는 문제 해결

#### <a name="azwebsites"></a>Az.Websites
* 새 cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - 컨테이너 지속적인 배포 Webhook URL을 가져옵니다.
* 새 cmdlet New-AzWebAppContainerPSSession 및 Enter-WebAppContainerPSSession -  windows 컨테이너 앱에 PowerShell 원격 세션을 시작합니다.

## <a name="020---september-2018"></a>0.2.0 - 2018년 9월
 최초 릴리스