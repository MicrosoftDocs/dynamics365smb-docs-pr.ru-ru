---
title: "Практическое руководство. Настройка расширения \"Почтовые индексы Великобритании GetAddress.io\" | Документы Майкрософт"
description: "Описываются общие функции, которые вы используете для работы с данными в Financials, например ввод значений, сортировка данных и изменение представлений."
services: project-madeira
documentationcenter: 
author: bholtorf
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: getaddress.io, postcodes, extension
ms.date: 06/02/2017
ms.author: bholtorf
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: c5a99f7a90b2f832bba3eb088d0faa7514c14708
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-set-up-the-getaddressio-uk-postcodes-extension"></a><span data-ttu-id="8960d-103">Практическое руководство. Настройка расширения "Почтовые индексы Великобритании GetAddress.io"</span><span class="sxs-lookup"><span data-stu-id="8960d-103">How to: Set Up the GetAddress.io UK Postcodes Extension</span></span>
<span data-ttu-id="8960d-104">Это расширение облегчает ввод данных в Великобритании для объектов, таких как клиенты, контакты, сотрудники, поставщики, банковские счета и т. д.</span><span class="sxs-lookup"><span data-stu-id="8960d-104">This extension makes it easy to enter addresses in the UK for entities like customers, contacts, employees, vendors, bank accounts, and so on.</span></span> 

<span data-ttu-id="8960d-105">Расширение "Почтовые индексы Великобритании GetAddress.io" использует API getAddress для поиска адресов в почтовых индексах в Великобритании.</span><span class="sxs-lookup"><span data-stu-id="8960d-105">The GetAddress.io UK Postcodes extension uses the getAddress API to find addresses in postcodes in the UK.</span></span> <span data-ttu-id="8960d-106">Для использования расширения необходимо получить план и ключ API для API getAddress.</span><span class="sxs-lookup"><span data-stu-id="8960d-106">To use the extension, you need to get a plan and an API Key for the getAddress API.</span></span> <span data-ttu-id="8960d-107">Это просто, и мы помогаем в этом при настройке расширения "Почтовые индексы Великобритании GetAddress.io".</span><span class="sxs-lookup"><span data-stu-id="8960d-107">That's easy, and we help you do that when you set up the GetAddress.io UK Postcodes extension.</span></span> <span data-ttu-id="8960d-108">Планы основываются на использовании или, как это иногда называется, вызовах.</span><span class="sxs-lookup"><span data-stu-id="8960d-108">Plans are based on use, or what's sometimes referred to as calls.</span></span> <span data-ttu-id="8960d-109">Вызов в данном случае — это когда [!INCLUDE[d365fin](includes/d365fin_md.md)] отображает список адресов в почтовом индексе.</span><span class="sxs-lookup"><span data-stu-id="8960d-109">A call, in this case, is when [!INCLUDE[d365fin](includes/d365fin_md.md)] displays a list of addresses in a postcode.</span></span> <span data-ttu-id="8960d-110">В зависимости от того, как часто вы добавляете адреса, выберите план, оптимальный для вас.</span><span class="sxs-lookup"><span data-stu-id="8960d-110">Depending on how often you add addresses, choose the plan that is best for you.</span></span> <span data-ttu-id="8960d-111">Если выбрать **Получить ключ API** на странице, вы будете использовать план **Бесплатно**, который позволяет добавить 20 адресов в день и действителен в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="8960d-111">If you just choose **Get API Key** in the page, you'll use the **Free** plan, which lets you add 20 addresses per day, and is valid for 30 days.</span></span> 

##<a name="to-set-up-the-getaddressio-uk-postcodes-extension"></a><span data-ttu-id="8960d-112">Настройка расширения "Почтовые индексы Великобритании GetAddress.io"</span><span class="sxs-lookup"><span data-stu-id="8960d-112">To set up the GetAddress.io UK Postcodes extension</span></span> 
1. <span data-ttu-id="8960d-113">Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Подключения к службе**, а затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="8960d-113">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Service Connections**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8960d-114">В окне **Подключения к службе** выберите **Служба почтовых индексов Великобритании**.</span><span class="sxs-lookup"><span data-stu-id="8960d-114">In the **Service Connections** window, choose **UK Postcode Service**.</span></span>
3. <span data-ttu-id="8960d-115">На странице **Конфигурация поставщика почтовых индексов** выберите **Отключено**.</span><span class="sxs-lookup"><span data-stu-id="8960d-115">In the **Postcode provider configuration** page, choose **Disabled**.</span></span>
4. <span data-ttu-id="8960d-116">В окне **Выбор службы почтовых индексов** выберите **GetAddress.io**.</span><span class="sxs-lookup"><span data-stu-id="8960d-116">In the **Postal code service selection** window, choose **GetAddress.io**.</span></span>
5. <span data-ttu-id="8960d-117">В окне **Конфигурация GetAddress.io** выберите **Получить ключ API**, чтобы открыть страницу **Планы** на веб-сайте для API getAddress.</span><span class="sxs-lookup"><span data-stu-id="8960d-117">In the **GetAddress.io Config** window, choose **Get API Key** to open the **Plans** page on the website for the getAddress API.</span></span>  

    > [!NOTE]  
>   <span data-ttu-id="8960d-118">Возможно, потребуется разрешить всплывающие окна в браузере.</span><span class="sxs-lookup"><span data-stu-id="8960d-118">You might need to allow pop-ups in your browser.</span></span>
6. <span data-ttu-id="8960d-119">Приобретите план или выберите **Получить ключ API**, а затем введите свой адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8960d-119">Purchase a plan, or just choose **Get API Key**, and then provide your email address.</span></span>
7. <span data-ttu-id="8960d-120">Откройте электронную почту в getAddress.io и скопируйте ключ API.</span><span class="sxs-lookup"><span data-stu-id="8960d-120">Open the email from getAddress.io, and copy the API key.</span></span> <span data-ttu-id="8960d-121">Ключ находится под заголовком **Ваш ключ API**.</span><span class="sxs-lookup"><span data-stu-id="8960d-121">The key is under the **Your API Key** heading.</span></span>
8. <span data-ttu-id="8960d-122">В окне **Конфигурация GetAddress.io** вставьте ключ API в поле **Ключ API**, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="8960d-122">In the **GetAddress.io Config** window, paste the API key in the **API Key** field, and then choose **OK**.</span></span>
9. <span data-ttu-id="8960d-123">На странице **Подключения к службе** проверьте, что в поле **Поставщика адресов** отображается **GetAddress.io**.</span><span class="sxs-lookup"><span data-stu-id="8960d-123">In the **Service Connections** page, verify that the **Address Provider** field shows **GetAddress.io**.</span></span> <span data-ttu-id="8960d-124">Если да, служба включена.</span><span class="sxs-lookup"><span data-stu-id="8960d-124">If it does, the service is enabled.</span></span>

## <a name="see-also"></a><span data-ttu-id="8960d-125">См. также</span><span class="sxs-lookup"><span data-stu-id="8960d-125">See Also</span></span>
<span data-ttu-id="8960d-126">[Почтовые индексы Великобритании GetAddress.io](ui-extensions-getaddressio.md)
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] Использование расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="8960d-126">[GetAddress.io UK Postcodes](ui-extensions-getaddressio.md)
[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
<span data-ttu-id="8960d-127">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8960d-127">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
