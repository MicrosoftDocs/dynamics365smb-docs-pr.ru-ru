---
title: Управление намерениями доступа к базе данных в Business Central | Документация Microsoft
description: Измените намерение доступа к базе данных для отчетов, страниц API и запросов.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/30/2020
ms.author: jswymer
ms.openlocfilehash: b46786b60d7c5799b056c49188785bd595db57ff
ms.sourcegitcommit: 866f0e6ed9df3397072b9df838e31c3a1f4b626d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2020
ms.locfileid: "3333912"
---
# <a name="managing-database-access-intent"></a><span data-ttu-id="de6f7-103">Управление намерением доступа к базе данных</span><span class="sxs-lookup"><span data-stu-id="de6f7-103">Managing Database Access Intent</span></span> 

<span data-ttu-id="de6f7-104">Как суперпользователь или администратор, вы можете изменить намерение доступа к базе данных в отчетах, страницах типа API и запросах, чтобы повысить производительность службы.</span><span class="sxs-lookup"><span data-stu-id="de6f7-104">As a super user or administrator, you can change the database access intent on reports, pages of the type API, and queries to improve performance of the service.</span></span>

## <a name="overview"></a><span data-ttu-id="de6f7-105">Обзор</span><span class="sxs-lookup"><span data-stu-id="de6f7-105">Overview</span></span>

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="de6f7-106">можно настроить на использование реплик только для чтения основной базы данных (чтение-запись).</span><span class="sxs-lookup"><span data-stu-id="de6f7-106">can be set up to use read-only replicas of the primary (read-write) database.</span></span> <span data-ttu-id="de6f7-107">Использование реплики базы данных снижает нагрузку на основную базу данных.</span><span class="sxs-lookup"><span data-stu-id="de6f7-107">Using the database replica reduces the load on the primary database.</span></span> <span data-ttu-id="de6f7-108">В некоторых случаях это также улучшит производительность при просмотре данных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="de6f7-108">In some cases, it will also improve the performance when viewing data in the client.</span></span> <span data-ttu-id="de6f7-109">Реплики полезны для объектов, таких как отчеты, запросы и страницы API, которые используются только для просмотра данных, а не для их изменения.</span><span class="sxs-lookup"><span data-stu-id="de6f7-109">Replicas are beneficial for objects, like reports, queries, and API pages, that are used for viewing data only, not modifying data.</span></span>

<span data-ttu-id="de6f7-110">Когда объекты запускаются, намерение доступа к базе данных определяет, использовать ли реплику только для чтения, если таковая имеется, или первичную базу данных.</span><span class="sxs-lookup"><span data-stu-id="de6f7-110">When objects run, the database access intent determines whether to use a read-only replica, if one is available, or the primary database.</span></span> <span data-ttu-id="de6f7-111">Отчеты, страницы API и запросы разрабатываются с предопределенным намерением доступа к базе данных (см. раздел [Свойство DatabaseAccessIntent](/dynamics365/business-central/dev-itpro/developer/properties/devenv-dataaccessintent-property)).</span><span class="sxs-lookup"><span data-stu-id="de6f7-111">Reports, API pages, and queries are developed with a predefined database access intent (see [DatabaseAccessIntent property](/dynamics365/business-central/dev-itpro/developer/properties/devenv-dataaccessintent-property)).</span></span>

<span data-ttu-id="de6f7-112">Страница **Список намерений доступа к базе данных** позволяет вам переопределить предопределенное намерение доступа к базе данных для объектов при их запуске.</span><span class="sxs-lookup"><span data-stu-id="de6f7-112">The **Database Access Intent List** page lets you override the predefined database access intent for objects when they're run.</span></span>

<span data-ttu-id="de6f7-113">В сфере баз данных эта функция обычно известна как *горизонтальное масштабирование для чтения*. Для получения дополнительной информации о горизонтальном масштабировании для чтения и намерениях доступа к данным в [!INCLUDE[prodshort](includes/prodshort.md)] см. раздел [Использование горизонтального масштабирования для чтения для улучшения производительности](/dynamics365/business-central/dev-itpro/administration/database-read-scale-out-overview) в справке [!INCLUDE[prodshort](includes/prodshort.md)] для разработчиков и администраторов.</span><span class="sxs-lookup"><span data-stu-id="de6f7-113">In database terms, this feature is commonly known as *read scale-out*. For more information about read-scale out and data access intent in [!INCLUDE[prodshort](includes/prodshort.md)], see [Utilizing Read Scale-Out for Better Performance](/dynamics365/business-central/dev-itpro/administration/database-read-scale-out-overview) in the [!INCLUDE[prodshort](includes/prodshort.md)] Developer and Administration help.</span></span>

