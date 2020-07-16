---
title: Аудит изменений | Документация Майкрософт
description: Вы можете активизировать журнал пользователя, чтобы у вас была история всех изменений, внесенных в данные в отслеживаемых таблицах. Также можно отслеживать действия с помощью определенных типов журналов действий.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: user log, user activity, tracking
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 201716238ddd42ac19cd769a8635d726e27e1509
ms.sourcegitcommit: 3e9c89f90db5eaed599630299353300621fe4007
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "3528817"
---
# <a name="auditing-changes-in-business-central"></a><span data-ttu-id="9d8a3-104">Изменение аудита в Business Central</span><span class="sxs-lookup"><span data-stu-id="9d8a3-104">Auditing Changes in Business Central</span></span>

<span data-ttu-id="9d8a3-105">Можно включить журнал изменений в [!INCLUDE[d365fin](includes/d365fin_md.md)], чтобы иметь историю действий.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-105">You can enable the change log in [!INCLUDE[d365fin](includes/d365fin_md.md)] so you have a history of activities.</span></span> <span data-ttu-id="9d8a3-106">Журнал основывается на изменениях, внесенных в данные таблиц, по которым выполняется отслеживание. На странице **Операции журнала изменений** операции хронологически упорядочены, а также показывает изменения, примененные к полям в определенных таблицах.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-106">The log is based on changes that are made to data in the tables that you track. On the **Change Log Entries** page, entries are chronologically ordered and show changes that are made to the fields on the specified tables.</span></span> <span data-ttu-id="9d8a3-107">Журнал изменений записывает все изменения в таблице.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-107">The change log collects all changes that are made to the table.</span></span>

> [!Important]
> <span data-ttu-id="9d8a3-108">Изменения пользователя не видны на странице **Операции журнала изменений**, пока сеанс пользователя не будет перезагружен, что выполняется в следующих случаях:</span><span class="sxs-lookup"><span data-stu-id="9d8a3-108">A user's changes are not visible in the **Change Log Entries** until the user's session is restarted, which happens in the following cases:</span></span>
<br />
> * <span data-ttu-id="9d8a3-109">Срок действия сеанса завершился и сеанс был обновлен.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-109">The session expired and was refreshed.</span></span>
> * <span data-ttu-id="9d8a3-110">Пользователь выбрал другую организацию или ролевой центр.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-110">The user selected another company or Role Center.</span></span>
> * <span data-ttu-id="9d8a3-111">Пользователь выполнил выход, затем снова вход.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-111">The user signed out and back in.</span></span>

## <a name="working-with-the-change-log"></a><span data-ttu-id="9d8a3-112">Работа с журналом изменений</span><span class="sxs-lookup"><span data-stu-id="9d8a3-112">Working with the Change Log</span></span>

<span data-ttu-id="9d8a3-113">Обычной проблемой со многих финансовых системах является выявление источника происхождения ошибок и изменений в данных.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-113">A common problem in many financial systems is to locate the origin of errors and changes in data.</span></span> <span data-ttu-id="9d8a3-114">Это может быть все что угодно — от неправильно введенного номера телефона клиента, до неправильного учета в Главной книге.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-114">It could be anything from an incorrect customer telephone number to an incorrect posting to the general ledger.</span></span> <span data-ttu-id="9d8a3-115">Журнал изменений позволяет отслеживать все изменения, внесенные пользователем непосредственно в данные базы данных.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-115">The change log lets you track all direct modifications a user makes to data in the database.</span></span> <span data-ttu-id="9d8a3-116">Необходимо указать каждую таблицу и поле, которые система должна записывать в журнал, после чего следует активировать журнал изменений.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-116">You must specify each table and field that you want the system to log, and then you must activate the change log.</span></span>  

<span data-ttu-id="9d8a3-117">Можно активировать и деактивировать журнал изменений на странице **Настройка журнала изменений**.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-117">You activate and deactivate the change log on the **Change Log Setup** page.</span></span> <span data-ttu-id="9d8a3-118">Когда пользователь активирует или деактивирует журнал изменений, это действие регистрируется, чтобы всегда можно было просмотреть, какой пользователь деактивировал или повторно активировал журнал изменений.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-118">When a user activates or deactivates the change log, this activity is logged, so you can always see which user deactivated or reactivated the change log.</span></span>

