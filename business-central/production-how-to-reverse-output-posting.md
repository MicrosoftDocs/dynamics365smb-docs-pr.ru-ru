---
title: Практическое руководство. Сторнирование учета выхода | Документация Майкрософт
description: Бывают случаи, когда учет выхода необходимо сторнировать. Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 33be858c687381a50f42d1c59ca735358f113d72
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3788754"
---
# <a name="reverse-output-posting"></a><span data-ttu-id="8600a-104">Сторнирование учета выхода</span><span class="sxs-lookup"><span data-stu-id="8600a-104">Reverse Output Posting</span></span>
<span data-ttu-id="8600a-105">Бывают случаи, когда учет выхода необходимо сторнировать.</span><span class="sxs-lookup"><span data-stu-id="8600a-105">There are times when output posting must be reversed.</span></span> <span data-ttu-id="8600a-106">Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода.</span><span class="sxs-lookup"><span data-stu-id="8600a-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span></span>  

## <a name="to-reverse-an-output-posting"></a><span data-ttu-id="8600a-107">Сторнирование проводки по выпуску</span><span class="sxs-lookup"><span data-stu-id="8600a-107">To reverse an output posting</span></span>  
1.  <span data-ttu-id="8600a-108">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Журнал выхода продукции**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="8600a-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Output Journal**, and then choose the related link.</span></span> <span data-ttu-id="8600a-109">Выберите пакет.</span><span class="sxs-lookup"><span data-stu-id="8600a-109">Select your batch.</span></span>  
2. <span data-ttu-id="8600a-110">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="8600a-110">Fill in the fields as necessary.</span></span> <span data-ttu-id="8600a-111">Дополнительные сведения см. разделе [Учет в пакетном режиме выпуска продукции и времени работы](production-how-to-post-output-quantity.md).</span><span class="sxs-lookup"><span data-stu-id="8600a-111">For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span></span>
3.  <span data-ttu-id="8600a-112">В поле **Примен. к операции** выберите соответствующую операцию книги товаров.</span><span class="sxs-lookup"><span data-stu-id="8600a-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span></span> <span data-ttu-id="8600a-113">При этом будут сторнированы операции журналов производственных мощностей и товаров.</span><span class="sxs-lookup"><span data-stu-id="8600a-113">This reverses the capacity and item ledger entries.</span></span>  
4. <span data-ttu-id="8600a-114">Учтите сторнирование путем учета журнала.</span><span class="sxs-lookup"><span data-stu-id="8600a-114">Post the reversal by posting the journal.</span></span>  

<span data-ttu-id="8600a-115">Операции журнала выхода продукции учитываются в книге товаров как положительная корректировка.</span><span class="sxs-lookup"><span data-stu-id="8600a-115">The output journal entries are posted to the item ledger as a positive adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8600a-116">См. также</span><span class="sxs-lookup"><span data-stu-id="8600a-116">See Also</span></span>  
 <span data-ttu-id="8600a-117">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="8600a-117">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
 [<span data-ttu-id="8600a-118">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="8600a-118">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
 <span data-ttu-id="8600a-119">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="8600a-119">[Planning](production-planning.md)    </span></span>  
 [<span data-ttu-id="8600a-120">Запасы</span><span class="sxs-lookup"><span data-stu-id="8600a-120">Inventory</span></span>](inventory-manage-inventory.md)  
 [<span data-ttu-id="8600a-121">Покупки</span><span class="sxs-lookup"><span data-stu-id="8600a-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="8600a-122">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8600a-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
