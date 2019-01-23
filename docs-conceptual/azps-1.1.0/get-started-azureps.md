---
title: Azure PowerShell 시작
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 01/14/2019
ms.openlocfilehash: 483e74d7d047562b1c170c3767495161b9c5eb2f
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342000"
---
# <a name="get-started-with-azure-powershell"></a><span data-ttu-id="38c4d-102">Azure PowerShell 시작</span><span class="sxs-lookup"><span data-stu-id="38c4d-102">Get started with Azure PowerShell</span></span>

<span data-ttu-id="38c4d-103">Azure PowerShell은 명령줄에서 Azure 리소스를 관리하기 위해 설계되었습니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-103">Azure PowerShell is designed for managing and administering Azure resources from the command line.</span></span> <span data-ttu-id="38c4d-104">Azure Resource Manager 모델을 사용하는 자동화된 도구를 만들려는 경우 Azure PowerShell을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="38c4d-104">Use Azure PowerShell when you want to build automated tools that use the Azure Resource Manager model.</span></span>
<span data-ttu-id="38c4d-105">[Azure Cloud Shell](/azure/cloud-shell/overview)과 함께 브라우저에서 사용하거나 로컬 컴퓨터에 설치하여 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="38c4d-105">Try it out in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or install on your local machine.</span></span>

<span data-ttu-id="38c4d-106">이 문서에서는 Azure PowerShell을 시작하는 방법 및 핵심 개념을 설명합니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-106">This article helps you get started with Azure PowerShell and teaches the core concepts behind it.</span></span>

## <a name="install-or-run-in-azure-cloud-shell"></a><span data-ttu-id="38c4d-107">Azure Cloud Shell에서 설치 또는 실행</span><span class="sxs-lookup"><span data-stu-id="38c4d-107">Install or run in Azure Cloud Shell</span></span>

