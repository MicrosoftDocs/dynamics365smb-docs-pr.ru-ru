---
title: Использование Invoicing и Business Central | Документы Майкрософт
description: Обходное решение для доступа к Microsoft Invoicing при регистрации на Dynamics 365 Business Central.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Invoicing, Office 365
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: 0173d64e140cfea91bf7f08d821c2d30cf0eb7b3
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241488"
---
# <a name="using-the-same-office-365-account-in-included365finincludesd365finlongmdmd-and-microsoft-invoicing"></a>Использование одной и той же учетной записи Office 365 в [!INCLUDE[d365fin](includes/d365fin_long_md.md)] и Microsoft Invoicing
При регистрации на пробную версию [!INCLUDE[d365fin](includes/d365fin_md.md)] можно перейти на 30-дневную фазу оценки, начать подписку или прекратить использование [!INCLUDE[d365fin](includes/d365fin_md.md)]. Во всех случаях при входе на портал Office может отобразиться плитка **Microsoft Invoicing**, которую можно нажать. Это часть подписки Office 365 Business Premium, поэтому не все пользователи увидят эту плитку на портале Office.  

Если открыть Microsoft Invoicing, отобразится сообщение о невозможности получить доступ к Microsoft Invoicing, поскольку ваша учетная запись используется в [!INCLUDE[d365fin](includes/d365fin_md.md)].  

Подобное сообщение отображается при установке мобильного приложения для Invoicing.  

## <a name="workaround"></a>Обходное решение
Invoicing и [!INCLUDE[d365fin](includes/d365fin_md.md)] используют одну и ту же платформу. Это означает, что вы распознаетесь как существующий пользователь [!INCLUDE[d365fin](includes/d365fin_md.md)] при нажатии Invoicing на портале Office. Причиной этого является то, что Invoicing не может использовать ту же организацию, что и [!INCLUDE[d365fin](includes/d365fin_md.md)].  

Поэтому вам следует выполнить вход в [!INCLUDE[d365fin](includes/d365fin_md.md)] и переименовать существующую организацию, а затем создать новую организацию, которую можно использовать в Invoicing. В этом обходном решении данные не перемещаются и не перезаписываются.

### <a name="to-rename-your-company"></a>Переименование организации
1. Выполните вход в [!INCLUDE[d365fin](includes/d365fin_md.md)].
2. В правом верхнем углу щелкните значок **Параметры** ![Параметры](media/ui-experience/settings_icon_small.png "Значок \"Параметры\" для ролевого центра"), а затем выберите **Мои настройки**.
3. В поле **Организация** выберите другую организацию.
4. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Компании**, затем выберите связанную ссылку.  
5. На странице **Организации** выберите **Изменить список**.  
6. Измените имя записи *Моя организация* на другое.  

    Подождите несколько минут. Будут внесены некоторые изменения в основную базу данных, что займет некоторое время.
7.  После того, как система будет готова к работе, нажмите кнопку **Создать новую организацию**.  
8.  В открывшемся диалоговом окне укажите имя как *Моя организация* и выберите параметр **Производственный выпуск — только данные настройки**.  

Выполнение этой операции также займет несколько минут. По завершении процесса можно будет получить доступ к Invoicing в рамках Office 365 Business Premium.  

### <a name="what-about-my-data"></a>Что происходит с данными?
При переименовании имени первоначальной организации таблицы баз данных, в которых хранятся существующие данные [!INCLUDE[d365fin](includes/d365fin_md.md)], будут переименованы, но сами данные не будут изменены.  

Если используется и Invoicing, и [!INCLUDE[d365fin](includes/d365fin_md.md)], данные хранятся в двух различных контейнерах (двух организациях). Данные не используются совместно, поэтому потребуется управлять клиентами и товарами в обеих организациях.  

## <a name="see-also"></a>См. также
[Вопросы и ответы](across-faq.md)  
[Администрация](admin-setup-and-administration.md)  
