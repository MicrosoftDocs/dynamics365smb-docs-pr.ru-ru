---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7ead218d289668d893a659f730a4c64e31195f10
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5788579"
---
<span data-ttu-id="7e13e-101">При вводе даты и времени, то есть даты и времени в одном поле, необходимо оставлять пробел между датой и временем.</span><span class="sxs-lookup"><span data-stu-id="7e13e-101">When you enter datetimes, which are a date and time combined into one field, you must enter a space between the date and the time.</span></span> <span data-ttu-id="7e13e-102">Часть даты может содержать только пробелы в форме официального разделителя дат настроек региона.</span><span class="sxs-lookup"><span data-stu-id="7e13e-102">The date part can only contain spaces in the form of the official date separator of your region settings.</span></span> <span data-ttu-id="7e13e-103">Время может содержать пробелы вокруг индикатора AM/PM в соответствующих региональных настройках.</span><span class="sxs-lookup"><span data-stu-id="7e13e-103">The time can contain spaces around the AM/PM indicator in relevant regional settings.</span></span>

<!--It is also possible to enter only a date in a datetime field, but it is not possible to enter only a time.-->

<span data-ttu-id="7e13e-104">В следующей таблице представлены способы ввода даты и времени и их интерпретация.</span><span class="sxs-lookup"><span data-stu-id="7e13e-104">The following table lists the various ways in which you can enter datetimes and how they're interpreted.</span></span>  

