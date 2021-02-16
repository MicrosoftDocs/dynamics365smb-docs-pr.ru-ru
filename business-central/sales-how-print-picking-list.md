---
title: Печать сборочного листа из заказа на продажу
description: Сборочные листы можно печатать непосредственно из заказа на продажу, счета продажи и других исходящих документов продажи.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 47ae132d862d2c05bef4ea0d0af26688bdd16588
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4758221"
---
# <a name="print-the-picking-list"></a><span data-ttu-id="8b946-103">Печать сборочного листа</span><span class="sxs-lookup"><span data-stu-id="8b946-103">Print the Picking List</span></span>
<span data-ttu-id="8b946-104">Сборочные листы можно печатать непосредственно из заказа на продажу, счета продажи и любого другого документа, который является основанием для отгрузки товаров.</span><span class="sxs-lookup"><span data-stu-id="8b946-104">You can print an inventory picking list directly from a sales order, a sales invoice, or any other document that initiates shipment of items.</span></span>

<span data-ttu-id="8b946-105">Этот отчет обычно используется в компаниях, которые не используют отдельную функциональность для управления складом, чтобы работник склада мог просто просмотреть или напечатать сборочный лист из связанного с ним документа продаж.</span><span class="sxs-lookup"><span data-stu-id="8b946-105">This report is typically used in companies without dedicated functionality for warehouse management, so that an inventory worker can simply view or print the picking list from the related sales document.</span></span> <span data-ttu-id="8b946-106">В компаниях с большими объемами или более сложными процессами подбор товаров планируется и выполняется по специальным складским документам.</span><span class="sxs-lookup"><span data-stu-id="8b946-106">In companies with higher volume or more complex processes, picking is planned and performed in dedicated warehouse documents.</span></span> <span data-ttu-id="8b946-107">Дополнительные сведения см. в разделе [Подбор товаров](warehouse-pick-items.md).</span><span class="sxs-lookup"><span data-stu-id="8b946-107">For more information, see [Pick Items](warehouse-pick-items.md).</span></span>

## <a name="to-print-a-picking-list-from-a-sales-order"></a><span data-ttu-id="8b946-108">Печать сборочного листа из заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="8b946-108">To print a picking list from a sales order</span></span>  
<span data-ttu-id="8b946-109">Следующая процедура основана на заказе на продажу.</span><span class="sxs-lookup"><span data-stu-id="8b946-109">The following procedure is based on a sales order.</span></span> <span data-ttu-id="8b946-110">Аналогичные шаги можно использовать для всех документов продажи, которые являются основанием для отгрузки товаров.</span><span class="sxs-lookup"><span data-stu-id="8b946-110">The steps are similar for all sales documents that can be used to initiate shipment of items.</span></span>

1. <span data-ttu-id="8b946-111">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Заказы на продажу**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="8b946-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Sales Orders**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8b946-112">Откройте заказ на продажу, для которого требуется собрать товары.</span><span class="sxs-lookup"><span data-stu-id="8b946-112">Open the sales order that you want to pick items for.</span></span>  
3. <span data-ttu-id="8b946-113">Выберите действие **Отчет**, а затем выберите действие **Сборочный лист по заказу**.</span><span class="sxs-lookup"><span data-stu-id="8b946-113">Choose the **Report** action, and then choose the **Picking List by Order** action.</span></span>  
4. <span data-ttu-id="8b946-114">Нажмите кнопку **Печать**, чтобы распечатать сборочный лист, или кнопку **Просмотр**, чтобы отобразить его на экране.</span><span class="sxs-lookup"><span data-stu-id="8b946-114">Choose the **Print** button to print the picking list or choose the **Preview** button to view it on the screen.</span></span>

<span data-ttu-id="8b946-115">Вы также можете сохранить сборочный лист в качестве документа, — например, чтобы отправить его кому-либо или добавить в качестве вложения в заказ на продажу.</span><span class="sxs-lookup"><span data-stu-id="8b946-115">You can also save the picking list as a document, for example, to send to someone or to add as an attachment to the sales order.</span></span> <span data-ttu-id="8b946-116">Дополнительные сведения см. в разделе [Управление вложениями, ссылками и заметками в карточках и документах](ui-how-add-link-to-record.md).</span><span class="sxs-lookup"><span data-stu-id="8b946-116">For more information, see [Manage Attachments, Links, and Notes on Cards and Documents](ui-how-add-link-to-record.md).</span></span>

> [!NOTE]
> <span data-ttu-id="8b946-117">Если вы использовали в заказе на продажу функцию **Раскрыть спецификацию**, то в отчете отображаются только компоненты связанного сборочного элемента.</span><span class="sxs-lookup"><span data-stu-id="8b946-117">If you used the **Explode BOM** function on the sales order, then only the components of the related assembly item are shown in the report.</span></span> <span data-ttu-id="8b946-118">Дополнительные сведения см. в разделе [Работа со спецификациями](inventory-how-work-BOMs.md).</span><span class="sxs-lookup"><span data-stu-id="8b946-118">For more information, see [Work with Bills of Material](inventory-how-work-BOMs.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="8b946-119">См. также</span><span class="sxs-lookup"><span data-stu-id="8b946-119">See Also</span></span>  
[<span data-ttu-id="8b946-120">Запасы</span><span class="sxs-lookup"><span data-stu-id="8b946-120">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="8b946-121">Подбор товаров</span><span class="sxs-lookup"><span data-stu-id="8b946-121">Pick Items</span></span>](warehouse-pick-items.md)  
<span data-ttu-id="8b946-122">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8b946-122">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>   
