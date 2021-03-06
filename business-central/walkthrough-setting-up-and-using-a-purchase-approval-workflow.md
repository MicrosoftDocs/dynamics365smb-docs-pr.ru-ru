---
title: Настройка и использование рабочего процесса утверждения покупки
description: Можно автоматизировать процесс утверждения новых или измененных записей, например документов, строк журнала и карточек клиента, путем создания рабочих процессов с шагами для соответствующих утверждений. Перед созданием рабочих процессов утверждения необходимо задать утверждающего и заместителя утверждающего для каждого пользователя. Также можно установить предельные суммы для утверждающих, чтобы определить, какие записи продаж и покупок им разрешается утверждать. Запросы на утверждение и другие уведомления можно отправлять по электронной почте или как внутренние записки. Для каждого пользователя также можно указать время получения ими уведомлений.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 05/26/2021
ms.author: edupont
ms.openlocfilehash: 964e1dae3dc754198777c703a15c1ef0b6fe82a7
ms.sourcegitcommit: 6bce51954f17b80491e180f25d67ff18b1618a88
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "6110983"
---
# <a name="walkthrough-setting-up-and-using-a-purchase-approval-workflow"></a>Пошаговое руководство. Настройка и использование рабочего процесса утверждения покупки

Можно автоматизировать процесс утверждения новых или измененных записей, например документов, строк журнала и карточек клиента, путем создания рабочих процессов с шагами для соответствующих утверждений. Перед созданием рабочих процессов утверждения необходимо задать утверждающего и заместителя утверждающего для каждого пользователя. Также можно установить предельные суммы для утверждающих, чтобы определить, какие записи продаж и покупок им разрешается утверждать. Запросы на утверждение и другие уведомления можно отправлять по электронной почте или как внутренние записки. Для каждого пользователя также можно указать время получения ими уведомлений.

> [!NOTE]
> В дополнение к функции рабочих процессов в [!INCLUDE[prod_short](includes/prod_short.md)], можно использовать Power Automate для определения рабочих процессов для событий в [!INCLUDE[prod_short](includes/prod_short.md)]. Обратите внимание, что хотя это две отдельных системы рабочих процессов, любой шаблон потока, созданный в Power Automate, добавляется в список шаблонов рабочих процессов в [!INCLUDE[prod_short](includes/prod_short.md)]. Дополнительные сведения см. в разделе [Использование Business Central в автоматическом бизнес-процессе](across-how-use-financials-data-source-flow.md).  

 Можно настроить и использовать рабочие процессы, связывающие задачи бизнес-процесса, выполняемые различными пользователями. Системные задачи, такие как автоматический учет, могут включаться в качестве шагов рабочего процесса, предшествующих задачам пользователя или выполняемых после них. Типичные шаги рабочего процесса – запрос и выдача разрешения на создание новых записей. Дополнительные сведения см. в разделе [Рабочий процесс](across-workflow.md).  

## <a name="about-this-walkthrough"></a>Об этом пошаговом руководстве

В этом пошаговом руководстве рассматриваются следующие задачи:  

- Настройка пользователей утверждения  
- Настройка уведомлений для пользователей утверждения  
- Изменение и включение рабочего процесса утверждения  
- Запрос утверждения заказа на покупку, как у Алисии  
- Получение уведомления с утверждением запроса, как у Шона  

## <a name="story"></a>Сюжет

Шон – привилегированный пользователь CRONUS. Он создает два пользователя утверждения. Один – Алисия, которая представляет агента по закупкам. Другой — сам Шон, который представляет утверждающего для Алисии. Шон дает себе неограниченные права на утверждение покупок и указывает, что он должен получать уведомления в форме внутренних записок сразу при возникновении соответствующего события. Наконец, Шон создает требуемый рабочий процесс утверждения как копию существующего шаблона рабочего процесса утверждения заказов на покупку, оставляет все существующие условия наступления событий и параметры отклика без изменений, а затем включает рабочий процесс.  