|<span data-ttu-id="7e13e-105">Формат ввода</span><span class="sxs-lookup"><span data-stu-id="7e13e-105">Entry</span></span>|<span data-ttu-id="7e13e-106">Интерпретация</span><span class="sxs-lookup"><span data-stu-id="7e13e-106">Interpretation</span></span>|
|---------------|------------------------|
|<span data-ttu-id="7e13e-107">08-01-2022 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="7e13e-107">08-01-2022 05:48:12 PM</span></span>|<span data-ttu-id="7e13e-108">08\-01\-2022 05:48:12 PM</span><span class="sxs-lookup"><span data-stu-id="7e13e-108">08\-01\-2022 05:48:12 PM</span></span>|
|<span data-ttu-id="7e13e-109">131222 132455</span><span class="sxs-lookup"><span data-stu-id="7e13e-109">131222 132455</span></span>|<span data-ttu-id="7e13e-110">12.13.22, 13:24:55</span><span class="sxs-lookup"><span data-stu-id="7e13e-110">13-12-22 13:24:55</span></span>|
|<span data-ttu-id="7e13e-111">1-12-22 10</span><span class="sxs-lookup"><span data-stu-id="7e13e-111">1-12-22 10</span></span>|<span data-ttu-id="7e13e-112">12.01.22, 10:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-112">01-12-22 10:00:00</span></span>|
|<span data-ttu-id="7e13e-113">1.12.22 5</span><span class="sxs-lookup"><span data-stu-id="7e13e-113">1.12.22 5</span></span>|<span data-ttu-id="7e13e-114">12.01.22, 05:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-114">01-12-22 05:00:00</span></span>|
|<span data-ttu-id="7e13e-115">1.12.22</span><span class="sxs-lookup"><span data-stu-id="7e13e-115">1.12.22</span></span>|<span data-ttu-id="7e13e-116">12.01.22, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-116">01-12-22 00:00:00</span></span>|
|<span data-ttu-id="7e13e-117">11 12</span><span class="sxs-lookup"><span data-stu-id="7e13e-117">11 12</span></span>|<span data-ttu-id="7e13e-118">11-е число текущего месяца и года, 12:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-118">11-current month-current year 12:00:00</span></span>|
|<span data-ttu-id="7e13e-119">1112 12</span><span class="sxs-lookup"><span data-stu-id="7e13e-119">1112 12</span></span>|<span data-ttu-id="7e13e-120">11 декабря текущего года, 12:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-120">11-12-current year 12:00:00</span></span>|
|<span data-ttu-id="7e13e-121">t или сегодня</span><span class="sxs-lookup"><span data-stu-id="7e13e-121">t or today</span></span>|<span data-ttu-id="7e13e-122">текущая дата, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-122">today's date 00:00:00</span></span>|
|<span data-ttu-id="7e13e-123">t время</span><span class="sxs-lookup"><span data-stu-id="7e13e-123">t time</span></span>|<span data-ttu-id="7e13e-124">текущая дата, фактическое время</span><span class="sxs-lookup"><span data-stu-id="7e13e-124">today's date actual time</span></span>|
|<span data-ttu-id="7e13e-125">с 10:30</span><span class="sxs-lookup"><span data-stu-id="7e13e-125">t 10:30</span></span>|<span data-ttu-id="7e13e-126">текущая дата, 10:30:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-126">today's date 10:30:00</span></span>|
|<span data-ttu-id="7e13e-127">с 3:3:3</span><span class="sxs-lookup"><span data-stu-id="7e13e-127">t 3:3:3</span></span>|<span data-ttu-id="7e13e-128">текущая дата, 03:03:03</span><span class="sxs-lookup"><span data-stu-id="7e13e-128">today's date 03:03:03</span></span>|
|<span data-ttu-id="7e13e-129">w или рабочая дата</span><span class="sxs-lookup"><span data-stu-id="7e13e-129">w or workdate</span></span>|<span data-ttu-id="7e13e-130">рабочая дата, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-130">the working date 00:00:00</span></span>|
|<span data-ttu-id="7e13e-131">m или понедельник</span><span class="sxs-lookup"><span data-stu-id="7e13e-131">m or Monday</span></span>|<span data-ttu-id="7e13e-132">понедельник текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-132">Monday of the current week 00:00:00</span></span>|
|<span data-ttu-id="7e13e-133">tu или вторник</span><span class="sxs-lookup"><span data-stu-id="7e13e-133">tu or Tuesday</span></span>|<span data-ttu-id="7e13e-134">вторник текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-134">Tuesday of the current week 00:00:00</span></span>|
|<span data-ttu-id="7e13e-135">we или среда</span><span class="sxs-lookup"><span data-stu-id="7e13e-135">we or Wednesday</span></span>|<span data-ttu-id="7e13e-136">среда текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-136">Wednesday of the current week 00:00:00</span></span>|
|<span data-ttu-id="7e13e-137">th или четверг</span><span class="sxs-lookup"><span data-stu-id="7e13e-137">th or Thursday</span></span>|<span data-ttu-id="7e13e-138">четверг текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-138">Thursday of the current week 00:00:00</span></span>|
|<span data-ttu-id="7e13e-139">f или пятница</span><span class="sxs-lookup"><span data-stu-id="7e13e-139">f or Friday</span></span>|<span data-ttu-id="7e13e-140">пятница текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-140">Friday of the current week 00:00:00</span></span>|
|<span data-ttu-id="7e13e-141">s или суббота</span><span class="sxs-lookup"><span data-stu-id="7e13e-141">s or Saturday</span></span>|<span data-ttu-id="7e13e-142">суббота текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-142">Saturday of the current week 00:00:00</span></span>|
|<span data-ttu-id="7e13e-143">su или воскресенье</span><span class="sxs-lookup"><span data-stu-id="7e13e-143">su or Sunday</span></span>|<span data-ttu-id="7e13e-144">воскресенье текущей недели, 00:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-144">Sunday of the current week 00:00:00</span></span>|
|<span data-ttu-id="7e13e-145">вт10:30</span><span class="sxs-lookup"><span data-stu-id="7e13e-145">tu 10:30</span></span>|<span data-ttu-id="7e13e-146">вторник текущей недели, 10:30:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-146">Tuesday of the current week 10:30:00</span></span>|
|<span data-ttu-id="7e13e-147">вт 3:3:3</span><span class="sxs-lookup"><span data-stu-id="7e13e-147">tu 3:3:3</span></span>|<span data-ttu-id="7e13e-148">вторник текущей недели, 03:03:03</span><span class="sxs-lookup"><span data-stu-id="7e13e-148">Tuesday of the current week 03:03:03</span></span>|
|<span data-ttu-id="7e13e-149">в23 в</span><span class="sxs-lookup"><span data-stu-id="7e13e-149">t23 t</span></span>|<span data-ttu-id="7e13e-150">Вторник недели 23 года рабочей даты, текущее время дня</span><span class="sxs-lookup"><span data-stu-id="7e13e-150">Tuesday of week 23 of the work date year, current time of day</span></span>|
|<span data-ttu-id="7e13e-151">в23</span><span class="sxs-lookup"><span data-stu-id="7e13e-151">t23</span></span>|<span data-ttu-id="7e13e-152">Вторник недели 23 года рабочей даты</span><span class="sxs-lookup"><span data-stu-id="7e13e-152">Tuesday of week 23 of the work date year</span></span>|
|<span data-ttu-id="7e13e-153">в 23</span><span class="sxs-lookup"><span data-stu-id="7e13e-153">t 23</span></span>|<span data-ttu-id="7e13e-154">Сегодня 23:00:00</span><span class="sxs-lookup"><span data-stu-id="7e13e-154">Today 23:00:00</span></span>|
|<span data-ttu-id="7e13e-155">в-1</span><span class="sxs-lookup"><span data-stu-id="7e13e-155">t-1</span></span>|<span data-ttu-id="7e13e-156">Вторник недели 1 года рабочей даты</span><span class="sxs-lookup"><span data-stu-id="7e13e-156">Tuesday of week 1 of the work date year</span></span>|


