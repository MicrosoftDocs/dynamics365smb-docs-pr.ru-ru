---
title: Обзор строки учета финансового журнала | Документация Майкрософт
description: В этом разделе рассматриваются изменения модуля codeunit 12 **Фин. журнал - строка учета** — это основной объект приложения для учета главной книги и единственное место для вставки операций главной книги, НДС, книги поставщиков и клиентов.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: design, general ledger, post
ms.date: 06/08/2021
ms.author: edupont
ms.openlocfilehash: 1f6060eb7672b332fb570eb13fe027a3b58e6594
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/09/2021
ms.locfileid: "6215257"
---
# <a name="general-journal-post-line-overview"></a><span data-ttu-id="6be74-103">Обзор строки учета финансового журнала</span><span class="sxs-lookup"><span data-stu-id="6be74-103">General Journal Post Line Overview</span></span>

<span data-ttu-id="6be74-104">Модуль codeunit 12 **Фин. журнал - строка учета** — это основной объект приложения для учета главной книги и единственное место для вставки операций главной книги, НДС, книги поставщиков и клиентов.</span><span class="sxs-lookup"><span data-stu-id="6be74-104">Codeunit 12, **Gen. Jnl.-Post Line**, is the major application object for general ledger posting and is the only place to insert general ledger, VAT, and customer and vendor ledger entries.</span></span> <span data-ttu-id="6be74-105">Этот модуль codeunit также используется для всех операций применения, отмены применения и сторнирования.</span><span class="sxs-lookup"><span data-stu-id="6be74-105">This codeunit is also used for all Apply, Unapply and Reverse operations.</span></span>  
  
<span data-ttu-id="6be74-106">В Microsoft Dynamics NAV 2013 R2 codeunit был переработан, поскольку он стал очень большим, примерно с 7600 строками кода.</span><span class="sxs-lookup"><span data-stu-id="6be74-106">In Microsoft Dynamics NAV 2013 R2, the codeunit was redesigned because it had become very large, with approximately 7,600 code lines.</span></span> <span data-ttu-id="6be74-107">Архитектура была изменена и модуль codeunit стало проще использовать и поддерживать.</span><span class="sxs-lookup"><span data-stu-id="6be74-107">The architecture was changed and the codeunit has been made simpler and more maintainable.</span></span> <span data-ttu-id="6be74-108">Эта документация описывает изменения и содержит сведения, необходимые для обновления.</span><span class="sxs-lookup"><span data-stu-id="6be74-108">This documentation describes the changes and provides information that you will need for upgrade.</span></span>  
  
## <a name="old-architecture"></a><span data-ttu-id="6be74-109">Старая архитектура</span><span class="sxs-lookup"><span data-stu-id="6be74-109">Old Architecture</span></span>  
<span data-ttu-id="6be74-110">Старая архитектура имела следующие функции:</span><span class="sxs-lookup"><span data-stu-id="6be74-110">The old architecture had the following features:</span></span>  
  
* <span data-ttu-id="6be74-111">Глобальные переменные использовались слишком часто, что увеличивало возможность скрытых ошибок из-за неправильного использования переменных.</span><span class="sxs-lookup"><span data-stu-id="6be74-111">There was extensive use of global variables, which increased the possibility of hidden errors due to use of variables with the wrong scope.</span></span>  
* <span data-ttu-id="6be74-112">Существовало множество длинных процедур (содержащих более 100 строк кода) с высоким уровнем цикломатической сложности (т.е. частое использование вложенных операторов CASE, REPEAT и IF), из-за чего код было сложно считывать и поддерживать.</span><span class="sxs-lookup"><span data-stu-id="6be74-112">There were many long procedures (with more than 100 code lines) that also had high cyclomatic complexity (that is, a lot of CASE, REPEAT, IF nested statements), which made the code very difficult to read and maintain.</span></span>  
* <span data-ttu-id="6be74-113">Несколько процедур, которые использовались только локально и предназначались только для локального использования, не были отмечены как локальные.</span><span class="sxs-lookup"><span data-stu-id="6be74-113">Several procedures that were only used locally and were only meant to be used locally were not marked as local.</span></span>  
* <span data-ttu-id="6be74-114">В большинстве процедур отсутствовали параметры и использовались глобальные переменные.</span><span class="sxs-lookup"><span data-stu-id="6be74-114">Most procedures had no parameters and used global variables.</span></span> <span data-ttu-id="6be74-115">В некоторых процедурах использовались параметры и были переопределены глобальные переменные локальными значениями.</span><span class="sxs-lookup"><span data-stu-id="6be74-115">Some used parameters and overrode global variables with locals.</span></span>  
* <span data-ttu-id="6be74-116">Шаблоны кода для поиска счетов главной книги и создания операций НДС и главной книги не были стандартизированы и различаются в зависимости от места использования.</span><span class="sxs-lookup"><span data-stu-id="6be74-116">Code patterns for searching the general ledger accounts and creating general ledger and VAT entries was not standardized and varied from place to place.</span></span> <span data-ttu-id="6be74-117">Кроме того, часто возникает дублирование кода и нарушается симметрия между кодом клиента и поставщика.</span><span class="sxs-lookup"><span data-stu-id="6be74-117">In addition, there was a lot of code duplication and broken symmetry between customer and vendor code.</span></span>  
* <span data-ttu-id="6be74-118">Большая часть кода в модуле codeunit 12, т.е. приблизительно 30 процентов, связана с расчетами скидки оплаты и отклонения в оплате, хотя эти функции не требуются в большинстве стран или регионов.</span><span class="sxs-lookup"><span data-stu-id="6be74-118">A large part of the code in codeunit 12, approximately 30 percent, related to payment discount and tolerance calculations, although these features are not needed in many countries or regions.</span></span>  
* <span data-ttu-id="6be74-119">Функции "Учет", "Применить", "Отменить применение", "Сторнировать", "Скидка оплаты", "Отклонение в оплате" и "Коррекция валютного курса" были объединены в модуль codeunit 12 с помощью длинного списка глобальных переменных.</span><span class="sxs-lookup"><span data-stu-id="6be74-119">Posting, Apply, Unapply, Reverse, Payment Discount and Tolerance, and Exchange Rate Adjustment were married together in codeunit 12 using a long list of global variables.</span></span>  
  
