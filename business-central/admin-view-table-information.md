---
title: Просмотр информации о таблицах
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/20/2020
ms.author: jswymer
ms.openlocfilehash: de93063a60e6b64405b1491a67489c8bfa4657ad
ms.sourcegitcommit: 99915b493a7e49d12c530f2f9fda1fcedb518b6e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/21/2020
ms.locfileid: "3275322"
---
# <a name="viewing-table-information"></a><span data-ttu-id="a8122-102">Просмотр информации о таблицах</span><span class="sxs-lookup"><span data-stu-id="a8122-102">Viewing Table Information</span></span>

<span data-ttu-id="a8122-103">Страница **8700 Сведения о таблице** содержит информацию обо всех системных и бизнес-таблицах в решении Business Central.</span><span class="sxs-lookup"><span data-stu-id="a8122-103">The page **8700 Table Information** provides information about all system and business tables in a Business Central solution.</span></span> <span data-ttu-id="a8122-104">В частности, на этой странице отображается информация о количестве данных, содержащихся в таблицах.</span><span class="sxs-lookup"><span data-stu-id="a8122-104">In particular, the page displays information about the amount of data the tables contain.</span></span>

<span data-ttu-id="a8122-105">Эта информация может быть полезна для устранения проблем с производительностью, потому позволяет увидеть распределение объема данных по таблицам.</span><span class="sxs-lookup"><span data-stu-id="a8122-105">This information is useful for troubleshooting performance problems, because let's you see the distribution of data size across tables.</span></span>

## <a name="viewing-table-information"></a><span data-ttu-id="a8122-106">Просмотр информации о таблицах</span><span class="sxs-lookup"><span data-stu-id="a8122-106">Viewing table information</span></span>

<span data-ttu-id="a8122-107">Чтобы открыть эту страницу, выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Сведения о таблице**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="a8122-107">To open this page, select the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Table Information**, and then choose the related link.</span></span>

<span data-ttu-id="a8122-108">В следующей таблице показано, какая именно информация предоставляется по каждой таблице:</span><span class="sxs-lookup"><span data-stu-id="a8122-108">The following table describes the information provided for each table:</span></span>

|<span data-ttu-id="a8122-109">Столбец</span><span class="sxs-lookup"><span data-stu-id="a8122-109">Column</span></span>|<span data-ttu-id="a8122-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a8122-110">Description</span></span>|
|------|-----------|
|<span data-ttu-id="a8122-111">Название организации</span><span class="sxs-lookup"><span data-stu-id="a8122-111">Company Name</span></span>|<span data-ttu-id="a8122-112">Название организации, к которой относится таблица (если таблица относится к какой-либо организации).</span><span class="sxs-lookup"><span data-stu-id="a8122-112">The name of the company, if any, that the table belongs to.</span></span>|
|<span data-ttu-id="a8122-113">Название таблицы</span><span class="sxs-lookup"><span data-stu-id="a8122-113">Table Name</span></span>|<span data-ttu-id="a8122-114">Название таблицы.</span><span class="sxs-lookup"><span data-stu-id="a8122-114">The name of the table.</span></span>|
|<span data-ttu-id="a8122-115">Номер таблицы</span><span class="sxs-lookup"><span data-stu-id="a8122-115">Table No.</span></span>|<span data-ttu-id="a8122-116">Идентификатор таблицы.</span><span class="sxs-lookup"><span data-stu-id="a8122-116">The ID of the table</span></span>|
|<span data-ttu-id="a8122-117">Кол-во</span><span class="sxs-lookup"><span data-stu-id="a8122-117">No.</span></span> <span data-ttu-id="a8122-118">записей</span><span class="sxs-lookup"><span data-stu-id="a8122-118">of Records</span></span>|<span data-ttu-id="a8122-119">ОБщее количество записей, хранящихся в таблице.</span><span class="sxs-lookup"><span data-stu-id="a8122-119">The total number of records stored in the table.</span></span>|
|<span data-ttu-id="a8122-120">Размер записи</span><span class="sxs-lookup"><span data-stu-id="a8122-120">Record Size</span></span>|<span data-ttu-id="a8122-121">Средний размер записи в килобайтах.</span><span class="sxs-lookup"><span data-stu-id="a8122-121">The average record size in KB/record.</span></span> <span data-ttu-id="a8122-122">Значение рассчитывается по следующей формуле: 1024(Размер)/(Кол-во</span><span class="sxs-lookup"><span data-stu-id="a8122-122">The value is calculated using the following formula: 1024(Size)/(No.</span></span> <span data-ttu-id="a8122-123">записей).</span><span class="sxs-lookup"><span data-stu-id="a8122-123">of Records)\`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="a8122-124">См. также</span><span class="sxs-lookup"><span data-stu-id="a8122-124">See Also</span></span>

[<span data-ttu-id="a8122-125">Инспекция страниц</span><span class="sxs-lookup"><span data-stu-id="a8122-125">Inspecting Pages</span></span>](across-inspect-page.md)  
[<span data-ttu-id="a8122-126">Статьи о производительности для разработчиков</span><span class="sxs-lookup"><span data-stu-id="a8122-126">Performance Articles For Developers</span></span>](/dynamics365/business-central/dev-itpro/performance/performance-developer)  