<span data-ttu-id="9d8a3-119">На странице **Настройка журнала изменений**, если выбрать действие **Таблицы**, можно указать, для каких таблиц требуется отслеживать изменения и какие изменения требуется отслеживаться. [!INCLUDE[d365fin](includes/d365fin_md.md)] также отслеживает несколько системных таблиц.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-119">On the **Change Log Setup** page, if you choose the **Tables** action, you can specify which tables you want to track changes for, and which changes to track. [!INCLUDE[d365fin](includes/d365fin_md.md)] also tracks a number of system tables.</span></span>

<span data-ttu-id="9d8a3-120">После настройки журнала изменений, его активации и внесения изменений в данные можно просмотреть и отфильтровать изменения на странице **Операции журнала изменений**.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-120">After you have set up the change log, activated it, and made a change to data, you can view and filter the changes on the **Change Log Entries** page.</span></span> <span data-ttu-id="9d8a3-121">Если требуется удалить операции, это можно сделать на странице **Удалить операции журнала изменений**, в котором можно установить фильтры на основе времени и даты.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-121">If you want to delete entries, you can do that on the **Delete Change Log Entries** page, where you can set filters based on dates and time.</span></span>  

## <a name="working-with-activity-logs"></a><span data-ttu-id="9d8a3-122">Работа с журналами действий</span><span class="sxs-lookup"><span data-stu-id="9d8a3-122">Working with Activity Logs</span></span>

<span data-ttu-id="9d8a3-123">С некоторых страниц в [!INCLUDE[prodshort](includes/prodshort.md)] можно просмотреть журнал действий, в котором указаны состояние и возможные ошибки из файлов, которые вы экспортируете или импортируете в [!INCLUDE[prodshort](includes/prodshort.md)],</span><span class="sxs-lookup"><span data-stu-id="9d8a3-123">From some pages in [!INCLUDE[prodshort](includes/prodshort.md)], you can view an activity log that shows the status and any errors from files that you export from or import into [!INCLUDE[prodshort](includes/prodshort.md)].</span></span>  

<span data-ttu-id="9d8a3-124">Эта информация отображается на странице **Журнал действий** в соответствии с контекстом, из которого открыта страница.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-124">The information is displayed in the **Activity Log** page, according to the context that it is opened from.</span></span> <span data-ttu-id="9d8a3-125">Открыть ее можно, например, со страниц **Настройка службы обмена документами**, **Входящий документ**, **Учтенный счет продажи** и **Учтенная кредит-нота продажи**.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-125">You can open the window from the **Document Exchange Service Setup**, **Incoming Document**, **Posted Sales Invoice**, and **Posted Sales Credit Memo** pages, for example.</span></span> <span data-ttu-id="9d8a3-126">Вы можете очистить список записей журнала или просто удалить из него записи старше 7 дней.</span><span class="sxs-lookup"><span data-stu-id="9d8a3-126">You can empty the list of log entries, or just clear the list of entries older than 7 days.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9d8a3-127">См. также</span><span class="sxs-lookup"><span data-stu-id="9d8a3-127">See Also</span></span>
[<span data-ttu-id="9d8a3-128">Изменение базовых настроек</span><span class="sxs-lookup"><span data-stu-id="9d8a3-128">Change Basic Settings</span></span>](ui-change-basic-settings.md)  
[<span data-ttu-id="9d8a3-129">Сортировка, поиск и фильтрация</span><span class="sxs-lookup"><span data-stu-id="9d8a3-129">Sorting, Searching, and Filtering</span></span>](ui-enter-criteria-filters.md)  
[<span data-ttu-id="9d8a3-130">Поиск страниц и информации с помощью функции "Что вы хотите сделать"</span><span class="sxs-lookup"><span data-stu-id="9d8a3-130">Finding Pages and Information with Tell Me</span></span>](ui-search.md)  
<span data-ttu-id="9d8a3-131">[Назначение разрешений пользователям и группам](ui-define-granular-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="9d8a3-131">[Assign Permissions to Users and Groups](ui-define-granular-permissions.md)  </span></span>  
<span data-ttu-id="9d8a3-132">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9d8a3-132">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
