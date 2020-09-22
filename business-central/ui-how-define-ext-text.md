---
title: Добавление строк для определения расширенных описаний
description: Вы можете добавить строки, чтобы расширить стандартный текст описания товара, счет ГК и другие данные.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 07/08/2020
ms.author: edupont
ms.openlocfilehash: cf0418f4182e9d66da88af9262dd807a34dd3572
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3782322"
---
# <a name="add-extended-text"></a><span data-ttu-id="9fd16-103">Добавить расширенный текст</span><span class="sxs-lookup"><span data-stu-id="9fd16-103">Add Extended Text</span></span>

<span data-ttu-id="9fd16-104">Вы можете расширить описание товаров, единиц хранения, счетов главной книги и ресурсов, добавив дополнительные строки в виде расширенного текста.</span><span class="sxs-lookup"><span data-stu-id="9fd16-104">You can extend the description for items, stock-keeping units, general ledger accounts, and resources by adding extra lines as extended text.</span></span> <span data-ttu-id="9fd16-105">Вы также можете установить условия для использования дополнительных строк.</span><span class="sxs-lookup"><span data-stu-id="9fd16-105">You can also set up conditions for use of the extra lines.</span></span>  

<span data-ttu-id="9fd16-106">В следующем разделе описывается, как добавить расширенный текст в описание товара.</span><span class="sxs-lookup"><span data-stu-id="9fd16-106">The following section describes how to add extended text to a description of an item.</span></span> <span data-ttu-id="9fd16-107">Но те же шаги применяются к единицам хранения, счетам главной книги и ресурсам.</span><span class="sxs-lookup"><span data-stu-id="9fd16-107">But the same steps apply to stock-keeping units, general ledger accounts, and resources.</span></span>  

## <a name="to-define-extended-text-for-an-description"></a><span data-ttu-id="9fd16-108">Определение расширенного текста для описания</span><span class="sxs-lookup"><span data-stu-id="9fd16-108">To define extended text for an description</span></span>

1. <span data-ttu-id="9fd16-109">Откройте карточку для товара, для которого необходимо добавить расширенный текст, затем выберите действие **Расширенный текст**.</span><span class="sxs-lookup"><span data-stu-id="9fd16-109">Open the card for an item that you want to add extended text to, and then choose the **Extended Text** action.</span></span>
2. <span data-ttu-id="9fd16-110">Заполните поля **Код** и **Описание**.</span><span class="sxs-lookup"><span data-stu-id="9fd16-110">Fill in the **Code** and **Description** fields.</span></span>
3. <span data-ttu-id="9fd16-111">Выберите **Создать**.</span><span class="sxs-lookup"><span data-stu-id="9fd16-111">Choose the **New**.</span></span>
4. <span data-ttu-id="9fd16-112">Заполните поле **Код языка** или установите флажок **Все коды языков**, если используются коды языков.</span><span class="sxs-lookup"><span data-stu-id="9fd16-112">Fill in the **Language Code** field or select the **All Language Codes** check box if you use language codes.</span></span>
5. <span data-ttu-id="9fd16-113">Заполните поля **Дата начала** и **Дата окончания** для ограничения времени использования расширенного текста.</span><span class="sxs-lookup"><span data-stu-id="9fd16-113">Fill in the **Starting Date** and **Ending Date** fields if you want to limit the dates on which the extended text is used.</span></span>
6. <span data-ttu-id="9fd16-114">В поле **Текст** введите расширенный текст.</span><span class="sxs-lookup"><span data-stu-id="9fd16-114">In the **Text** field, write the extended text.</span></span>
7. <span data-ttu-id="9fd16-115">Установите соответствующие флажки для тех типов документов, в которых необходимо печатать расширенный текст.</span><span class="sxs-lookup"><span data-stu-id="9fd16-115">Select relevant check boxes for the document types where you want the extended text printed.</span></span>
8. <span data-ttu-id="9fd16-116">Закройте страницу.</span><span class="sxs-lookup"><span data-stu-id="9fd16-116">Close the page.</span></span>

<span data-ttu-id="9fd16-117">Теперь вы можете добавить этот расширенный текст в документы.</span><span class="sxs-lookup"><span data-stu-id="9fd16-117">You can now add this extended text to documents.</span></span> <span data-ttu-id="9fd16-118">Следующая процедура объясняет, как добавить расширенный текст в заказ на продажу, но те же шаги применимы к любому другому документу, который вы указали для расширенного текста.</span><span class="sxs-lookup"><span data-stu-id="9fd16-118">The following procedure explains how to add extended text to a sales order, but the same steps apply to any other document that you specified for the extended text.</span></span>  

## <a name="to-add-an-extended-item-text-on-a-sales-order-line"></a><span data-ttu-id="9fd16-119">Добавление расширенного текста товара в строку заказа на продажу</span><span class="sxs-lookup"><span data-stu-id="9fd16-119">To add an extended item text on a sales order line</span></span>

1. <span data-ttu-id="9fd16-120">Откройте заказ на продажу со строкой продажи для товара, для которого определен расширенный текст.</span><span class="sxs-lookup"><span data-stu-id="9fd16-120">Open a sales order with a sales line for an item that has extended text defined.</span></span> <span data-ttu-id="9fd16-121">Дополнительные сведения см. в разделе [Продажа продукции](sales-how-sell-products.md).</span><span class="sxs-lookup"><span data-stu-id="9fd16-121">For more information, see [Sell Products](sales-how-sell-products.md).</span></span>
2. <span data-ttu-id="9fd16-122">Выберите соответствующую строку, затем выберите действие **Вставить расширенный текст**.</span><span class="sxs-lookup"><span data-stu-id="9fd16-122">Select the line in question, and then choose the **Insert Ext. Text** action.</span></span>

## <a name="see-also"></a><span data-ttu-id="9fd16-123">См. также</span><span class="sxs-lookup"><span data-stu-id="9fd16-123">See Also</span></span>

[<span data-ttu-id="9fd16-124">Настройка запасов</span><span class="sxs-lookup"><span data-stu-id="9fd16-124">Setting Up Inventory</span></span>](inventory-setup-inventory.md)  
<span data-ttu-id="9fd16-125">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9fd16-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
