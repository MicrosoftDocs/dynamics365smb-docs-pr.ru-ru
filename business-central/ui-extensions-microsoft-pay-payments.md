---
title: Стандарт Microsoft Pay | Документация Майкрософт
description: Предоставляет сведения о расширении Microsoft Pay.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 5885674316e082323462cbad9fce3f20590f06d5
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3915039"
---
# <a name="the-microsoft-pay-extension"></a><span data-ttu-id="64d46-103">Расширение Microsoft Pay</span><span class="sxs-lookup"><span data-stu-id="64d46-103">The Microsoft Pay Extension</span></span>

> [!IMPORTANT]
> <span data-ttu-id="64d46-104">Начиная с 8 февраля 2020 года изменения в сервисе Microsoft Pay будут влиять нна расширение Microsoft Pay в Microsoft [!INCLUDE[d365fin](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="64d46-104">Effective February 8 2020, changes in the Microsoft Pay service will affect the Microsoft Pay extension in Microsoft [!INCLUDE[d365fin](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="64d46-105">Из-за изменений после 8 февраля ссылка **Оплатить**, которую расширение Microsoft Pay генерирует для счетов в [!INCLUDE[d365fin](includes/d365fin_md.md)], не будет открывать Microsoft Pay.</span><span class="sxs-lookup"><span data-stu-id="64d46-105">Due to the changes, after February 8, the **Pay now** payment links that the Microsoft Pay extension generates for invoices in [!INCLUDE[d365fin](includes/d365fin_md.md)] will not open Microsoft Pay.</span></span> <span data-ttu-id="64d46-106">Клиенты, которые используют расширение, должны изменить свои настройки службы платежей, чтобы вместо этого использовать расширение PayPal.</span><span class="sxs-lookup"><span data-stu-id="64d46-106">Customers who are using the extension should change their Payment Services setup to start using the PayPal extension instead.</span></span><br /></br>
>
> <span data-ttu-id="64d46-107">С 8 января мы будем отображать уведомление в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="64d46-107">From January 8, we will display a notification in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="64d46-108">Уведомление будет содержать ссылку на параметры, которые необходимо изменить, и дополнительную информацию.</span><span class="sxs-lookup"><span data-stu-id="64d46-108">The notification will contain a link to the settings that you need to change and to more information.</span></span> <span data-ttu-id="64d46-109">После 8 февраля расширение Microsoft Pay больше не будет доступно в [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="64d46-109">After February 8, the Microsoft Pay extension will no longer be available in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span><br /></br>
>
> <span data-ttu-id="64d46-110">Изменения коснулись следующих версий Business Central:</span><span class="sxs-lookup"><span data-stu-id="64d46-110">The changes impact the following versions of Business Central:</span></span>
> - <span data-ttu-id="64d46-111">Microsoft Dynamics 365 Business Central, октябрь 2018</span><span class="sxs-lookup"><span data-stu-id="64d46-111">Microsoft Dynamics 365 Business Central October 2018</span></span>
> - <span data-ttu-id="64d46-112">Microsoft Dynamics 365 Business Central, апрель 2019</span><span class="sxs-lookup"><span data-stu-id="64d46-112">Microsoft Dynamics 365 Business Central April 2019</span></span>
> - <span data-ttu-id="64d46-113">Microsoft Dynamics 365 Business Central 2019, выпуск волны 2</span><span class="sxs-lookup"><span data-stu-id="64d46-113">Microsoft Dynamics 365 Business Central 2019 Release Wave 2</span></span>

<span data-ttu-id="64d46-114">Клиенты постоянно требуют более высокого качества обслуживания как с точки зрения качества продукции, так и с точки зрения вариантов доставки и оплаты.</span><span class="sxs-lookup"><span data-stu-id="64d46-114">Customers continuously require higher customer service, both in terms of the quality of product but also in terms of delivery and payment services.</span></span> <span data-ttu-id="64d46-115">Служба платежей Microsoft Pay помогает улучшить качество обслуживания.</span><span class="sxs-lookup"><span data-stu-id="64d46-115">The Microsoft Pay service helps you increase your customer service.</span></span>

<span data-ttu-id="64d46-116">Расширение Microsoft Pay добавляет ссылку Microsoft Pay в ваши документы продажи, чтобы клиент мог легко заплатить с помощью Microsoft Pay.</span><span class="sxs-lookup"><span data-stu-id="64d46-116">The Microsoft Pay extension adds a Microsoft Pay link to your sales documents so customers can easily pay using Microsoft Pay.</span></span> <span data-ttu-id="64d46-117">Затем можно отправить документы по электронной почте для обеспечения более высокого уровня обслуживания клиентов и сократить время, требуемое для поступления платежей клиентов на ваш банковский счет.</span><span class="sxs-lookup"><span data-stu-id="64d46-117">Then you can send the documents by email to provide higher customer service and shorten the time it takes for customers’ payments to arrive on your bank account.</span></span>

<span data-ttu-id="64d46-118">Расширение Microsoft Pay предоставляет следующие преимущества:</span><span class="sxs-lookup"><span data-stu-id="64d46-118">The Microsoft Pay extension provides the following benefits:</span></span>
- <span data-ttu-id="64d46-119">Платежи клиентов быстрее отображаются на вашем банковском счете.</span><span class="sxs-lookup"><span data-stu-id="64d46-119">Customer payments appear faster on your bank account.</span></span>
- <span data-ttu-id="64d46-120">У клиентов есть больше способов оплачивать счета.</span><span class="sxs-lookup"><span data-stu-id="64d46-120">Customers have more ways to pay invoices.</span></span>
- <span data-ttu-id="64d46-121">Microsoft Pay предлагает надежную службу платежей, которой клиенты отдают предпочтение по сравнению с вводом данных кредитных карт на неизвестных веб-сайтах.</span><span class="sxs-lookup"><span data-stu-id="64d46-121">Microsoft Pay offers a trustworthy payment service, which customers prefer to entering credit card information on unknown web sites.</span></span>
- <span data-ttu-id="64d46-122">Microsoft Pay предлагает несколько способов обработки платежей, в том числе обработку кредитных карт, таких как PayPal и Stripe.</span><span class="sxs-lookup"><span data-stu-id="64d46-122">Microsoft Pay offers multiple ways of handling payments, including credit card processing, such as PayPal and Stripe.</span></span>
- <span data-ttu-id="64d46-123">Ссылка Microsoft Pay может автоматически внедряться в каждый документ счета или пользователем.</span><span class="sxs-lookup"><span data-stu-id="64d46-123">The Microsoft Pay link can be embedded automatically on every invoice document or by the user.</span></span>
- <span data-ttu-id="64d46-124">Поскольку данная функция построена как расширение, ее можно свободно включать тогда, когда это нужно для ваших бизнес-процессов.</span><span class="sxs-lookup"><span data-stu-id="64d46-124">Because this functionality is built as an extension, it gives you full control to enable it when and if your business processes require it.</span></span>

<span data-ttu-id="64d46-125">Включение расширения службы платежей в [!INCLUDE[d365fin](includes/d365fin_md.md)] бесплатно, однако вам потребуется связаться со службой платежей для получения учетной записи.</span><span class="sxs-lookup"><span data-stu-id="64d46-125">Enabling payment service extensions is free in [!INCLUDE[d365fin](includes/d365fin_md.md)], however, you will need to contact the payment service to get an account.</span></span> <span data-ttu-id="64d46-126">Дополнительные сведения см. в разделе [Включение платежей клиентов через службу платежей](sales-how-enable-payment-service-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="64d46-126">For more information, see [Enable Customer Payment Through Payment Services](sales-how-enable-payment-service-extensions.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="64d46-127">См. также</span><span class="sxs-lookup"><span data-stu-id="64d46-127">See Also</span></span>
<span data-ttu-id="64d46-128">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="64d46-128">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="64d46-129">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="64d46-129">Setting Up Sales</span></span>](sales-setup-sales.md)  
<span data-ttu-id="64d46-130">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="64d46-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
