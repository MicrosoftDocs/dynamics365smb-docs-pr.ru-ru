---
title: Использование перекрестных ссылок на товары | Документация Майкрософт
description: Если настроить перекрестную ссылку между описанием товара, которое вы используете для товара, и описанием, которое использует поставщик этого товара, то описание товара поставщика автоматически вставляется в документы покупки для поставщика, когда вы заполняете **Номер перекрестной ссылки**. .
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 89a99080723ee57270583ee2f277250d767b8dde
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3181944"
---
# <a name="use-item-cross-references"></a><span data-ttu-id="e9565-104">Использование перекрестных ссылок по товару</span><span class="sxs-lookup"><span data-stu-id="e9565-104">Use Item Cross References</span></span>
<span data-ttu-id="e9565-105">Если настроить перекрестную ссылку между описанием товара, которое вы используете для товара, и описанием, которое использует поставщик этого товара, то описание товара поставщика автоматически вставляется в документы покупки для поставщика, когда вы заполняете **Номер перекрестной ссылки**.</span><span class="sxs-lookup"><span data-stu-id="e9565-105">If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.**</span></span> <span data-ttu-id="e9565-106">.</span><span class="sxs-lookup"><span data-stu-id="e9565-106">field.</span></span> <span data-ttu-id="e9565-107">Такая же функция применяется для номеров товаров клиента в документах продажи.</span><span class="sxs-lookup"><span data-stu-id="e9565-107">The same functionality applies for customer item numbers on sales documents.</span></span>

<span data-ttu-id="e9565-108">В приведенных ниже процедурах описано, как использовать перекрестные ссылки товара на стороне покупки.</span><span class="sxs-lookup"><span data-stu-id="e9565-108">The following procedures describe how to use item cross references on the purchase side.</span></span> <span data-ttu-id="e9565-109">Действия на стороне продажи аналогичны.</span><span class="sxs-lookup"><span data-stu-id="e9565-109">The steps are similar for the sales side.</span></span>

## <a name="to-set-up-an-item-cross-reference-to-a-vendors-item-description"></a><span data-ttu-id="e9565-110">Настройка перекрестной ссылки товара на описание товара поставщика</span><span class="sxs-lookup"><span data-stu-id="e9565-110">To set up an item cross reference to a vendor's item description</span></span>
1. <span data-ttu-id="e9565-111">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e9565-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="e9565-112">Откройте карточку для товара, для которого требуется создать перекрестную ссылку на описание товара, которое используется поставщиком для данного товара.</span><span class="sxs-lookup"><span data-stu-id="e9565-112">Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.</span></span>
3. <span data-ttu-id="e9565-113">Выберите действие **Перекрестные ссылки**.</span><span class="sxs-lookup"><span data-stu-id="e9565-113">Choose the **Cross References** action.</span></span>
4. <span data-ttu-id="e9565-114">В новой строке на странице **Описание перекрестных ссылок по товару** заполните поля требуемыми данными.</span><span class="sxs-lookup"><span data-stu-id="e9565-114">On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="e9565-115">.</span><span class="sxs-lookup"><span data-stu-id="e9565-115">.</span></span>

## <a name="to-enter-a-vendors-item-description-on-a-purchase-order"></a><span data-ttu-id="e9565-116">Ввод описания товара поставщика в заказ на покупку</span><span class="sxs-lookup"><span data-stu-id="e9565-116">To enter a vendor's item description on a purchase order</span></span>
1. <span data-ttu-id="e9565-117">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на покупку**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="e9565-117">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="e9565-118">Создайте заказ на покупку для поставщика, для которого вы настроили перекрестную ссылку товара в предыдущей процедуре.</span><span class="sxs-lookup"><span data-stu-id="e9565-118">Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.</span></span>
3. <span data-ttu-id="e9565-119">Создайте строку покупки для товара, для которого вы настроили перекрестную ссылку товара в предыдущей процедуре.</span><span class="sxs-lookup"><span data-stu-id="e9565-119">Create a purchase line for the item that you set up an item cross reference for in the previous procedure.</span></span>
4. <span data-ttu-id="e9565-120">В поле **Номер перекрестной ссылки**</span><span class="sxs-lookup"><span data-stu-id="e9565-120">In the **Cross-Reference No.**</span></span> <span data-ttu-id="e9565-121">выберите перекрестную ссылку товара, которая была создана, затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="e9565-121">field, select the item cross reference that you have created, and then choose the **OK** button.</span></span>

<span data-ttu-id="e9565-122">Поле **Описание** в строке перезаписывается описанием товара поставщика согласно настройкам в перекрестной ссылке товара.</span><span class="sxs-lookup"><span data-stu-id="e9565-122">The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.</span></span>

## <a name="see-also"></a><span data-ttu-id="e9565-123">См. также</span><span class="sxs-lookup"><span data-stu-id="e9565-123">See Also</span></span>
[<span data-ttu-id="e9565-124">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="e9565-124">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="e9565-125">Запасы</span><span class="sxs-lookup"><span data-stu-id="e9565-125">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="e9565-126">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e9565-126">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
