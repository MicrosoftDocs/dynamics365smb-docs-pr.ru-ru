---
title: Практическое руководство. Сторнирование учета выхода | Документация Майкрософт
description: Бывают случаи, когда учет выхода необходимо сторнировать. Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 5901ad209149c113497d676a5c86379fc8424a0e
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5392753"
---
# <a name="reverse-output-posting"></a><span data-ttu-id="21919-104">Сторнирование учета выхода</span><span class="sxs-lookup"><span data-stu-id="21919-104">Reverse Output Posting</span></span>
<span data-ttu-id="21919-105">Бывают случаи, когда учет выхода необходимо сторнировать.</span><span class="sxs-lookup"><span data-stu-id="21919-105">There are times when output posting must be reversed.</span></span> <span data-ttu-id="21919-106">Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода.</span><span class="sxs-lookup"><span data-stu-id="21919-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span></span>  

## <a name="to-reverse-an-output-posting"></a><span data-ttu-id="21919-107">Сторнирование проводки по выпуску</span><span class="sxs-lookup"><span data-stu-id="21919-107">To reverse an output posting</span></span>  
1.  <span data-ttu-id="21919-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал выхода продукции**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="21919-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.</span></span> <span data-ttu-id="21919-109">Выберите пакет.</span><span class="sxs-lookup"><span data-stu-id="21919-109">Select your batch.</span></span>  
2. <span data-ttu-id="21919-110">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="21919-110">Fill in the fields as necessary.</span></span> <span data-ttu-id="21919-111">Дополнительные сведения см. разделе [Учет в пакетном режиме выпуска продукции и времени работы](production-how-to-post-output-quantity.md).</span><span class="sxs-lookup"><span data-stu-id="21919-111">For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span></span>
3.  <span data-ttu-id="21919-112">В поле **Примен. к операции** выберите соответствующую операцию книги товаров.</span><span class="sxs-lookup"><span data-stu-id="21919-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span></span> <span data-ttu-id="21919-113">При этом будут сторнированы операции журналов производственных мощностей и товаров.</span><span class="sxs-lookup"><span data-stu-id="21919-113">This reverses the capacity and item ledger entries.</span></span>  
4. <span data-ttu-id="21919-114">Учтите сторнирование путем учета журнала.</span><span class="sxs-lookup"><span data-stu-id="21919-114">Post the reversal by posting the journal.</span></span>  

<span data-ttu-id="21919-115">Операции журнала выхода продукции учитываются в книге товаров как положительная корректировка.</span><span class="sxs-lookup"><span data-stu-id="21919-115">The output journal entries are posted to the item ledger as a positive adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="21919-116">См. также</span><span class="sxs-lookup"><span data-stu-id="21919-116">See Also</span></span>  
 <span data-ttu-id="21919-117">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="21919-117">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
 [<span data-ttu-id="21919-118">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="21919-118">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
 <span data-ttu-id="21919-119">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="21919-119">[Planning](production-planning.md)    </span></span>  
 [<span data-ttu-id="21919-120">Запасы</span><span class="sxs-lookup"><span data-stu-id="21919-120">Inventory</span></span>](inventory-manage-inventory.md)  
 [<span data-ttu-id="21919-121">Покупки</span><span class="sxs-lookup"><span data-stu-id="21919-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="21919-122">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="21919-122">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>  


[!INCLUDE[footer-include](includes/footer-banner.md)]