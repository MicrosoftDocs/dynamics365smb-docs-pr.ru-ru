---
title: "Отслеживание действий пользователей в журнале изменений | Документы Майкрософт"
description: "Вы можете активизировать журнал пользователя, чтобы у вас была история всех изменений, внесенных в данные в отслеживаемых таблицах."
author: edupont04
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 11/14/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 3f158d7ed56445d6d2acf2ef8e5e9ab8e7487531
ms.openlocfilehash: bd0751ad5a4c0c7d9c3f7d5621bb7e6a62c3be2a
ms.contentlocale: ru-ru
ms.lasthandoff: 12/04/2018

---
# <a name="logging-changes-in-business-central"></a><span data-ttu-id="5a22a-103">Изменение ведения журналов в Business Central</span><span class="sxs-lookup"><span data-stu-id="5a22a-103">Logging Changes in Business Central</span></span>

<span data-ttu-id="5a22a-104">Можно включить журнал изменений в [!INCLUDE[d365fin](includes/d365fin_md.md)], чтобы иметь историю действий.</span><span class="sxs-lookup"><span data-stu-id="5a22a-104">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span></span> <span data-ttu-id="5a22a-105">Журнал основывается на изменениях, внесенных в данные таблиц, по которым выполняется отслеживание. На странице **Операции журнала изменений** операции хронологически упорядочены, а также показывает изменения, примененные к полям в определенных таблицах.</span><span class="sxs-lookup"><span data-stu-id="5a22a-105">The log is based on changes that are made to data in the tables that you track. On the **Change Log Entries** page, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span></span> <span data-ttu-id="5a22a-106">Журнал изменений записывает все изменения в таблице.</span><span class="sxs-lookup"><span data-stu-id="5a22a-106">The change log collects all changes that are made to the table.</span></span>

> [!Important]
> <span data-ttu-id="5a22a-107">Изменения пользователя не видны на странице **Операции журнала изменений**, пока сеанс пользователя не будет перезагружен, что выполняется в следующих случаях:</span><span class="sxs-lookup"><span data-stu-id="5a22a-107">A user's changes are not visible in the **Change Log Entries** until the user's session is restarted, which happens in the following cases:</span></span>
<br />
> * <span data-ttu-id="5a22a-108">Срок действия сеанса завершился и сеанс был обновлен.</span><span class="sxs-lookup"><span data-stu-id="5a22a-108">The session expired and was refreshed.</span></span>
> * <span data-ttu-id="5a22a-109">Пользователь выбрал другую организацию или ролевой центр.</span><span class="sxs-lookup"><span data-stu-id="5a22a-109">The user selected another company or Role Center.</span></span>
> * <span data-ttu-id="5a22a-110">Пользователь выполнил выход, затем снова вход.</span><span class="sxs-lookup"><span data-stu-id="5a22a-110">The user signed out and back in.</span></span>

## <a name="working-with-the-change-log"></a><span data-ttu-id="5a22a-111">Работа с журналом изменений</span><span class="sxs-lookup"><span data-stu-id="5a22a-111">Working with the Change Log</span></span>

<span data-ttu-id="5a22a-112">Обычной проблемой со многих финансовых системах является выявление источника происхождения ошибок и изменений в данных.</span><span class="sxs-lookup"><span data-stu-id="5a22a-112">A common problem in many financial systems is to locate the origin of errors and changes in data.</span></span> <span data-ttu-id="5a22a-113">Это может быть все что угодно — от неправильно введенного номера телефона клиента, до неправильного учета в Главной книге.</span><span class="sxs-lookup"><span data-stu-id="5a22a-113">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span></span> <span data-ttu-id="5a22a-114">Журнал изменений позволяет отслеживать все изменения, внесенные пользователем непосредственно в данные базы данных.</span><span class="sxs-lookup"><span data-stu-id="5a22a-114">The change log lets you track all direct modifications a user makes to data in the database.</span></span> <span data-ttu-id="5a22a-115">Необходимо указать каждую таблицу и поле, которые система должна записывать в журнал, после чего следует активировать журнал изменений.</span><span class="sxs-lookup"><span data-stu-id="5a22a-115">You must specify each table and field that you want the system to log, and then you must activate the change log.</span></span>  

<span data-ttu-id="5a22a-116">Можно активировать и деактивировать журнал изменений на странице **Настройка журнала изменений**.</span><span class="sxs-lookup"><span data-stu-id="5a22a-116">You activate and deactivate the change log on the **Change Log Setup** page.</span></span> <span data-ttu-id="5a22a-117">Когда пользователь активирует или деактивирует журнал изменений, это действие регистрируется, чтобы всегда можно было просмотреть, какой пользователь деактивировал или повторно активировал журнал изменений.</span><span class="sxs-lookup"><span data-stu-id="5a22a-117">When a user activates or deactivates the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span></span>

<span data-ttu-id="5a22a-118">На странице **Настройка журнала изменений**, если выбрать действие **Таблицы**, можно указать, для каких таблиц требуется отслеживать изменения и какие изменения требуется отслеживаться. [!INCLUDE[d365fin](includes/d365fin_md.md)] также отслеживает несколько системных таблиц.</span><span class="sxs-lookup"><span data-stu-id="5a22a-118">On the **Change Log Setup** page, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span></span>

<span data-ttu-id="5a22a-119">После настройки журнала изменений, его активации и внесения изменений в данные можно просмотреть и отфильтровать изменения на странице **Операции журнала изменений**.</span><span class="sxs-lookup"><span data-stu-id="5a22a-119">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes on the **Change Log Entries** page.</span></span> <span data-ttu-id="5a22a-120">Если требуется удалить операции, это можно сделать на странице **Удалить операции журнала изменений**, в котором можно установить фильтры на основе времени и даты.</span><span class="sxs-lookup"><span data-stu-id="5a22a-120">If you want to delete entries, you can do that on the **Delete Change Log Entries** page, where you can set filters based on dates and time.</span></span>  

## <a name="see-also"></a><span data-ttu-id="5a22a-121">См. также</span><span class="sxs-lookup"><span data-stu-id="5a22a-121">See Also</span></span>
[<span data-ttu-id="5a22a-122">Изменение базовых настроек</span><span class="sxs-lookup"><span data-stu-id="5a22a-122">Changing Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="5a22a-123">Сортировка</span><span class="sxs-lookup"><span data-stu-id="5a22a-123">Sorting</span></span>](ui-sorting.md)  
[<span data-ttu-id="5a22a-124">Использование поиска страницы или отчета</span><span class="sxs-lookup"><span data-stu-id="5a22a-124">Using Search for Page or Report</span></span>](ui-search.md)  
<span data-ttu-id="5a22a-125">[Управление пользователями и разрешениями](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="5a22a-125">[Managing Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="5a22a-126">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5a22a-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

