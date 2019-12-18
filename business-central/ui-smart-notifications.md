---
title: Работа с умными уведомлениями и определение случаев, когда они должны отображаться | Документация Майкрософт
description: Вы можете получать уведомления об изменениях состояния или о событиях, например о просроченном платеже или о том, что запасы подходят к концу.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 11/29/2019
ms.author: bholtorf
ms.openlocfilehash: 4839de7b4deff107d8a1644367e28216eb8a789e
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881946"
---
# <a name="manage-notifications"></a><span data-ttu-id="58a69-103">Управление уведомлениями</span><span class="sxs-lookup"><span data-stu-id="58a69-103">Manage Notifications</span></span>

[!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="58a69-104">может помочь работать эффективнее, например уведомляя об определенных событиях или изменениях статуса, например, когда вы собираетесь выставить счет клиенту, у которого имеется просроченная задолженность, или когда доступные запасы ниже количества, которое вы собираетесь продать.</span><span class="sxs-lookup"><span data-stu-id="58a69-104">can help you work smarter by notifying you about certain events or changes in status, such as when you are about to invoice a customer who has an overdue balance, or the available inventory is lower than the quantity you are about to sell, for example.</span></span> <span data-ttu-id="58a69-105">Эти уведомления отображаются как разумные подсказки в контексте выполняемой вами задачи, и вы можете игнорировать уведомление или проверить сведения о проблеме.</span><span class="sxs-lookup"><span data-stu-id="58a69-105">These notifications are shown as discreet tips in the context of the task you are doing, and you can choose to ignore the notification or to see details about the issue.</span></span>  

<span data-ttu-id="58a69-106">Если вы решите посмотреть сведения для уведомления, вы можете выполнить действие для устранения проблемы, например связаться с клиентом, приобрести дополнительные складские запасы и т. д.</span><span class="sxs-lookup"><span data-stu-id="58a69-106">If you choose to see details for a notification, you can take action to resolve the issue, such as contacting the customer, buying more inventory, and so on.</span></span> <span data-ttu-id="58a69-107">Действия выбираете вы, а [!INCLUDE[d365fin](includes/d365fin_md.md)] дает советы и рекомендации.</span><span class="sxs-lookup"><span data-stu-id="58a69-107">It's your choice what to do, and [!INCLUDE[d365fin](includes/d365fin_md.md)] gives you advice and recommendations.</span></span>  

<span data-ttu-id="58a69-108">Уведомления помогают неопытным пользователям выполнять незнакомые задачи, не уменьшая производительности более опытных пользователей.</span><span class="sxs-lookup"><span data-stu-id="58a69-108">Notifications can help untrained users complete unfamiliar tasks, and do not reduce productivity for the more trained user.</span></span>  

## <a name="to-turn-notifications-on-or-off-and-control-when-they-are-sent"></a><span data-ttu-id="58a69-109">Включение и отключение уведомлений, а также управление временем их отправки</span><span class="sxs-lookup"><span data-stu-id="58a69-109">To turn notifications on or off, and control when they are sent</span></span>

<span data-ttu-id="58a69-110">При первом запуске [!INCLUDE[d365fin](includes/d365fin_md.md)] все уведомления включены, но их можно включить и отключить, например, если вы не заинтересованы в определенном событии или статусе.</span><span class="sxs-lookup"><span data-stu-id="58a69-110">When you first start with [!INCLUDE[d365fin](includes/d365fin_md.md)] all notifications are turned on, but you can turn them on or off, for example, if you aren't interested in a certain event or status.</span></span>  

<span data-ttu-id="58a69-111">Кроме того, некоторые уведомления позволяют указать условия их отправки.</span><span class="sxs-lookup"><span data-stu-id="58a69-111">Additionally, some notifications let you specify the conditions under which they are sent.</span></span> <span data-ttu-id="58a69-112">Например, если нужно получить уведомление при низком уровне запасов, но только для товаров, которые вы покупаете у определенного поставщика.</span><span class="sxs-lookup"><span data-stu-id="58a69-112">For example, if you want to be notified when inventory is running low, but only for items you buy from a certain vendor.</span></span>  

<span data-ttu-id="58a69-113">Включение и отключение уведомлений, а также указание условий применяется только к вам.</span><span class="sxs-lookup"><span data-stu-id="58a69-113">Turning notifications on or off, and specifying conditions, applies only to you.</span></span>  

1. <span data-ttu-id="58a69-114">В правом верхнем углу щелкните значок **Параметры** ![Параметры](media/ui-experience/settings_icon_small.png "Значок настроек для ролевого центра"), а затем выберите действие **Мои настройки**.</span><span class="sxs-lookup"><span data-stu-id="58a69-114">In the top right corner, choose the **Settings** icon ![Settings](media/ui-experience/settings_icon_small.png "Settings icon for role center"), and then choose the **My Settings** action.</span></span>  
2. <span data-ttu-id="58a69-115">На странице **Мои настройки** в поле **Уведомления** выберите *Изменение времени получения уведомлений*</span><span class="sxs-lookup"><span data-stu-id="58a69-115">On the **My Settings** page, in the **Notifications** field, choose the *Change when I receive notifications.*</span></span> <span data-ttu-id="58a69-116">.</span><span class="sxs-lookup"><span data-stu-id="58a69-116">link.</span></span>  
3. <span data-ttu-id="58a69-117">На открывшейся странице включите или отключите уведомление, выбрав или сняв флажок **Включено**.</span><span class="sxs-lookup"><span data-stu-id="58a69-117">In the page that appears, turn on or turn off a notification by selecting or clearing the **Enabled** check box.</span></span>  
4. <span data-ttu-id="58a69-118">Чтобы указать условия, которые вызывают уведомление, перейдите по ссылке **Просмотр сведений фильтра** и заполните поля.</span><span class="sxs-lookup"><span data-stu-id="58a69-118">To specify conditions that trigger a notification, choose the **View filter details** link, and then fill in the fields.</span></span>  

## <a name="see-also"></a><span data-ttu-id="58a69-119">См. также</span><span class="sxs-lookup"><span data-stu-id="58a69-119">See Also</span></span>

<span data-ttu-id="58a69-120">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="58a69-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
