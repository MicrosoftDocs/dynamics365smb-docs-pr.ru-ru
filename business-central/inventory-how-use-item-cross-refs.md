---
title: Использование перекрестных ссылок по товару
description: Установите ссылки между описаниями, которые вы и ваш поставщик используете для товара, чтобы вы могли вставить описание товара поставщика в документы покупки.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: item reference, cross reference, inventory
ms.date: 01/12/2021
ms.author: edupont
ms.openlocfilehash: 2f500d7df80235b8f092fc3f0a7ae8fd27cd8aea
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5377627"
---
# <a name="use-item-cross-references"></a><span data-ttu-id="999e2-103">Использование перекрестных ссылок по товару</span><span class="sxs-lookup"><span data-stu-id="999e2-103">Use Item Cross References</span></span>
<span data-ttu-id="999e2-104">Если настроить перекрестную ссылку между описанием товара, которое вы используете для товара, и описанием, которое использует поставщик этого товара, то описание товара поставщика автоматически вставляется в документы покупки для поставщика, когда вы заполняете **Номер перекрестной ссылки**.</span><span class="sxs-lookup"><span data-stu-id="999e2-104">If you set up a cross reference between the item description that you use for an item and the description that the vendor of that item uses, then the vendor's item description is automatically inserted on purchase documents for the vendor when you fill in the **Cross-Reference No.**</span></span> <span data-ttu-id="999e2-105">.</span><span class="sxs-lookup"><span data-stu-id="999e2-105">field.</span></span> <span data-ttu-id="999e2-106">Такая же функция применяется для номеров товаров клиента в документах продажи.</span><span class="sxs-lookup"><span data-stu-id="999e2-106">The same functionality applies for customer item numbers on sales documents.</span></span>

<span data-ttu-id="999e2-107">В приведенных ниже процедурах описано, как использовать перекрестные ссылки товара на стороне покупки.</span><span class="sxs-lookup"><span data-stu-id="999e2-107">The following procedures describe how to use item cross references on the purchase side.</span></span> <span data-ttu-id="999e2-108">Действия на стороне продажи аналогичны.</span><span class="sxs-lookup"><span data-stu-id="999e2-108">The steps are similar for the sales side.</span></span>

> [!NOTE]
> <span data-ttu-id="999e2-109">Идентификаторы товаров, такие как GTIN или GUID, все чаще содержат 30 или более символов, что больше, чем может обрабатывать текущая функция перекрестных ссылок на товары.</span><span class="sxs-lookup"><span data-stu-id="999e2-109">It's becoming more common for item identifiers such as GTINs or GUIDs to contain 30 or more characters, which is more than the current feature for item cross references can handle.</span></span> <span data-ttu-id="999e2-110">Если вам нужно использовать ссылки, содержащие более 30 символов, ваш администратор может включить функцию **Запись более длинных ссылок на товары** на странице [Управление функциями](https://businesscentral.dynamics.com/?page=2610) (ссылка требует наличия клиента [!INCLUDE[prod_short](includes/prod_short.md)]).</span><span class="sxs-lookup"><span data-stu-id="999e2-110">If you need to use references that contain more than 30 characters, your administrator can turn on the **Write longer item references** feature on the [Feature Management](https://businesscentral.dynamics.com/?page=2610) page (link requires that you have a [!INCLUDE[prod_short](includes/prod_short.md)] tenant).</span></span> <span data-ttu-id="999e2-111">То, как вы используете ссылки, не меняется, но меняются названия таких вещей, как страницы и кнопки.</span><span class="sxs-lookup"><span data-stu-id="999e2-111">How you use references doesn't change, but the names of things like pages and buttons will.</span></span> <span data-ttu-id="999e2-112">Например, страница **Описание перекрестных ссылок по товару** станет страницей **Операции со ссылками на товар**.</span><span class="sxs-lookup"><span data-stu-id="999e2-112">For example, the **Item Cross-Reference Entries** page will become the **Item Reference Entries** page.</span></span>