Для тестирования рабочего процесса утверждения Шон сначала входит в [!INCLUDE[prod_short](includes/prod_short.md)] под именем Алисии и запрашивает утверждение заказа на покупку. Затем Шон входит в систему под своим именем, видит записку в своем ролевом центре, переходит по ссылке к запросу на утверждение заказа на покупку и утверждает этот запрос.  

## <a name="users"></a>Пользователи

Прежде чем можно будет настроить пользователей утверждения и способ их уведомления, следует убедиться, что два пользователя существуют в [!INCLUDE[prod_short](includes/prod_short.md)]: один пользователь будет представлять Алисию. Другой пользователь (вы сами), будет представлять Шона. Для получения дополнительной информации см. раздел [Создание пользователей в соответствии с лицензиями](ui-how-users-permissions.md).

### <a name="setting-up-approval-users"></a>Настройка пользователей утверждения

Войдя в систему в качестве самого себя, настройте Алисию как пользователя утверждения, утверждающим которого будите вы сами. Настройте права утверждения и укажите, как и когда вы будете получать уведомления о запросах на утверждение.  

#### <a name="to-set-up-yourself-and-alicia-as-approval-users"></a>Чтобы указать себя и Алисию в качестве пользователей утверждения

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка пользователя для утверждений**, затем выберите соответствующую ссылку.  
2. На странице **Настройка пользователя для утверждений** выберите действие **Создать**.  

    > [!NOTE]  
    >  Следует настроить утверждающего до того, как настраивать пользователей, которым требуется утверждение этого утверждающего лица. Таким образом, до настройки данных Алисии необходимо настроить свои данные.  

3. Настройте двух пользователей утверждения, заполнив поля, как указано в следующей таблице.  

    |ИД пользователя|Код утверждающего|Утверждение закупок без ограничений|  
    |-------------|-----------------|---------------------------------|  
    |ВЫ||Выбрано|  
    |АЛИСИЯ|ВЫ||  

### <a name="setting-up-notifications"></a>Настройка уведомления

В этом пошаговом руководстве пользователь уведомляется внутренней заметкой о запросах, которые требуется утвердить. Уведомление об утверждении также может быть отправлено по электронной почте, и вы можете добавить шаг отклика рабочего процесса, который уведомляет отправителя, когда запрос утвержден или отклонен. Дополнительные сведения см. в разделе [Определение сроков и порядка получения уведомлений пользователями](across-how-to-specify-when-and-how-to-receive-notifications.md).

#### <a name="to-set-up-how-and-when-you-are-notified"></a>Чтобы настроить способ и момент получения уведомлений

1. На странице **Настройка пользователя для утверждений** выберите для себя строку, затем выберите действие **Настройка уведомлений**.  
2. На странице **Настройка уведомлений** в поле **Тип уведомления** выберите **Утверждение**.  
3. В поле **Метод уведомления** выберите **Заметка**.  
4. На странице **Настройка уведомлений** выберите действие **График уведомлений**.  
5. На странице **График уведомлений** в поле **Повторение** выберите **Сразу**.  

## <a name="creating-the-approval-workflow"></a>Создание рабочего процесса утверждения

Создайте рабочий процесс утверждения заказа на покупку путем копирования шагов из шаблона рабочего процесса **Утверждение заказа на покупку**. Оставьте шаги существующего рабочего процесса без изменений, а затем включите этот рабочий процесс.  

> [!TIP]
> Если требуется, добавьте шаг отклика рабочего процесса, чтобы уведомить отправителя, когда его запрос был утвержден или отклонен. Дополнительные сведения см. в разделе [Определение сроков и порядка получения уведомлений пользователями](across-how-to-specify-when-and-how-to-receive-notifications.md).

### <a name="to-create-and-enable-a-purchase-order-approval-workflow"></a>Чтобы создать и включить рабочий процесс утверждения заказа на покупку

1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Рабочие процессы**, затем выберите соответствующую ссылку.  
2. На странице **Рабочие процессы** выберите **Действия**, затем выберите **Создать**, а затем выберите действие **Создать рабочий процесс из шаблона**.  
3. На странице **Шаблоны рабочих процессов** выберите шаблон рабочего процесса под именем **Рабочий процесс утверждения заказа на покупку**.  

    Откроется страница **Рабочий процесс** для нового рабочего процесса, содержащее всю информацию из выбранного шаблона. Значение в поле **Код** дополняется символами *-01*, которые указывают, что это первый рабочий процесс, созданный на основе шаблона рабочего процесса **Рабочий процесс утверждения заказа на покупку**.  