## <a name="to-change-the-database-access-intent"></a><span data-ttu-id="de6f7-114">Изменение намерения доступа к базе данных</span><span class="sxs-lookup"><span data-stu-id="de6f7-114">To change the database access intent</span></span>

1. <span data-ttu-id="de6f7-115">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Список намерений доступа к базе данных**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="de6f7-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Database Access Intent List**, and then choose the related link.</span></span>

    <span data-ttu-id="de6f7-116">На странице перечислены все отчеты, страницы и запросы.</span><span class="sxs-lookup"><span data-stu-id="de6f7-116">The page lists all reports, pages, and queries.</span></span> <span data-ttu-id="de6f7-117">Столбец **Цель доступа** включает одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="de6f7-117">The **Access Intent** column includes one of the following values:</span></span>

    |<span data-ttu-id="de6f7-118">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="de6f7-118">**Setting**</span></span>|<span data-ttu-id="de6f7-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="de6f7-119">**Description**</span></span>|  
    |------------|-------------|  
    |<span data-ttu-id="de6f7-120">**По умолч.**</span><span class="sxs-lookup"><span data-stu-id="de6f7-120">**Default**</span></span>|<span data-ttu-id="de6f7-121">Указывает, что объект использует предопределенное намерение доступа к базе данных.</span><span class="sxs-lookup"><span data-stu-id="de6f7-121">Indicates that the object uses the predefined database access intent.</span></span>|
    |<span data-ttu-id="de6f7-122">**Разрешить запись**</span><span class="sxs-lookup"><span data-stu-id="de6f7-122">**Allow Write**</span></span>|<span data-ttu-id="de6f7-123">Устанавливает объект для использования первичной базы данных, позволяя пользователю изменять данные.</span><span class="sxs-lookup"><span data-stu-id="de6f7-123">Sets the object to use the primary database, allowing the user to modify data.</span></span>|
    |<span data-ttu-id="de6f7-124">**Только чтение**</span><span class="sxs-lookup"><span data-stu-id="de6f7-124">**Read Only**</span></span>|<span data-ttu-id="de6f7-125">Устанавливает объект для использования реплики базы данных, что означает, что пользователь может только просматривать данные, но не изменять их.</span><span class="sxs-lookup"><span data-stu-id="de6f7-125">Sets the object to use the database replica, which means that the user can only view data, not change data.</span></span>|

2. <span data-ttu-id="de6f7-126">Выберите действие **Изменить список**.</span><span class="sxs-lookup"><span data-stu-id="de6f7-126">Choose the **Edit List** action.</span></span>

3. <span data-ttu-id="de6f7-127">На странице **Изменение — список намерений доступа к базе данных** измените поле **Цель доступа** для объектов.</span><span class="sxs-lookup"><span data-stu-id="de6f7-127">On the **Edit - Database Access Intent List** page, change the **Access Intent** field for the objects.</span></span>

    > [!NOTE]
    > <span data-ttu-id="de6f7-128">Если объект, который можно редактировать, например, карточка клиента, установлен на **Только чтение**, первичная база данных будет по-прежнему использоваться, независимо от цели доступа, что позволяет пользователям вносить изменения в обычном режиме.</span><span class="sxs-lookup"><span data-stu-id="de6f7-128">If an object that is editable, like the Customer Card, is set to **Read Only**, the primary database will still be used, regardless of the access intent, allowing users to make changes as normal.</span></span>

## <a name="see-related-training-at-microsoft-learn"></a><span data-ttu-id="de6f7-129">См. соответствующее обучение на странице [Microsoft Learn](/learn/paths/deploy-configure-dynamics-365-business-central/)</span><span class="sxs-lookup"><span data-stu-id="de6f7-129">See Related Training at [Microsoft Learn](/learn/paths/deploy-configure-dynamics-365-business-central/)</span></span>

## <a name="see-also"></a><span data-ttu-id="de6f7-130">См. также</span><span class="sxs-lookup"><span data-stu-id="de6f7-130">See Also</span></span>
[<span data-ttu-id="de6f7-131">Функциональные бизнес-возможности</span><span class="sxs-lookup"><span data-stu-id="de6f7-131">Business Functionality</span></span>](across-business-functionality.md)  
[<span data-ttu-id="de6f7-132">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="de6f7-132">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="de6f7-133">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="de6f7-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="de6f7-134">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="de6f7-134">Getting Started</span></span>](product-get-started.md)    

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
