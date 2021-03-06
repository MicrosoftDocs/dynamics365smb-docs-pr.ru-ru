---
title: Немедленное создание счетов покупки
description: В случае потребности в оплате поставщику наличными или чеком, необходимый учет можно производить при учете самого счета.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: d7962031aa7dda7dafa96ade8e11339c06ebb305
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5784596"
---
# <a name="settle-purchase-invoices-promptly"></a>Немедленное создание счетов покупки

В случае потребности в оплате поставщику наличными или чеком, платеж можно учесть при учете счета.  

> [!NOTE]  
> Если оплата счетов наличными, чеком или банковским переводом производится часто, то можно рекомендовать установить специальный метод оплаты с использованием балансирующего счета и ввода этого метода в поле **Способ платежа** на карточке поставщика. Номер балансирующего счета вставляется автоматически в заголовок счета при создании нового счета. Дополнительные сведения см. в разделе [Определение способов оплаты](finance-payment-methods.md).  

## <a name="to-settle-purchase-invoices-promptly"></a>Немедленное создание счетов покупки

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета покупки**, затем выберите соответствующую ссылку.  
2. Выберите действие **Создать**.  
3. Для того чтобы произвести оплату наличными или с помощью банковского трансферта, следует ввести номер счета ГК или банковского счета в поле **Номер баланс. счета**.  

> [!IMPORTANT]  
> Поля **Тип баланс. счета** и **Номер баланс. счета** не включены в стандартную схему заголовка счета. Чтобы разнести оплату счета, вы должны связаться с партнером Microsoft, который может добавить поля с помощью кода.  
>
> Эта настройка требуется только в том случае, если вы не укажете балансирующие счета в способах оплаты, как описано выше.

## <a name="see-also"></a>См. также

[Управление кредиторской задолженностью](payables-manage-payables.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]