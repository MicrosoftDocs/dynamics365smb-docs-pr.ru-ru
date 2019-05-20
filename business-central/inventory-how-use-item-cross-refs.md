---
title: Использование перекрестных ссылок на товары | Документы Майкрософт
description: Если настроить перекрестную ссылку между описанием товара, которое вы используете для товара, и описанием, которое использует поставщик этого товара, то описание товара поставщика автоматически вставляется в документы покупки для поставщика, когда вы заполняете **Номер перекрестной ссылки**. .
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: ca9f31b737fbd81bd1abba2a942301d0c9c919a6
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1244049"
---
# <a name="use-item-cross-references"></a>Использование перекрестных ссылок по товару
Если настроить перекрестную ссылку между описанием товара, которое вы используете для товара, и описанием, которое использует поставщик этого товара, то описание товара поставщика автоматически вставляется в документы покупки для поставщика, когда вы заполняете **Номер перекрестной ссылки**. . Такая же функция применяется для номеров товаров клиента в документах продажи.

В приведенных ниже процедурах описано, как использовать перекрестные ссылки товара на стороне покупки. Действия на стороне продажи аналогичны.

## <a name="to-set-up-an-item-cross-reference-to-a-vendors-item-description"></a>Настройка перекрестной ссылки товара на описание товара поставщика
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите связанную ссылку.
2. Откройте карточку для товара, для которого требуется создать перекрестную ссылку на описание товара, которое используется поставщиком для данного товара.
3. Выберите действие **Перекрестные ссылки**.
4. В новой строке на странице **Описание перекрестных ссылок по товару** заполните поля требуемыми данными. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].

## <a name="to-enter-a-vendors-item-description-on-a-purchase-order"></a>Ввод описания товара поставщика в заказ на покупку
1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на покупку**, затем выберите связанную ссылку.
2. Создайте заказ на покупку для поставщика, для которого вы настроили перекрестную ссылку товара в предыдущей процедуре.
3. Создайте строку покупки для товара, для которого вы настроили перекрестную ссылку товара в предыдущей процедуре.
4. В поле **Номер перекрестной ссылки** выберите перекрестную ссылку товара, которая была создана, затем выберите кнопку **ОК**.

Поле **Описание** в строке перезаписывается описанием товара поставщика согласно настройкам в перекрестной ссылке товара.

## <a name="see-also"></a>См. также
[Регистрация новых товаров](inventory-how-register-new-items.md)  
[Наличие](inventory-manage-inventory.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)