### <a name="new-architecture"></a><span data-ttu-id="6be74-120">Новая архитектура</span><span class="sxs-lookup"><span data-stu-id="6be74-120">New Architecture</span></span>  
<span data-ttu-id="6be74-121">В [!INCLUDE[prod_short](includes/prod_short.md)] модуль codeunit 12 усовершенствован следующим образом:</span><span class="sxs-lookup"><span data-stu-id="6be74-121">In [!INCLUDE[prod_short](includes/prod_short.md)], codeunit 12 has had the following improvements:</span></span>  
  
* <span data-ttu-id="6be74-122">Модуль codeunit 12 был реорганизован на более мелкие процедуры (все содержат менее 100 строк кода).</span><span class="sxs-lookup"><span data-stu-id="6be74-122">Codeunit 12 has been refactored into smaller procedures (all less than 100 code lines).</span></span>  
* <span data-ttu-id="6be74-123">Стандартизированные шаблоны для поиска счетов главной книги реализованы с помощью вспомогательных функций из таблицы "Учетная группа".</span><span class="sxs-lookup"><span data-stu-id="6be74-123">Standardized patterns for the search of general ledger accounts have been implemented by using helper functions from Posting Group tables.</span></span>  
* <span data-ttu-id="6be74-124">Платформа механизма учета была реализована для управления началом и окончанием транзакций и для изолирования создания в главной книге и операциях НДС, коллекции коррекции НДС и расчета дополнительных сумм валюты.</span><span class="sxs-lookup"><span data-stu-id="6be74-124">A Posting Engine Framework has been implemented to manage the start and finish of transactions and to isolate the creation to general ledger and VAT entries, the collection of VAT adjustment, and the calculation of additional currency amounts.</span></span>  
* <span data-ttu-id="6be74-125">Дублирование кода устранено.</span><span class="sxs-lookup"><span data-stu-id="6be74-125">Code duplication has been eliminated.</span></span>  
* <span data-ttu-id="6be74-126">Множество вспомогательных функций перемещены в соответствующие таблицы и книги клиентов и поставщиков.</span><span class="sxs-lookup"><span data-stu-id="6be74-126">Many helper functions have been transferred to corresponding customer and vendor ledger entry tables.</span></span>  
* <span data-ttu-id="6be74-127">Использование глобальных переменных сведено к минимуму, чтобы в каждой процедуре использовались параметры и инкапсулировалась собственная логика применения.</span><span class="sxs-lookup"><span data-stu-id="6be74-127">The use of global variables has been minimized, so that each procedure uses parameters and encapsulates its own application logic.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="6be74-128">См. также</span><span class="sxs-lookup"><span data-stu-id="6be74-128">See Also</span></span>

[<span data-ttu-id="6be74-129">Сведения о проектировании: структура интерфейса учета</span><span class="sxs-lookup"><span data-stu-id="6be74-129">Design Details: Posting Interface Structure</span></span>](design-details-posting-interface-structure.md)  
[<span data-ttu-id="6be74-130">Сведения о проектировании: структура механизма учета</span><span class="sxs-lookup"><span data-stu-id="6be74-130">Design Details: Posting Engine Structure</span></span>](design-details-posting-engine-structure.md)  
[<span data-ttu-id="6be74-131">Сведения о проектировании: строка учета финансового журнала (Dynamics NAV)</span><span class="sxs-lookup"><span data-stu-id="6be74-131">Design Details: General Journal Post Line (Dynamics NAV)</span></span>](/dynamics-nav-app/design-details-general-journal-post-line)  


[!INCLUDE[footer-include](includes/footer-banner.md)]