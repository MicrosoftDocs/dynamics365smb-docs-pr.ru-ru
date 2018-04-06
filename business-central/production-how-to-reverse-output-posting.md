---
title: "Практическое руководство. Сторнирование учета выхода | Документы Майкрософт"
description: "Бывают случаи, когда учет выхода необходимо сторнировать. Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f2430dcf45303e04baad406880783ab0f74dd4f2
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="reverse-output-posting"></a><span data-ttu-id="e899d-104">Сторнирование учета выхода</span><span class="sxs-lookup"><span data-stu-id="e899d-104">Reverse Output Posting</span></span>
<span data-ttu-id="e899d-105">Бывают случаи, когда учет выхода необходимо сторнировать.</span><span class="sxs-lookup"><span data-stu-id="e899d-105">There are times when output posting must be reversed.</span></span> <span data-ttu-id="e899d-106">Например, если произошла ошибка при вводе данных и в производственном заказе учтено неверное количество выхода.</span><span class="sxs-lookup"><span data-stu-id="e899d-106">An example of this would be if a data entry error occurred and an incorrect amount of output is posted to a production order.</span></span>  

## <a name="to-reverse-an-output-posting"></a><span data-ttu-id="e899d-107">Сторнирование проводки по выпуску</span><span class="sxs-lookup"><span data-stu-id="e899d-107">To reverse an output posting</span></span>  
1.  <span data-ttu-id="e899d-108">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Журнал выхода продукции**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="e899d-108">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Output Journal**, and then choose the related link.</span></span> <span data-ttu-id="e899d-109">Выберите пакет.</span><span class="sxs-lookup"><span data-stu-id="e899d-109">Select your batch.</span></span>  
2. <span data-ttu-id="e899d-110">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="e899d-110">Fill in the fields as necessary.</span></span> <span data-ttu-id="e899d-111">Дополнительные сведения см. разделе [Учет в пакетном режиме выпуска продукции и времени работы](production-how-to-post-output-quantity.md).</span><span class="sxs-lookup"><span data-stu-id="e899d-111">For more information, see [Batch Post Output and Run Times](production-how-to-post-output-quantity.md).</span></span>
3.  <span data-ttu-id="e899d-112">В поле **Примен. к операции** выберите соответствующую операцию книги товаров.</span><span class="sxs-lookup"><span data-stu-id="e899d-112">In the **Applies-To Entry** field, select the associated item ledger entry.</span></span> <span data-ttu-id="e899d-113">При этом будут сторнированы операции журналов производственных мощностей и товаров.</span><span class="sxs-lookup"><span data-stu-id="e899d-113">This reverses the capacity and item ledger entries.</span></span>  
4. <span data-ttu-id="e899d-114">Учтите сторнирование путем учета журнала.</span><span class="sxs-lookup"><span data-stu-id="e899d-114">Post the reversal by posting the journal.</span></span>  

<span data-ttu-id="e899d-115">Операции журнала выхода продукции учитываются в книге товаров как положительная корректировка.</span><span class="sxs-lookup"><span data-stu-id="e899d-115">The output journal entries are posted to the item ledger as a positive adjustment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e899d-116">См. также</span><span class="sxs-lookup"><span data-stu-id="e899d-116">See Also</span></span>  
 <span data-ttu-id="e899d-117">[Производство](production-manage-manufacturing.md)  </span><span class="sxs-lookup"><span data-stu-id="e899d-117">[Manufacturing](production-manage-manufacturing.md)  </span></span>  
 [<span data-ttu-id="e899d-118">Настройка производства</span><span class="sxs-lookup"><span data-stu-id="e899d-118">Setting Up Manufacturing</span></span>](production-configure-production-processes.md)  
 <span data-ttu-id="e899d-119">[Планирование](production-planning.md)    </span><span class="sxs-lookup"><span data-stu-id="e899d-119">[Planning](production-planning.md)    </span></span>  
 [<span data-ttu-id="e899d-120">Наличие</span><span class="sxs-lookup"><span data-stu-id="e899d-120">Inventory</span></span>](inventory-manage-inventory.md)  
 [<span data-ttu-id="e899d-121">Покупки</span><span class="sxs-lookup"><span data-stu-id="e899d-121">Purchasing</span></span>](purchasing-manage-purchasing.md)  
 <span data-ttu-id="e899d-122">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e899d-122">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

