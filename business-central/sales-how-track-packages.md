---
title: Как осуществить трассировку посылок | Документация Майкрософт
description: Используйте службу отслеживания экспедиторов для контроля хода доставки.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: rfq
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 5136c675d50e4d9ac91f43755dfb44810701096d
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "4758021"
---
# <a name="track-packages"></a><span data-ttu-id="0d2c1-103">Трассировка посылок</span><span class="sxs-lookup"><span data-stu-id="0d2c1-103">Track Packages</span></span>

<span data-ttu-id="0d2c1-104">Некоторые экспедиторы предоставляют через Интернет услуги, позволяющие отслеживать упаковки, переданные этому агенту.</span><span class="sxs-lookup"><span data-stu-id="0d2c1-104">A number of shipping agents provide services on the Internet that allow you to track parcels you have handed over to the agent.</span></span> <span data-ttu-id="0d2c1-105">Если организация пользуется услугами одного или нескольких таких экспедиторов, в программе можно настроить определенную базовую информацию и использовать функцию автоматической трассировки для учтенных отгрузок, учтенных счетов продажи, учтенных кредит-нот продажи и учтенных возвратных приходных накладных.</span><span class="sxs-lookup"><span data-stu-id="0d2c1-105">If you use one or more of these shipping agents, you can set up certain basic information and use the automatic tracking feature from posted shipments, posted sales invoices, posted sales credit memos, and posted return receipts.</span></span> <span data-ttu-id="0d2c1-106">Дополнительные сведения см. в разделе [Настройка экспедиторов](sales-how-to-set-up-shipping-agents.md).</span><span class="sxs-lookup"><span data-stu-id="0d2c1-106">For more information, see [Set Up Shipping Agents](sales-how-to-set-up-shipping-agents.md).</span></span>  

<span data-ttu-id="0d2c1-107">В следующей процедуре показано, как отслеживать пакет из учтенной расходной накладной продажи, но те же шаги применяются для включения отслеживания пакетов со страниц "Учтенный счет продажи", "Учтенная кредит-нота продажи" и "Учтенная возвратная приходная накладная".</span><span class="sxs-lookup"><span data-stu-id="0d2c1-107">The following procedure shows how to track a package from a posted sales shipment, but the same steps apply to enable package tracking from the Posted Sales Invoice, Posted Sales Credit Memo, and Posted Return Receipt pages.</span></span>  

## <a name="to-track-a-package"></a><span data-ttu-id="0d2c1-108">Трассировка посылки</span><span class="sxs-lookup"><span data-stu-id="0d2c1-108">To track a package</span></span>

1. <span data-ttu-id="0d2c1-109">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенная расх. накладная продажи**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="0d2c1-109">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Sales Shipment**, and then choose the related link.</span></span>
2. <span data-ttu-id="0d2c1-110">Откройте соответствующую расходную накладную.</span><span class="sxs-lookup"><span data-stu-id="0d2c1-110">Open the relevant shipment.</span></span>
3. <span data-ttu-id="0d2c1-111">Выберите действие **Обновить документ**.</span><span class="sxs-lookup"><span data-stu-id="0d2c1-111">Choose the **Update Document** action.</span></span>
4. <span data-ttu-id="0d2c1-112">В поле **Номер трасс. посылки**</span><span class="sxs-lookup"><span data-stu-id="0d2c1-112">In the **Package Tracking No.**</span></span> <span data-ttu-id="0d2c1-113">укажите номер посылки, полученный от экспедитора.</span><span class="sxs-lookup"><span data-stu-id="0d2c1-113">field, enter the package number you have received from the shipping agent.</span></span> <span data-ttu-id="0d2c1-114">При необходимости обновите значение в поле **Экспедитор** и закройте страницу.</span><span class="sxs-lookup"><span data-stu-id="0d2c1-114">Update **Shipping Agent** if needed and close the page.</span></span>
5. <span data-ttu-id="0d2c1-115">Выберите действие **Трассировать пакет**.</span><span class="sxs-lookup"><span data-stu-id="0d2c1-115">Choose the **Track Package** action.</span></span>

<span data-ttu-id="0d2c1-116">Браузер по умолчанию открывает страницу отслеживания экспедитора.</span><span class="sxs-lookup"><span data-stu-id="0d2c1-116">Your default browser opens the shipping agent's tracking page.</span></span>

## <a name="see-also"></a><span data-ttu-id="0d2c1-117">См. также</span><span class="sxs-lookup"><span data-stu-id="0d2c1-117">See Also</span></span>

[<span data-ttu-id="0d2c1-118">Настройка экспедиторов</span><span class="sxs-lookup"><span data-stu-id="0d2c1-118">Set Up Shipping Agents</span></span>](sales-how-to-set-up-shipping-agents.md)  
[<span data-ttu-id="0d2c1-119">Продажи</span><span class="sxs-lookup"><span data-stu-id="0d2c1-119">Sales</span></span>](sales-manage-sales.md)  
[<span data-ttu-id="0d2c1-120">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="0d2c1-120">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="0d2c1-121">Отправка документов по электронной почте</span><span class="sxs-lookup"><span data-stu-id="0d2c1-121">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
<span data-ttu-id="0d2c1-122">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="0d2c1-122">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>
