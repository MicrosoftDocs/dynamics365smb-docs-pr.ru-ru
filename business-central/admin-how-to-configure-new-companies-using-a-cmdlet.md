---
title: "Настройка новых организаций с помощью командлета | Документы Майкрософт"
description: "В некоторых сценариях может потребоваться загрузить и импортировать пакет конфигурации без участия пользователей или без использования пользовательского интерфейса служб RapidStart Services. Для этого можно воспользоваться командлетом Windows PowerShell."
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/06/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 9d248f2f8676c392451ae4a6f99932145f354f5b
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="configure-new-companies-using-a-cmdlet"></a><span data-ttu-id="d795f-104">Настройка новых организаций с помощью командлета</span><span class="sxs-lookup"><span data-stu-id="d795f-104">Configure New Companies using a Cmdlet</span></span>
<span data-ttu-id="d795f-105">В некоторых сценариях может потребоваться загрузить и импортировать пакет конфигурации без участия пользователей или без использования пользовательского интерфейса служб RapidStart Services.</span><span class="sxs-lookup"><span data-stu-id="d795f-105">In a number of scenarios, you may want to load and import a configuration package without involving your users or using the RapidStart Services user interface.</span></span> <span data-ttu-id="d795f-106">Для этого можно воспользоваться командлетом Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d795f-106">You can do so by using a Windows PowerShell cmdlet.</span></span> <span data-ttu-id="d795f-107">Ниже перечислены сценарии, в которых это может быть полезно.</span><span class="sxs-lookup"><span data-stu-id="d795f-107">Scenarios where this may be useful include:</span></span>  

- <span data-ttu-id="d795f-108">Выполнение импорта данных сразу для нескольких установок [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="d795f-108">Performing data import across multiple [!INCLUDE[d365fin](includes/d365fin_md.md)] installations.</span></span>
- <span data-ttu-id="d795f-109">Настройка дополнительных областей приложения для нескольких клиентов.</span><span class="sxs-lookup"><span data-stu-id="d795f-109">Configuring additional application areas for multiple customers.</span></span>  

## <a name="to-deploy-a-configuration-package-using-a-cmdlet"></a><span data-ttu-id="d795f-110">Развертывание пакета конфигурации с использованием командлета</span><span class="sxs-lookup"><span data-stu-id="d795f-110">To deploy a configuration package using a cmdlet</span></span>  

1. <span data-ttu-id="d795f-111">Подготовьте пакет служб RapidStart Services.</span><span class="sxs-lookup"><span data-stu-id="d795f-111">Prepare a RapidStart Services package.</span></span> <span data-ttu-id="d795f-112">Например, можно создать пакет для импорта определенных значений, а также имена таблиц и полей, в которые следует вставить эти значения.</span><span class="sxs-lookup"><span data-stu-id="d795f-112">For example, you can create a package to import certain values and the names of the table and the fields to insert these values into.</span></span>  
2. <span data-ttu-id="d795f-113">Установите пакет на компьютере, на котором будет выполняться командлет.</span><span class="sxs-lookup"><span data-stu-id="d795f-113">Place the package on a computer where you will run the cmdlet.</span></span>  
3. <span data-ttu-id="d795f-114">Откройте оболочку администрирования [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="d795f-114">Open the [!INCLUDE[d365fin](includes/d365fin_md.md)] administration shell.</span></span>  
4. <span data-ttu-id="d795f-115">Введите **Invoke-NAVCodeUnit** и укажите сведения, как описано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="d795f-115">Enter **Invoke-NAVCodeUnit**, and specify information similar to the following example.</span></span>  
    ```powershell  
    Invoke-NAVCodeunit -Tenant Default -CompanyName "CRONUS International Ltd." -CodeunitId 8620 -MethodName ImportRapidStartPackage -Argument "C:TEMPRS_CONFIG.rapidstart" -ServerInstance DynamicsNAV71  

    ```
<span data-ttu-id="d795f-116">Командлет импортирует пакет в каждую компанию.</span><span class="sxs-lookup"><span data-stu-id="d795f-116">The cmdlet imports the package into each company.</span></span> <span data-ttu-id="d795f-117">Пользователи могут немедленно приступить к использованию новой функции.</span><span class="sxs-lookup"><span data-stu-id="d795f-117">Users can start to use the new functionality immediately.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d795f-118">См. также</span><span class="sxs-lookup"><span data-stu-id="d795f-118">See Also</span></span>  
[<span data-ttu-id="d795f-119">Настройка новых организаций</span><span class="sxs-lookup"><span data-stu-id="d795f-119">Configure New Companies</span></span>](admin-how-to-configure-new-companies.md)  
[<span data-ttu-id="d795f-120">Применение конфигураций к новым организациям</span><span class="sxs-lookup"><span data-stu-id="d795f-120">Apply Configurations to New Companies</span></span>](admin-apply-configuration-to-new-companies.md)  
[<span data-ttu-id="d795f-121">Настройка компании с помощью служб RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="d795f-121">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="d795f-122">Администрация</span><span class="sxs-lookup"><span data-stu-id="d795f-122">Administration</span></span>](admin-setup-and-administration.md)  
[<span data-ttu-id="d795f-123">Командлеты Windows PowerShell для Microsoft Dynamics NAV</span><span class="sxs-lookup"><span data-stu-id="d795f-123">Microsoft Dynamics NAV Windows PowerShell Cmdlets</span></span>](/dynamics-nav/microsoft-dynamics-nav-windows-powershell-cmdlets)

