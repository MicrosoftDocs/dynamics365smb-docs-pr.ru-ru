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
# <a name="the-microsoft-pay-extension"></a>Расширение Microsoft Pay

> [!IMPORTANT]
> Начиная с 8 февраля 2020 года изменения в сервисе Microsoft Pay будут влиять нна расширение Microsoft Pay в Microsoft [!INCLUDE[d365fin](includes/d365fin_long_md.md)]. Из-за изменений после 8 февраля ссылка **Оплатить**, которую расширение Microsoft Pay генерирует для счетов в [!INCLUDE[d365fin](includes/d365fin_md.md)], не будет открывать Microsoft Pay. Клиенты, которые используют расширение, должны изменить свои настройки службы платежей, чтобы вместо этого использовать расширение PayPal.<br /></br>
>
> С 8 января мы будем отображать уведомление в [!INCLUDE[d365fin](includes/d365fin_md.md)]. Уведомление будет содержать ссылку на параметры, которые необходимо изменить, и дополнительную информацию. После 8 февраля расширение Microsoft Pay больше не будет доступно в [!INCLUDE[d365fin](includes/d365fin_md.md)].<br /></br>
>
> Изменения коснулись следующих версий Business Central:
> - Microsoft Dynamics 365 Business Central, октябрь 2018
> - Microsoft Dynamics 365 Business Central, апрель 2019
> - Microsoft Dynamics 365 Business Central 2019, выпуск волны 2

Клиенты постоянно требуют более высокого качества обслуживания как с точки зрения качества продукции, так и с точки зрения вариантов доставки и оплаты. Служба платежей Microsoft Pay помогает улучшить качество обслуживания.

Расширение Microsoft Pay добавляет ссылку Microsoft Pay в ваши документы продажи, чтобы клиент мог легко заплатить с помощью Microsoft Pay. Затем можно отправить документы по электронной почте для обеспечения более высокого уровня обслуживания клиентов и сократить время, требуемое для поступления платежей клиентов на ваш банковский счет.

Расширение Microsoft Pay предоставляет следующие преимущества:
- Платежи клиентов быстрее отображаются на вашем банковском счете.
- У клиентов есть больше способов оплачивать счета.
- Microsoft Pay предлагает надежную службу платежей, которой клиенты отдают предпочтение по сравнению с вводом данных кредитных карт на неизвестных веб-сайтах.
- Microsoft Pay предлагает несколько способов обработки платежей, в том числе обработку кредитных карт, таких как PayPal и Stripe.
- Ссылка Microsoft Pay может автоматически внедряться в каждый документ счета или пользователем.
- Поскольку данная функция построена как расширение, ее можно свободно включать тогда, когда это нужно для ваших бизнес-процессов.

Включение расширения службы платежей в [!INCLUDE[d365fin](includes/d365fin_md.md)] бесплатно, однако вам потребуется связаться со службой платежей для получения учетной записи. Дополнительные сведения см. в разделе [Включение платежей клиентов через службу платежей](sales-how-enable-payment-service-extensions.md).

## <a name="see-also"></a>См. также
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  
[Настройка продаж](sales-setup-sales.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
