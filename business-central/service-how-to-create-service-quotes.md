---
title: Как создавать сервисные предложения | Документация Майкрософт
description: Страницу **Сервисное предложение** можно использовать для создания документов, в которые вводится информация о сервисе, например ремонте и обслуживании, для сервисных товаров по запросу клиента. Можно использовать сервисное предложение как предварительный черновик сервисного заказа, а затем преобразовать предложение в сервисный заказ.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 92c93b2e0b876920f1c259d31b4d839a5b2ecbc0
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5388803"
---
# <a name="create-service-quotes"></a><span data-ttu-id="13953-104">Создание сервисных предложений</span><span class="sxs-lookup"><span data-stu-id="13953-104">Create Service Quotes</span></span>
<span data-ttu-id="13953-105">Сервисные предложения можно рассматривать как основу для сервисных заказов.</span><span class="sxs-lookup"><span data-stu-id="13953-105">You can think of service quotes as the basis for service orders.</span></span> <span data-ttu-id="13953-106">Фактически, они почти полностью идентичны.</span><span class="sxs-lookup"><span data-stu-id="13953-106">In fact, they are almost identical.</span></span> <span data-ttu-id="13953-107">Они содержат такие сведения, как клиент, тип заказа, товар, который требует обслуживания, сведения для выставления счетов и отгрузки, а также информацию о фактической сервисной работе.</span><span class="sxs-lookup"><span data-stu-id="13953-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span></span>
 
<span data-ttu-id="13953-108">Можно использовать сервисное предложение как предварительный черновик сервисного заказа, а затем преобразовать предложение в сервисный заказ.</span><span class="sxs-lookup"><span data-stu-id="13953-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span></span>  
  
## <a name="to-create-a-service-quote"></a><span data-ttu-id="13953-109">Создание сервисного предложения</span><span class="sxs-lookup"><span data-stu-id="13953-109">To create a service quote</span></span>  
1. <span data-ttu-id="13953-110">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сервисные предложения**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="13953-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Quotes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="13953-111">Создание нового сервисного предложения.</span><span class="sxs-lookup"><span data-stu-id="13953-111">Create a new service quote.</span></span>  
3. <span data-ttu-id="13953-112">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="13953-112">In the **No.**</span></span> <span data-ttu-id="13953-113">введите номер сервисного предложения.</span><span class="sxs-lookup"><span data-stu-id="13953-113">field, enter a number for the service quote.</span></span> <span data-ttu-id="13953-114">Вместо этого, если на странице **Сервисный центр - настройка** настроены серии номеров сервисных предложений, можно нажать клавишу ВВОД, чтобы выбрать следующий доступный номер сервисного предложения.</span><span class="sxs-lookup"><span data-stu-id="13953-114">Alternatively, if you have set up a number series for service quotes on the **Service Mgt. Setup** page, you can press Enter to select the next available service quote number.</span></span>  
4. <span data-ttu-id="13953-115">В поле **Номер клиента**</span><span class="sxs-lookup"><span data-stu-id="13953-115">In the **Customer No.**</span></span>  <span data-ttu-id="13953-116">выберите соответствующего клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="13953-116">field, select the relevant customer from the list.</span></span>  

  > [!Note]  
  >  <span data-ttu-id="13953-117">Соответствующие поля для клиента заполняются автоматически данными из карточки **Клиент**.</span><span class="sxs-lookup"><span data-stu-id="13953-117">The customer fields are filled in automatically with information from the **Customer** card.</span></span> <span data-ttu-id="13953-118">Если карточка **Клиент** не существует для клиента, но шаблон клиента настроен, можно создать клиента из сервисного предложения.</span><span class="sxs-lookup"><span data-stu-id="13953-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span></span> <span data-ttu-id="13953-119">Заполните соответствующие поля, затем выберите действие **Создать клиента**.</span><span class="sxs-lookup"><span data-stu-id="13953-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span></span>  
  
5. <span data-ttu-id="13953-120">В зависимости от настроек на экспресс-вкладке **Обязательные поля**, возможно, на странице **Сервисный центр - настройка** нужно будет заполнить поля **Тип сервисного заказа** и **Код менеджера**.</span><span class="sxs-lookup"><span data-stu-id="13953-120">Depending on the settings on the **Mandatory Fields** FastTab on the **Service Mgt. Setup** page, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span></span>  
6. <span data-ttu-id="13953-121">Заполните строки сервисных товаров.</span><span class="sxs-lookup"><span data-stu-id="13953-121">Fill in the service item lines.</span></span>  
7. <span data-ttu-id="13953-122">Зарегистрируйте ожидаемые себестоимости в строках сервиса.</span><span class="sxs-lookup"><span data-stu-id="13953-122">Register estimated costs on the service lines.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="13953-123">См. также</span><span class="sxs-lookup"><span data-stu-id="13953-123">See Also</span></span>  
[<span data-ttu-id="13953-124">Создание сервисных заказов</span><span class="sxs-lookup"><span data-stu-id="13953-124">Create Service Orders</span></span>](service-how-to-create-service-orders.md)  
[<span data-ttu-id="13953-125">Работа с сервисными задачами</span><span class="sxs-lookup"><span data-stu-id="13953-125">Work on Service tasks</span></span>](service-how-to-work-on-service-tasks.md)  

 

[!INCLUDE[footer-include](includes/footer-banner.md)]