## <a name="to-set-up-an-item-cross-reference-to-a-vendors-item-description"></a><span data-ttu-id="999e2-113">Настройка перекрестной ссылки товара на описание товара поставщика</span><span class="sxs-lookup"><span data-stu-id="999e2-113">To set up an item cross reference to a vendor's item description</span></span>

1. <span data-ttu-id="999e2-114">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="999e2-114">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="999e2-115">Откройте карточку для товара, для которого требуется создать перекрестную ссылку на описание товара, которое используется поставщиком для данного товара.</span><span class="sxs-lookup"><span data-stu-id="999e2-115">Open the card for an item for which you want to create a cross reference to the item description that the vendor uses for that item.</span></span>
3. <span data-ttu-id="999e2-116">Выберите действие **Перекрестные ссылки**.</span><span class="sxs-lookup"><span data-stu-id="999e2-116">Choose the **Cross References** action.</span></span>

     <span data-ttu-id="999e2-117">Если вы не можете найти действие **Перекрестные ссылки**, выберите дополнительные параметры, а затем найдите его в **Связанные** > **Товар**.</span><span class="sxs-lookup"><span data-stu-id="999e2-117">If you cannot find the **Cross References** action, choose to view more options, and then find it under **Related** > **Item**.</span></span>
  
4. <span data-ttu-id="999e2-118">В новой строке на странице **Описание перекрестных ссылок по товару** заполните поля требуемыми данными.</span><span class="sxs-lookup"><span data-stu-id="999e2-118">On a new line on the **Item Cross-Reference Entries** page, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]<span data-ttu-id="999e2-119">.</span><span class="sxs-lookup"><span data-stu-id="999e2-119">.</span></span>

## <a name="to-enter-a-vendors-item-description-on-a-purchase-order"></a><span data-ttu-id="999e2-120">Ввод описания товара поставщика в заказ на покупку</span><span class="sxs-lookup"><span data-stu-id="999e2-120">To enter a vendor's item description on a purchase order</span></span>

1. <span data-ttu-id="999e2-121">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на покупку**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="999e2-121">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>
2. <span data-ttu-id="999e2-122">Создайте заказ на покупку для поставщика, для которого вы настроили перекрестную ссылку товара в предыдущей процедуре.</span><span class="sxs-lookup"><span data-stu-id="999e2-122">Create a purchase order for the vendor that you set up an item cross reference for in the previous procedure.</span></span>
3. <span data-ttu-id="999e2-123">Создайте строку покупки для товара, для которого вы настроили перекрестную ссылку товара в предыдущей процедуре.</span><span class="sxs-lookup"><span data-stu-id="999e2-123">Create a purchase line for the item that you set up an item cross reference for in the previous procedure.</span></span>
4. <span data-ttu-id="999e2-124">В поле **Номер перекрестной ссылки**</span><span class="sxs-lookup"><span data-stu-id="999e2-124">In the **Cross-Reference No.**</span></span> <span data-ttu-id="999e2-125">выберите перекрестную ссылку товара, которая была создана, затем выберите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="999e2-125">field, select the item cross reference that you have created, and then choose the **OK** button.</span></span>

<span data-ttu-id="999e2-126">Поле **Описание** в строке перезаписывается описанием товара поставщика согласно настройкам в перекрестной ссылке товара.</span><span class="sxs-lookup"><span data-stu-id="999e2-126">The **Description** field on the line is overwritten with the vendor's item description, as set up on the item cross-reference entry.</span></span>

## <a name="see-also"></a><span data-ttu-id="999e2-127">См. также</span><span class="sxs-lookup"><span data-stu-id="999e2-127">See Also</span></span>
[<span data-ttu-id="999e2-128">Регистрация новых товаров</span><span class="sxs-lookup"><span data-stu-id="999e2-128">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="999e2-129">Запасы</span><span class="sxs-lookup"><span data-stu-id="999e2-129">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="999e2-130">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="999e2-130">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]