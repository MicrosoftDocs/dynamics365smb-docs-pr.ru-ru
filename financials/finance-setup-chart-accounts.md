---
title: "Настройка плана счетов | Документы Майкрософт"
description: "Вы можете изменить счета по умолчанию в плане счетов и добавить новые счета."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: COA, cha of acc
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: ceb01999525139cabc7c31e2304f738dcc9267f8
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="setting-up-or-changing-the-chart-of-accounts"></a><span data-ttu-id="55ce2-103">Настройка или изменение плана счетов</span><span class="sxs-lookup"><span data-stu-id="55ce2-103">Setting Up or Changing the Chart of Accounts</span></span>
<span data-ttu-id="55ce2-104">В плане счетов отображаются счета главной книги, на которых хранятся финансовые данные.</span><span class="sxs-lookup"><span data-stu-id="55ce2-104">The chart of accounts shows the ledger accounts that store your financial data.</span></span> [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]<span data-ttu-id="55ce2-105"> включает стандартный план счетов, готовый к использованию в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="55ce2-105"> includes a standard chart of accounts that is ready to support your business.</span></span>
<span data-ttu-id="55ce2-106">Однако вы можете изменить счета по умолчанию и добавить новые счета.</span><span class="sxs-lookup"><span data-stu-id="55ce2-106">However, you can change the default accounts, and you can add new accounts.</span></span>  

## <a name="adding-or-changing-accounts"></a><span data-ttu-id="55ce2-107">Добавление или изменение счетов</span><span class="sxs-lookup"><span data-stu-id="55ce2-107">Adding or Changing Accounts</span></span>
<span data-ttu-id="55ce2-108">В плане счетов вы можете открыть каждый счет ГК и добавить или изменить параметры.</span><span class="sxs-lookup"><span data-stu-id="55ce2-108">From the chart of accounts, you can open each G/L account and add or change settings.</span></span>

> [!NOTE]  
>   <span data-ttu-id="55ce2-109">Вы можете удалить счет главной книги.</span><span class="sxs-lookup"><span data-stu-id="55ce2-109">You can delete a general ledger account.</span></span> <span data-ttu-id="55ce2-110">Однако прежде чем удалять его, должно быть соблюдено следующее:</span><span class="sxs-lookup"><span data-stu-id="55ce2-110">However, before you delete it, the following must be true:</span></span>  

* <span data-ttu-id="55ce2-111">Сальдо счета должно быть нулевым.</span><span class="sxs-lookup"><span data-stu-id="55ce2-111">The balance on the account must be zero.</span></span>  
* <span data-ttu-id="55ce2-112">В окне **Настройка Главной книги** должно быть задано поле **Разрешить удаление счета ГК до**, а на счете не должно быть операций книги в эту дату и после нее.</span><span class="sxs-lookup"><span data-stu-id="55ce2-112">The **Allow G/L Acc. Deletion Before** field must be set in the **General Ledger Setup** window, and the account must not have ledger entries on or after that date.</span></span>  
* <span data-ttu-id="55ce2-113">Если в окне **Настройка Главной книги** установлен флажок **Проверка использования счета ГК**, то счет не должен использоваться ни в одной из учетных групп или настроек учета.</span><span class="sxs-lookup"><span data-stu-id="55ce2-113">If the **Check G/L Account Usage** field in the **General Ledger Setup** window is selected, then the account must not be used in any posting groups or posting setup.</span></span>  

[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="55ce2-114"> не допускает удаления счета главной книги, на котором хранятся данные, необходимые для плана счетов.</span><span class="sxs-lookup"><span data-stu-id="55ce2-114"> will prevent you from deleting a general ledger account that stores data that is needed in the chart of accounts.</span></span>  

## <a name="see-also"></a><span data-ttu-id="55ce2-115">См. также</span><span class="sxs-lookup"><span data-stu-id="55ce2-115">See Also</span></span>
[<span data-ttu-id="55ce2-116">Главная книга и план счетов</span><span class="sxs-lookup"><span data-stu-id="55ce2-116">The General Ledger and the Chart of Accounts</span></span>](finance-general-ledger.md)  
[<span data-ttu-id="55ce2-117">Управление банковскими счетами</span><span class="sxs-lookup"><span data-stu-id="55ce2-117">Managing Bank Accounts</span></span>](bank-manage-bank-accounts.md)  
[<span data-ttu-id="55ce2-118">Работа с измерениями</span><span class="sxs-lookup"><span data-stu-id="55ce2-118">Working with Dimensions</span></span>](finance-dimensions.md)  
[<span data-ttu-id="55ce2-119">Импорт из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="55ce2-119">Importing from Other Finance Systems</span></span>](upload-data.md)  
[<span data-ttu-id="55ce2-120">Практическое руководство. Работа с кодами GIFI в Канаде</span><span class="sxs-lookup"><span data-stu-id="55ce2-120">How to: Work With GIFI Codes in Canada</span></span>](ca-finance-work-gifi-codes.md)  
<span data-ttu-id="55ce2-121">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="55ce2-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]