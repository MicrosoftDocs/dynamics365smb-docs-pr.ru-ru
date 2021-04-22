---
title: Создание предложения по покупке для запроса предложения | Документация Майкрософт
description: Описывается процесс создание предложения по продаже или запроса предложения (RFQ) для записи вашего предложения клиенту для продажи продуктов на определенных условиях.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: rfq
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 416c5a4e4376932c16a1496f2db2b0c79307d22b
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5772623"
---
# <a name="request-quotes"></a><span data-ttu-id="2619d-103">Запрос предложений</span><span class="sxs-lookup"><span data-stu-id="2619d-103">Request Quotes</span></span>
<span data-ttu-id="2619d-104">Предложение по покупке может использоваться в качестве предварительного предложения по заказу на покупку, а заказ затем может быть преобразован в счет или заказ на покупку.</span><span class="sxs-lookup"><span data-stu-id="2619d-104">A purchase quote can be used as a preliminary draft for a purchase order, and the order can then be converted to a purchase invoice or an order.</span></span>


## <a name="to-create-a-purchase-quote"></a><span data-ttu-id="2619d-105">Создание предложения по покупке</span><span class="sxs-lookup"><span data-stu-id="2619d-105">To create a purchase quote</span></span>
1. <span data-ttu-id="2619d-106">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Предложения по покупке**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="2619d-106">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Quotes**, and then choose the related link.</span></span>
2. <span data-ttu-id="2619d-107">Создайте новый документ, так же, как это делается для заказа на покупку.</span><span class="sxs-lookup"><span data-stu-id="2619d-107">Create a new document, in the same way as you make a purchase order.</span></span> <span data-ttu-id="2619d-108">Дополнительные сведения см. в разделе [Регистрация покупок](purchasing-how-record-purchases.md).</span><span class="sxs-lookup"><span data-stu-id="2619d-108">For more information, see [Record Purchases](purchasing-how-record-purchases.md).</span></span>

## <a name="to-convert-a-purchase-quote-to-a-purchase-order"></a><span data-ttu-id="2619d-109">Преобразование предложения по покупке в заказ на покупку</span><span class="sxs-lookup"><span data-stu-id="2619d-109">To convert a purchase quote to a purchase order</span></span>
<span data-ttu-id="2619d-110">Когда вы приняли предложение поставщика, можно преобразовать его в счет или заказ покупки для обработки покупки.</span><span class="sxs-lookup"><span data-stu-id="2619d-110">When you have accepted the vendor's quote, you can convert it to a purchase invoice or order to process the purchase.</span></span>

1. <span data-ttu-id="2619d-111">Откройте предложение по покупке, которое готово к преобразованию, затем выберите действие **Сделать заказ**.</span><span class="sxs-lookup"><span data-stu-id="2619d-111">Open a purchase quote that is ready to convert, and then choose the **Make Order** action.</span></span>

<span data-ttu-id="2619d-112">Предложение по покупке удаляется из базы данных.</span><span class="sxs-lookup"><span data-stu-id="2619d-112">The purchase quote is removed from the database.</span></span> <span data-ttu-id="2619d-113">Создается счет покупки или заказ на покупку на основе сведений в предложении по покупке, в котором можно обработать покупку.</span><span class="sxs-lookup"><span data-stu-id="2619d-113">A purchase invoice or a purchase order is created based on the information in the purchase quote in which you can process the purchase.</span></span> <span data-ttu-id="2619d-114">В поле **Номер предложения** в счете покупке или заказе покупки отображается номер предложения по покупки, из которого он создан.</span><span class="sxs-lookup"><span data-stu-id="2619d-114">In the **Quote No.** field on the purchase invoice or purchase order, you can see the number of the purchase quote that it was made from.</span></span>

## <a name="see-also"></a><span data-ttu-id="2619d-115">См. также</span><span class="sxs-lookup"><span data-stu-id="2619d-115">See Also</span></span>
[<span data-ttu-id="2619d-116">Покупки</span><span class="sxs-lookup"><span data-stu-id="2619d-116">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="2619d-117">Настройка покупки</span><span class="sxs-lookup"><span data-stu-id="2619d-117">Setting Up Purchasing</span></span>](purchasing-setup-purchasing.md)  
[<span data-ttu-id="2619d-118">Отправка документов по электронной почте</span><span class="sxs-lookup"><span data-stu-id="2619d-118">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
<span data-ttu-id="2619d-119">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2619d-119">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]