---
title: Использование выставления счетов и Business Central
description: Обходное решение для доступа к Microsoft Invoicing при регистрации на Dynamics 365 Business Central.
author: brentholtorf
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Invoicing, Microsoft 365
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: 53216f530c5e0f334f2ffb9f96f12c9804d8ad48
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "8520000"
---
# <a name="use-the-same-microsoft-365-account-in-prod_short-and-microsoft-invoicing"></a>Использование одной и той же учетной записи Microsoft 365 в [!INCLUDE[prod_short](includes/prod_long.md)] и Microsoft Invoicing
При регистрации на пробную версию [!INCLUDE[prod_short](includes/prod_short.md)] можно перейти на 30-дневную фазу оценки, начать подписку или прекратить использование [!INCLUDE[prod_short](includes/prod_short.md)]. Во всех случаях возможно, что вы в какой-то момент увидели что-то под названием **Microsoft Invoicing** и щелкнули соответствующую плитку. Это было приложение, которое входило в состав того, что сейчас называется подпиской Microsoft 365 Business Standard (а раньше называлось Microsoft 365 Business Premium), поэтому видеть эту плитку в своем интерфейсе Microsoft 365 могли не все.  

Microsoft Invoicing больше не предоставляется, однако если вам нужно войти в Invoicing, чтобы извлечь свои данные, вы можете увидеть сообщение о невозможности доступа Microsoft Invoicing из-за того, что ваша учетная запись используется в [!INCLUDE[prod_short](includes/prod_short.md)].  

Подобное сообщение отображается при установке мобильного приложения для Invoicing.  

## <a name="workaround"></a>Обходное решение
Invoicing и [!INCLUDE[prod_short](includes/prod_short.md)] используют одну и ту же платформу. Это означает, что вы распознаетесь как существующий пользователь [!INCLUDE[prod_short](includes/prod_short.md)] при нажатии пункта Invoicing в центре администрирования Microsoft 365. Причиной этого является то, что Invoicing не может использовать ту же организацию, что и [!INCLUDE[prod_short](includes/prod_short.md)].  

Поэтому вам следует выполнить вход в [!INCLUDE[prod_short](includes/prod_short.md)] и переименовать существующую организацию, а затем создать новую организацию, которую можно использовать в Invoicing. В этом обходном решении данные не перемещаются и не перезаписываются.

### <a name="to-rename-your-company"></a>Переименование организации
1. Выполните вход в [!INCLUDE[prod_short](includes/prod_short.md)].
2. В правом верхнем углу щелкните значок **Параметры** ![Параметры](media/ui-experience/settings_icon_small.png "Значок настроек для ролевого центра"), затем выберите **Мои настройки**.
3. В поле **Организация** выберите другую организацию.
4. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Компании**, а затем выберите связанную ссылку.  
5. На странице **Организации** выберите **Изменить список**.  
6. Измените имя записи *Моя организация* на другое.  

    Подождите несколько минут. Будут внесены некоторые изменения в основную базу данных, что займет некоторое время.
7.  После того, как система будет готова к работе, нажмите кнопку **Создать новую организацию**.  
8.  В открывшемся диалоговом окне укажите имя как *Моя организация* и выберите параметр **Производственный выпуск — только данные настройки**.  

Выполнение этой операции также займет несколько минут. По завершении процесса можно будет получить доступ к Invoicing в рамках Microsoft 365 Business Standard. но только для экспорта данных, так как приложение Invoicing устарело.  

### <a name="what-about-my-data"></a>Что происходит с данными?
При переименовании имени первоначальной организации таблицы баз данных, в которых хранятся существующие данные [!INCLUDE[prod_short](includes/prod_short.md)], будут переименованы, но сами данные не будут изменены.  

Если используется и Invoicing, и [!INCLUDE[prod_short](includes/prod_short.md)], данные хранятся в двух различных контейнерах (двух организациях). Данные не используются совместно, поэтому потребуется управлять клиентами и товарами в обеих организациях.  

## <a name="see-also"></a>См. также
[Вопросы и ответы](across-faq.yml)  
[Администрация](admin-setup-and-administration.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]