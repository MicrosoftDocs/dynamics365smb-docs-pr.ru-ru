---
title: Просмотр информации о таблицах
description: Узнайте, как просмотреть информацию о любых таблицах базы данных прямо из клиентского интерфейса в Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: 72e220aa310515c665ce85bd43f4ebd3aac157d0
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3922271"
---
# <a name="viewing-table-information"></a><span data-ttu-id="ff82e-103">Просмотр информации о таблицах</span><span class="sxs-lookup"><span data-stu-id="ff82e-103">Viewing Table Information</span></span>

<span data-ttu-id="ff82e-104">Страница **8700 Сведения о таблице** содержит информацию обо всех системных и бизнес-таблицах в решении Business Central.</span><span class="sxs-lookup"><span data-stu-id="ff82e-104">The page **8700 Table Information** provides information about all system and business tables in a Business Central solution.</span></span> <span data-ttu-id="ff82e-105">В частности, на этой странице отображается информация о количестве данных, содержащихся в таблицах.</span><span class="sxs-lookup"><span data-stu-id="ff82e-105">In particular, the page displays information about the amount of data the tables contain.</span></span>

<span data-ttu-id="ff82e-106">Эта информация может быть полезна для устранения проблем с производительностью, потому позволяет увидеть распределение объема данных по таблицам.</span><span class="sxs-lookup"><span data-stu-id="ff82e-106">This information is useful for troubleshooting performance problems, because let's you see the distribution of data size across tables.</span></span>

## <a name="viewing-table-information"></a><span data-ttu-id="ff82e-107">Просмотр информации о таблицах</span><span class="sxs-lookup"><span data-stu-id="ff82e-107">Viewing table information</span></span>

<span data-ttu-id="ff82e-108">Чтобы открыть эту страницу, выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Сведения о таблице**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ff82e-108">To open this page, select the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Table Information**, and then choose the related link.</span></span>

<span data-ttu-id="ff82e-109">В следующей таблице показано, какая именно информация предоставляется по каждой таблице:</span><span class="sxs-lookup"><span data-stu-id="ff82e-109">The following table describes the information provided for each table:</span></span>

|<span data-ttu-id="ff82e-110">Столбец</span><span class="sxs-lookup"><span data-stu-id="ff82e-110">Column</span></span>|<span data-ttu-id="ff82e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ff82e-111">Description</span></span>|
|------|-----------|
|<span data-ttu-id="ff82e-112">Название организации</span><span class="sxs-lookup"><span data-stu-id="ff82e-112">Company Name</span></span>|<span data-ttu-id="ff82e-113">Название организации, к которой относится таблица (если таблица относится к какой-либо организации).</span><span class="sxs-lookup"><span data-stu-id="ff82e-113">The name of the company, if any, that the table belongs to.</span></span>|
|<span data-ttu-id="ff82e-114">Название таблицы</span><span class="sxs-lookup"><span data-stu-id="ff82e-114">Table Name</span></span>|<span data-ttu-id="ff82e-115">Название таблицы.</span><span class="sxs-lookup"><span data-stu-id="ff82e-115">The name of the table.</span></span>|
|<span data-ttu-id="ff82e-116">Номер таблицы</span><span class="sxs-lookup"><span data-stu-id="ff82e-116">Table No.</span></span>|<span data-ttu-id="ff82e-117">Идентификатор таблицы.</span><span class="sxs-lookup"><span data-stu-id="ff82e-117">The ID of the table</span></span>|
|<span data-ttu-id="ff82e-118">Кол-во</span><span class="sxs-lookup"><span data-stu-id="ff82e-118">No.</span></span> <span data-ttu-id="ff82e-119">записей</span><span class="sxs-lookup"><span data-stu-id="ff82e-119">of Records</span></span>|<span data-ttu-id="ff82e-120">ОБщее количество записей, хранящихся в таблице.</span><span class="sxs-lookup"><span data-stu-id="ff82e-120">The total number of records stored in the table.</span></span>|
|<span data-ttu-id="ff82e-121">Размер записи</span><span class="sxs-lookup"><span data-stu-id="ff82e-121">Record Size</span></span>|<span data-ttu-id="ff82e-122">Средний размер записи в килобайтах.</span><span class="sxs-lookup"><span data-stu-id="ff82e-122">The average record size in KB/record.</span></span> <span data-ttu-id="ff82e-123">Значение рассчитывается по следующей формуле: 1024(Размер)/(Кол-во</span><span class="sxs-lookup"><span data-stu-id="ff82e-123">The value is calculated using the following formula: 1024(Size)/(No.</span></span> <span data-ttu-id="ff82e-124">записей).</span><span class="sxs-lookup"><span data-stu-id="ff82e-124">of Records)\`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="ff82e-125">См. также</span><span class="sxs-lookup"><span data-stu-id="ff82e-125">See Also</span></span>

[<span data-ttu-id="ff82e-126">Инспекция страниц</span><span class="sxs-lookup"><span data-stu-id="ff82e-126">Inspecting Pages</span></span>](across-inspect-page.md)  
[<span data-ttu-id="ff82e-127">Статьи о производительности для разработчиков</span><span class="sxs-lookup"><span data-stu-id="ff82e-127">Performance Articles For Developers</span></span>](/dynamics365/business-central/dev-itpro/performance/performance-developer)  