<span data-ttu-id="38c4d-108">Azure PowerShell을 시작하는 가장 쉬운 방법은 Azure Cloud Shell 환경에서 시도하는 것입니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-108">The easiest way to get started with Azure PowerShell is by trying it out in an Azure Cloud Shell environment.</span></span>
<span data-ttu-id="38c4d-109">Azure Cloud Shell을 실행하려면 [Azure Cloud Shell에서 PowerShell 빠른 시작](/azure/cloud-shell/quickstart-powershell)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="38c4d-109">To get up and running with Cloud Shell, see [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
<span data-ttu-id="38c4d-110">Cloud Shell은 Linux 컨테이너에서 PowerShell 6을 실행하므로 Windows 관련 기능을 사용할 수 없습니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-110">Cloud Shell runs PowerShell 6 on a Linux container, so Windows-specific functionality isn't available.</span></span>

<span data-ttu-id="38c4d-111">로컬 컴퓨터에 Azure PowerShell을 설치할 준비가 되면 [Azure PowerShell 모듈 설치](install-az-ps.md)의 지침을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-111">When you're ready to install Azure PowerShell on your local machine, follow the instructions in [Install the Azure PowerShell module](install-az-ps.md).</span></span>

## <a name="sign-in-to-azure"></a><span data-ttu-id="38c4d-112">Azure에 로그인</span><span class="sxs-lookup"><span data-stu-id="38c4d-112">Sign in to Azure</span></span>

<span data-ttu-id="38c4d-113">`Connect-AzAccount` cmdlet을 사용하여 대화형으로 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-113">Sign in interactively with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="38c4d-114">Cloud Shell을 사용하는 경우 이 단계를 건너뜁니다. Azure Cloud Shell 세션은 Cloud Shell 세션을 시작한 환경, 구독 및 테넌트에 대해 이미 인증되었습니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-114">Skip this step if you use Cloud Shell: Your Auzre Cloud Shell session is already authenticated for the environment, subscription, and tenant that launched the Cloud Shell session.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="38c4d-115">미국 이외 지역의 경우 `-Environment` 매개 변수를 사용하여 로그인합니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-115">If you're in a non-US region, use the `-Environment` parameter to sign in.</span></span> <span data-ttu-id="38c4d-116">[Get-AzEnvironment](/powershell/module/Az.Accounts/Get-AzEnvironment) cmdlet을 사용하여 해당 지역의 환경 이름을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-116">Get the name of the environment for your region by using the [Get-AzEnvironment](/powershell/module/Az.Accounts/Get-AzEnvironment) cmdlet.</span></span> <span data-ttu-id="38c4d-117">예를 들어, Azure 중국 21Vianet에 로그인하려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-117">For example, to sign in to Azure China 21Vianet:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="38c4d-118">https://microsoft.com/devicelogin에 사용할 토큰을 얻게 됩니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-118">You'll get a token to use on https://microsoft.com/devicelogin.</span></span> <span data-ttu-id="38c4d-119">브라우저에서 이 페이지를 열고 토큰을 입력하여 Azure 계정 자격 증명으로 로그인하고 Azure PowerShell을 승인하세요.</span><span class="sxs-lookup"><span data-stu-id="38c4d-119">Open this page in your browser and enter the token, then sign in with your Azure account credentials and authorize Azure PowerShell.</span></span> 

<span data-ttu-id="38c4d-120">Azure 계정에 로그인하면 Azure PowerShell cmdlet을 사용하여 구독에서 관리자 리소스에 액세스할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-120">Once signed in, use the Azure PowerShell cmdlets to access and manage resources in your subscription.</span></span> <span data-ttu-id="38c4d-121">로그인 프로세스 및 인증 방법에 대한 자세한 내용은 [Azure PowerShell을 사용하여 로그인](authenticate-azureps.md)을 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-121">To learn more about the sign-in process and authentication methods, see [Sign in with Azure PowerShell](authenticate-azureps.md).</span></span>

## <a name="find-commands"></a><span data-ttu-id="38c4d-122">명령 찾기</span><span class="sxs-lookup"><span data-stu-id="38c4d-122">Find commands</span></span>

<span data-ttu-id="38c4d-123">Azure PowerShell cmdlet은 PowerShell을 위한 표준 명명 규칙인 `VERB-NOUN`을 따릅니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-123">Azure PowerShell cmdlets follow a standard naming convention for PowerShell, `VERB-NOUN`.</span></span> <span data-ttu-id="38c4d-124">동사는 작업(예: `Create`,`Get`,`Set`,`Delete`)을 설명하고 명사는 리소스 종류를 설명합니다(예:`AzVM`,`AzKeyVaultCertificate`,`AzFirewall`,`AzVirtualNetworkGateway`).</span><span class="sxs-lookup"><span data-stu-id="38c4d-124">The verb describes the action (examples include `Create`, `Get`, `Set`, `Delete`) and the noun describes the resource type (examples include `AzVM`, `AzKeyVaultCertificate`, `AzFirewall`, `AzVirtualNetworkGateway`).</span></span> <span data-ttu-id="38c4d-125">Azure PowerShell에서 명사는 항상 접두사 `Az`를 사용하여 시작합니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-125">Nouns in Azure PowerShell always start with the prefix `Az`.</span></span> <span data-ttu-id="38c4d-126">표준 동사의 전체 목록은 [PowerShell 명령에 대한 승인된 동사](/powershell/developer/cmdlet/approved-verbs-for-windows-powershell-commands)를 참조합니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-126">For the full list of standard verbs, see [Approved verbs for PowerShell Commands](/powershell/developer/cmdlet/approved-verbs-for-windows-powershell-commands).</span></span>

<span data-ttu-id="38c4d-127">사용 가능한 명사, 동사 및 Azure PowerShell 모듈을 알면 [Get-Command](/powershell/module/microsoft.powershell.core/get-command) cmdlet을 사용하여 명령을 찾을 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-127">Knowing the nouns, verbs, and the Azure PowerShell modules available help you find commands with the [Get-Command](/powershell/module/microsoft.powershell.core/get-command) cmdlet.</span></span> <span data-ttu-id="38c4d-128">예를 들어 `Get` 동사를 사용하는 VM 관련 명령을 모두 찾으려면 다음을 수행합니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-128">For example, to find all VM-related commands that use the `Get` verb:</span></span>

```powershell-interactive
Get-Command -Verb Get -Noun AzVM* -Module Az.Compute
```

<span data-ttu-id="38c4d-129">일반 명령을 찾는 데 도움이 되도록 이 표에는 리소스 종류, 해당 Azure PowerShell 모듈 및 `Get-Command`와 함께 사용할 명사 접두사가 나열되어 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-129">To help you find common commands, this table lists the resource type, corresponding Azure PowerShell module, and noun prefix to use with `Get-Command`:</span></span>

| <span data-ttu-id="38c4d-130">리소스 종류</span><span class="sxs-lookup"><span data-stu-id="38c4d-130">Resource type</span></span> | <span data-ttu-id="38c4d-131">Azure PowerShell 모듈</span><span class="sxs-lookup"><span data-stu-id="38c4d-131">Azure PowerShell module</span></span> | <span data-ttu-id="38c4d-132">명사 접두사</span><span class="sxs-lookup"><span data-stu-id="38c4d-132">Noun prefix</span></span> |
|---------------|-------------------------|----------------|
| [<span data-ttu-id="38c4d-133">리소스 그룹</span><span class="sxs-lookup"><span data-stu-id="38c4d-133">Resource group</span></span>](/azure/azure-resource-manager/resource-group-overview) | [<span data-ttu-id="38c4d-134">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="38c4d-134">Az.Resources</span></span>](/powershell/module/az.resources#resources) | `AzResourceGroup` |
| [<span data-ttu-id="38c4d-135">가상 머신</span><span class="sxs-lookup"><span data-stu-id="38c4d-135">Virtual machines</span></span>](/azure/virtual-machines) | [<span data-ttu-id="38c4d-136">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="38c4d-136">Az.Compute</span></span>](/powershell/module/az.compute#virtual_machines) | `AzVM` |
| [<span data-ttu-id="38c4d-137">Storage 계정</span><span class="sxs-lookup"><span data-stu-id="38c4d-137">Storage accounts</span></span>](/azure/storage/common/storage-introduction) | [<span data-ttu-id="38c4d-138">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="38c4d-138">Az.Storage</span></span>](/powershell/module/az.storage/) | `AzStorageAccount` |
| [<span data-ttu-id="38c4d-139">Key Vault</span><span class="sxs-lookup"><span data-stu-id="38c4d-139">Key Vault</span></span>](/azure/key-vault/key-vault-whatis) | [<span data-ttu-id="38c4d-140">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="38c4d-140">Az.KeyVault</span></span>](/powershell/module/az.keyvault) | `AzKeyVault` |
| [<span data-ttu-id="38c4d-141">웹 애플리케이션</span><span class="sxs-lookup"><span data-stu-id="38c4d-141">Web applications</span></span>](/azure/app-service) | [<span data-ttu-id="38c4d-142">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="38c4d-142">Az.Websites</span></span>](/powershell/module/az.websites) | `AzWebApp` |
| [<span data-ttu-id="38c4d-143">SQL 데이터베이스</span><span class="sxs-lookup"><span data-stu-id="38c4d-143">SQL databases</span></span>](/azure/sql-database) | [<span data-ttu-id="38c4d-144">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="38c4d-144">Az.Sql</span></span>](/powershell/module/az.sql) | `AzSqlDatabase` |

<span data-ttu-id="38c4d-145">Azure PowerShell의 모듈 전체 목록은 GitHub에서 호스팅되는 [Azure PowerShell 모듈 목록](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md)을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="38c4d-145">For a full list of the modules in Azure PowerShell, see the [Azure PowerShell modules list](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md) hosted on GitHub.</span></span>

## <a name="learn-azure-powershell-basics-with-quickstarts-and-tutorials"></a><span data-ttu-id="38c4d-146">빠른 시작 및 자습서로 Azure PowerShell 기본 내용 학습</span><span class="sxs-lookup"><span data-stu-id="38c4d-146">Learn Azure PowerShell basics with quickstarts and tutorials</span></span>

<span data-ttu-id="38c4d-147">Azure PowerShell을 시작하려면 가상 머신 설정 및 쿼리 방법에 대한 심층적인 자습서를 참조해 보세요.</span><span class="sxs-lookup"><span data-stu-id="38c4d-147">To get started with Azure PowerShell, try an in-depth tutorial for setting up virtual machines and learning how to query them.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="38c4d-148">Azure PowerShell로 가상 머신 만들기</span><span class="sxs-lookup"><span data-stu-id="38c4d-148">Create virtual machines with Azure PowerShell</span></span>](azureps-vm-tutorial.yml)

<span data-ttu-id="38c4d-149">기타 인기 Azure 서비스에 대한 Azure PowerShell 빠른 시작도 있습니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-149">There are also Azure PowerShell quickstarts for other popular Azure services:</span></span>

* [<span data-ttu-id="38c4d-150">저장소 계정을 만드는</span><span class="sxs-lookup"><span data-stu-id="38c4d-150">Create a storage account</span></span>](/azure/storage/common/storage-quickstart-create-account?tabs=azure-powershell)
* [<span data-ttu-id="38c4d-151">Azure Blob Storage 간에 개체 전송</span><span class="sxs-lookup"><span data-stu-id="38c4d-151">Transfer objects to/from Azure Blob storage</span></span>](/azure/storage/blobs/storage-quickstart-blobs-powershell)
* [<span data-ttu-id="38c4d-152">Azure Key Vault에서 비밀을 만들고 검색</span><span class="sxs-lookup"><span data-stu-id="38c4d-152">Create and retrieve secrets from Azure Key Vault</span></span>](/azure/key-vault/quick-create-powershell)
* [<span data-ttu-id="38c4d-153">Azure SQL 데이터베이스 및 방화벽 만들기</span><span class="sxs-lookup"><span data-stu-id="38c4d-153">Create an Azure SQL database and firewall</span></span>](/azure/sql-database/scripts/sql-database-create-and-configure-database-powershell)
* [<span data-ttu-id="38c4d-154">Azure Container Instances의 컨테이너 실행</span><span class="sxs-lookup"><span data-stu-id="38c4d-154">Run a container in Azure Container Instances</span></span>](/azure/container-instances/container-instances-quickstart-powershell)
* [<span data-ttu-id="38c4d-155">가상 머신 확장 집합 만들기(VMSS)</span><span class="sxs-lookup"><span data-stu-id="38c4d-155">Create a Virtual Machine Scale Set (VMSS)</span></span>](/azure/virtual-machine-scale-sets/quick-create-powershell)
* [<span data-ttu-id="38c4d-156">표준 부하 분산 장치 만들기</span><span class="sxs-lookup"><span data-stu-id="38c4d-156">Create a standard load balancer</span></span>](/azure/load-balancer/quickstart-create-standard-load-balancer-powershell)

## <a name="next-steps"></a><span data-ttu-id="38c4d-157">다음 단계</span><span class="sxs-lookup"><span data-stu-id="38c4d-157">Next steps</span></span>

* [<span data-ttu-id="38c4d-158">Azure PowerShell로 로그인</span><span class="sxs-lookup"><span data-stu-id="38c4d-158">Sign in with Azure PowerShell</span></span>](authenticate-azureps.md)
* [<span data-ttu-id="38c4d-159">Azure PowerShell을 사용하여 Azure 구독 관리</span><span class="sxs-lookup"><span data-stu-id="38c4d-159">Manage Azure subscriptions with Azure PowerShell</span></span>](manage-subscriptions-azureps.md)
* [<span data-ttu-id="38c4d-160">Azure PowerShell로 서비스 주체 만들기</span><span class="sxs-lookup"><span data-stu-id="38c4d-160">Create service principals with Azure PowerShell</span></span>](create-azure-service-principal-azureps.md)
* <span data-ttu-id="38c4d-161">커뮤니티에서 도움말을 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="38c4d-161">Get help from the community:</span></span>
  * [<span data-ttu-id="38c4d-162">MSDN의 azure 포럼</span><span class="sxs-lookup"><span data-stu-id="38c4d-162">Azure forum on MSDN</span></span>](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [<span data-ttu-id="38c4d-163">Stacki 오버플로</span><span class="sxs-lookup"><span data-stu-id="38c4d-163">Stacki Overflow</span></span>](http://go.microsoft.com/fwlink/?LinkId=320213)