4. В заголовке страницы **Рабочий процесс** установите флажок **Включено**.  

## <a name="using-the-approval-workflow"></a>Использование рабочего процесса утверждения

Чтобы использовать новый рабочий процесс утверждения заказов на покупку, сначала войдите в [!INCLUDE[prod_short](includes/prod_short.md)] под именем Алисии, чтобы запросить утверждение заказа на покупку. Затем войдите в систему под своим именем, просмотрите записку в ролевом центре, перейдите по ссылке к запросу на утверждение, а затем утвердите запрос.  

### <a name="to-request-approval-of-a-purchase-order-as-alicia"></a>Чтобы запросить утверждение заказа на покупку от имени Алисии

1. Войдите от имени пользователя Алисия.
2. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы на покупку**, затем выберите соответствующую ссылку.  
3. Выберите строку, чтобы открыть заказ на покупку 106001.  
4. На странице **Заказ на покупку** выберите **Действия**, затем **Запросить утверждение**, а затем выберите действие **Отправить запрос на утверждение**.  

Обратите внимание, что значение в поле **Статус** изменено на **Ожидает утверждения**.  

### <a name="to-approve-the-purchase-order-as-sean"></a>Чтобы утвердить заказ на покупку от имени Шона

1. Войдите от имени пользователя Шон.
2. В ролевом центре в области **Самообслуживание**, выберите плитку **Запросы на утверждение**.
3. На странице **Запросы на утверждение** выберите строку о заказе на покупку от Алисии, затем выберите действие **Утвердить**.  

Значение в поле **Статус** заказа на покупку Алисии будет изменено на **Выпущено**.  

Вы настроили и протестировали простой рабочий процесс утверждения на основе первых двух шагов рабочего процесса утверждения заказа на покупку. Можно с легкостью расширить этот рабочий процесс таким образом, чтобы автоматически учесть заказ на покупку Алисии при его утверждении Шоном. Чтобы это сделать, необходимо включить рабочий процесс счета покупки, в котором откликом на выпущенный счет покупки является его учет. Сначала необходимо изменить условие события в первом шаге рабочего процесса с **Счет** (покупки) на **Заказ**.  

Универсальная версия [!INCLUDE[prod_short](includes/prod_short.md)] включает несколько шаблонов рабочего процесса для сценариев, которые поддерживаются кодом приложения. Большинство из них предназначено для рабочих процессов утверждения.  

Варианты рабочих процессов заполняются посредством заполнения полей в строках рабочего процесса из фиксированных списков значений события и отклика, представляющих сценарии, которые поддерживаются кодом приложения. Дополнительные сведения см. в разделе [Создание рабочих процессов](across-how-to-create-workflows.md).  

Если бизнес-сценарий требует события или отклика рабочего процесса, которые не поддерживаются, партнеру Майкрософт придется реализовать их через код или вы можете настроить рабочий процесс с помощью Power Automate. Дополнительные сведения см. в разделе [Использование [!INCLUDE[prod_short](includes/prod_short.md)] в автоматизированном рабочем процессе](across-how-use-financials-data-source-flow.md) или [События в AL](/dynamics365/business-central/dev-itpro/developer/devenv-events-in-al) в справке разработчика, соответственно.

## <a name="see-also"></a>См. также

[Настройка утверждающих пользователей](across-how-to-set-up-approval-users.md)  
[Настройка уведомлений рабочего процесса](across-setting-up-workflow-notifications.md)  
[Создание рабочих процессов](across-how-to-create-workflows.md)  
[Использование рабочего процесса утверждения](across-how-use-approval-workflows.md)  
[Рабочий процесс](across-workflow.md)  
[Использование Business Central в автоматическом бизнес-процессе](across-how-use-financials-data-source-flow.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]