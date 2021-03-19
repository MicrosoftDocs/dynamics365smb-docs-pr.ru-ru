---
title: Настройка плана счетов
description: Вы можете изменить счета по умолчанию в плане счетов и добавить новые счета.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: COA, cha of acc
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: f14859a641ddf6368a213f396a111a3423f49c4a
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5377116"
---
# <a name="setting-up-or-changing-the-chart-of-accounts"></a><span data-ttu-id="2f112-103">Настройка или изменение плана счетов</span><span class="sxs-lookup"><span data-stu-id="2f112-103">Setting Up or Changing the Chart of Accounts</span></span>
<span data-ttu-id="2f112-104">В плане счетов отображаются счета главной книги, на которых хранятся финансовые данные.</span><span class="sxs-lookup"><span data-stu-id="2f112-104">The chart of accounts shows the ledger accounts that store your financial data.</span></span> [!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="2f112-105">включает стандартный план счетов, готовый к использованию в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="2f112-105">includes a standard chart of accounts that is ready to support your business.</span></span>
<span data-ttu-id="2f112-106">Однако вы можете изменить счета по умолчанию и добавить новые счета.</span><span class="sxs-lookup"><span data-stu-id="2f112-106">However, you can change the default accounts, and you can add new accounts.</span></span>
<br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE43KO9?rel=0]


## <a name="adding-or-changing-accounts"></a><span data-ttu-id="2f112-107">Добавление или изменение счетов</span><span class="sxs-lookup"><span data-stu-id="2f112-107">Adding or Changing Accounts</span></span>
<span data-ttu-id="2f112-108">В плане счетов вы можете открыть каждый счет ГК и добавить или изменить параметры.</span><span class="sxs-lookup"><span data-stu-id="2f112-108">From the chart of accounts, you can open each G/L account and add or change settings.</span></span>

> [!NOTE]  
>   <span data-ttu-id="2f112-109">Вы можете удалить счет главной книги.</span><span class="sxs-lookup"><span data-stu-id="2f112-109">You can delete a general ledger account.</span></span> <span data-ttu-id="2f112-110">Однако прежде чем удалять его, должно быть соблюдено следующее:</span><span class="sxs-lookup"><span data-stu-id="2f112-110">However, before you delete it, the following must be true:</span></span>  
>  
>   * <span data-ttu-id="2f112-111">Сальдо счета должно быть нулевым.</span><span class="sxs-lookup"><span data-stu-id="2f112-111">The balance on the account must be zero.</span></span>  
>   * <span data-ttu-id="2f112-112">На странице **Настройка Главной книги** должно быть задано поле **Разрешить удаление счета ГК до**, а на счете не должно быть операций книги в эту дату и после нее.</span><span class="sxs-lookup"><span data-stu-id="2f112-112">The **Allow G/L Acc. Deletion Before** field must be set on the **General Ledger Setup** page, and the account must not have ledger entries on or after that date.</span></span>  
>   * <span data-ttu-id="2f112-113">Если на странице **Настройка Главной книги** установлен флажок **Проверка использования счета ГК**, то счет не должен использоваться ни в одной из учетных групп или настроек учета.</span><span class="sxs-lookup"><span data-stu-id="2f112-113">If the **Check G/L Account Usage** field on the **General Ledger Setup** page is selected, then the account must not be used in any posting groups or posting setup.</span></span>  

[!INCLUDE[prod_short](includes/prod_short.md)] <span data-ttu-id="2f112-114">не допускает удаления счета главной книги, на котором хранятся данные, необходимые для плана счетов.</span><span class="sxs-lookup"><span data-stu-id="2f112-114">will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span></span>  

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="2f112-115">См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/chart-accounts-dynamics-365-business-central/index)</span><span class="sxs-lookup"><span data-stu-id="2f112-115">See Related Training at [Microsoft Learn](/learn/modules/chart-accounts-dynamics-365-business-central/index)</span></span>

## <a name="see-also"></a><span data-ttu-id="2f112-116">См. также</span><span class="sxs-lookup"><span data-stu-id="2f112-116">See Also</span></span>
[<span data-ttu-id="2f112-117">Главная книга и план счетов</span><span class="sxs-lookup"><span data-stu-id="2f112-117">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
[<span data-ttu-id="2f112-118">Выверка банковских счетов</span><span class="sxs-lookup"><span data-stu-id="2f112-118">Reconciling Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="2f112-119">Работа с измерениями</span><span class="sxs-lookup"><span data-stu-id="2f112-119">Working with Dimensions</span></span>](finance-dimensions.md)  
[<span data-ttu-id="2f112-120">Импорт данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="2f112-120">Importing Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
[<span data-ttu-id="2f112-121">Работа с финансовыми отчетами</span><span class="sxs-lookup"><span data-stu-id="2f112-121">Work with Account Schedules</span></span>](bi-how-work-account-schedule.md)  
<span data-ttu-id="2f112-122">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2f112-122">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]


[!INCLUDE[footer-include](includes/footer-banner.md)]