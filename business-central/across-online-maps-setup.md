---
title: Настройка онлайн-карт
description: Узнайте, как настроить Business Central, чтобы предлагать маршруты и информацию о местоположении с помощью службы онлайн-карт.
author: rubenseishima
ms.service: dynamics365-business-central
ms.topic: article
ms.search.form: 800, 804
ms.date: 07/15/2022
ms.author: a-reishima
ms.openlocfilehash: 1fe92e5ba9ba28e8999e5f8487048f9df9d6d14c
ms.sourcegitcommit: 8b95e1700a9d1e5be16cbfe94fdf7b660f1cd5d7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2022
ms.locfileid: "9461304"
---
# <a name="set-up-online-maps"></a>Настройка онлайн-карт

Когда, например, планируется визит по адресу, сохраненному в карточке, например к клиенту, можно получить карту из службы интерактивных карт с описанием маршрутов на выбранном языке. Чтобы карта и маршрут, найденные службой интерактивных карт, были правильными, эту службу необходимо настроить в [!INCLUDE[prod_short](includes/prod_short.md)].

## <a name="set-up-the-online-map-feature"></a>Настройка функции онлайн-карты

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать 1.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Настройка онлайн-карты**, а затем выберите соответствующую ссылку.
2. На странице **Настройка онлайн-карты** заполните следующие поля. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]
3. Включите переключатель **Включено**.

### <a name="customize-the-online-map-provider-features"></a>Настройка функций поставщика онлайн-карт

Чтобы настроить функцию онлайн-карты помимо параметров, перечисленных на странице **Настройка онлайн-карты**, или для использования другого поставщика карт выполните следующие действия:

1. На странице **Настройка онлайн-карты** выберите действие **Настройка параметров**.
2. На странице **Настройка параметров онлайн-карты** выберите действие **Новый**.
3. Заполните поля, чтобы настроить способ, которым [!INCLUDE[prod_short](includes/prod_short.md)] будет генерировать URL-адреса для доступных сервисов. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]
   * См. перечень **Параметров замены онлайн-карты** на **Информационной панели**, чтобы получить данные, доступные для создания URL-адресов.

## <a name="see-also"></a>См. также

[Использование онлайн-карт для поиска местоположений и составления маршрутов](across-online-maps.md)  
[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  
[Администрация](admin-setup-and-administration.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
