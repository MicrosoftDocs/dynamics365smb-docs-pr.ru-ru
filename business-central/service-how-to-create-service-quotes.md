---
title: Как создавать сервисные предложения | Документация Майкрософт
description: Страницу **Сервисное предложение** можно использовать для создания документов, в которые вводится информация о сервисе, например ремонте и обслуживании, для сервисных товаров по запросу клиента. Можно использовать сервисное предложение как предварительный черновик сервисного заказа, а затем преобразовать предложение в сервисный заказ.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 4e04c2dc74ab1ecc0c0041258ca1824f872caac8
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2877235"
---
# <a name="create-service-quotes"></a><span data-ttu-id="5bbba-104">Создание сервисных предложений</span><span class="sxs-lookup"><span data-stu-id="5bbba-104">Create Service Quotes</span></span>
<span data-ttu-id="5bbba-105">Сервисные предложения можно рассматривать как основу для сервисных заказов.</span><span class="sxs-lookup"><span data-stu-id="5bbba-105">You can think of service quotes as the basis for service orders.</span></span> <span data-ttu-id="5bbba-106">Фактически, они почти полностью идентичны.</span><span class="sxs-lookup"><span data-stu-id="5bbba-106">In fact, they are almost identical.</span></span> <span data-ttu-id="5bbba-107">Они содержат такие сведения, как клиент, тип заказа, товар, который требует обслуживания, сведения для выставления счетов и отгрузки, а также информацию о фактической сервисной работе.</span><span class="sxs-lookup"><span data-stu-id="5bbba-107">They both contain information such as who the customer is, the type of order, the item that needs service, billing and shipping information, and information about the actual service work.</span></span>
 
<span data-ttu-id="5bbba-108">Можно использовать сервисное предложение как предварительный черновик сервисного заказа, а затем преобразовать предложение в сервисный заказ.</span><span class="sxs-lookup"><span data-stu-id="5bbba-108">You can use a service quote as a preliminary draft for a service order, and then convert the quote to a service order.</span></span>  
  
## <a name="to-create-a-service-quote"></a><span data-ttu-id="5bbba-109">Создание сервисного предложения</span><span class="sxs-lookup"><span data-stu-id="5bbba-109">To create a service quote</span></span>  
1. <span data-ttu-id="5bbba-110">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Сервисные предложения**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="5bbba-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Quotes**, and then choose the related link.</span></span>  
2. <span data-ttu-id="5bbba-111">Создание нового сервисного предложения.</span><span class="sxs-lookup"><span data-stu-id="5bbba-111">Create a new service quote.</span></span>  
3. <span data-ttu-id="5bbba-112">В поле **Номер**</span><span class="sxs-lookup"><span data-stu-id="5bbba-112">In the **No.**</span></span> <span data-ttu-id="5bbba-113">введите номер сервисного предложения.</span><span class="sxs-lookup"><span data-stu-id="5bbba-113">field, enter a number for the service quote.</span></span> <span data-ttu-id="5bbba-114">Вместо этого, если на странице **Сервисный центр - настройка** настроены серии номеров сервисных предложений, можно нажать клавишу ВВОД, чтобы выбрать следующий доступный номер сервисного предложения.</span><span class="sxs-lookup"><span data-stu-id="5bbba-114">Alternatively, if you have set up a number series for service quotes on the **Service Mgt. Setup** page, you can press Enter to select the next available service quote number.</span></span>  
4. <span data-ttu-id="5bbba-115">В поле **Номер клиента**</span><span class="sxs-lookup"><span data-stu-id="5bbba-115">In the **Customer No.**</span></span>  <span data-ttu-id="5bbba-116">выберите соответствующего клиента из списка.</span><span class="sxs-lookup"><span data-stu-id="5bbba-116">field, select the relevant customer from the list.</span></span>  

  > [!Note]  
  >  <span data-ttu-id="5bbba-117">Соответствующие поля для клиента заполняются автоматически данными из карточки **Клиент**.</span><span class="sxs-lookup"><span data-stu-id="5bbba-117">The customer fields are filled in automatically with information from the **Customer** card.</span></span> <span data-ttu-id="5bbba-118">Если карточка **Клиент** не существует для клиента, но шаблон клиента настроен, можно создать клиента из сервисного предложения.</span><span class="sxs-lookup"><span data-stu-id="5bbba-118">If a **Customer** card does not exist for the customer, and you have set up a customer template, you can create the customer from the service quote.</span></span> <span data-ttu-id="5bbba-119">Заполните соответствующие поля, затем выберите действие **Создать клиента**.</span><span class="sxs-lookup"><span data-stu-id="5bbba-119">Fill in the relevant fields, and then choose the **Create Customer** action.</span></span>  
  
5. <span data-ttu-id="5bbba-120">В зависимости от настроек на экспресс-вкладке **Обязательные поля**, возможно, на странице **Сервисный центр - настройка** нужно будет заполнить поля **Тип сервисного заказа** и **Код менеджера**.</span><span class="sxs-lookup"><span data-stu-id="5bbba-120">Depending on the settings on the **Mandatory Fields** FastTab on the **Service Mgt. Setup** page, you may need to fill in the **Service Order Type** field and the **Salesperson Code** field.</span></span>  
6. <span data-ttu-id="5bbba-121">Заполните строки сервисных товаров.</span><span class="sxs-lookup"><span data-stu-id="5bbba-121">Fill in the service item lines.</span></span>  
7. <span data-ttu-id="5bbba-122">Зарегистрируйте ожидаемые себестоимости в строках сервиса.</span><span class="sxs-lookup"><span data-stu-id="5bbba-122">Register estimated costs on the service lines.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="5bbba-123">См. также</span><span class="sxs-lookup"><span data-stu-id="5bbba-123">See Also</span></span>  
[<span data-ttu-id="5bbba-124">Создание сервисных заказов</span><span class="sxs-lookup"><span data-stu-id="5bbba-124">Create Service Orders</span></span>](service-how-to-create-service-orders.md)  
[<span data-ttu-id="5bbba-125">Работа с сервисными задачами</span><span class="sxs-lookup"><span data-stu-id="5bbba-125">Work on Service tasks</span></span>](service-how-to-work-on-service-tasks.md)  

 