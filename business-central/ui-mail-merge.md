---
title: Использование шаблонов Word для массовых сообщений | Документация Майкрософт
description: Шаблоны Word могут упростить массовое создание документов, персонализированных для определенных сущностей.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: document, mail, merge, Word, template, email
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: d29e29eca7dfc24ded51aed994ac7003fb4d30ab
ms.sourcegitcommit: 6bce51954f17b80491e180f25d67ff18b1618a88
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "6110958"
---
# <a name="using-word-templates-for-bulk-communication"></a>Использование шаблонов Word для массовых сообщений
Шаблоны Microsoft Word могут упростить массовые сообщения с такими сущностями, как клиенты и поставщики. Например, вы можете создавать буклеты для оповещения клиентов о кампании распродаж, письма для информирования поставщиков о новой политике закупок или приглашения для привлечения контактов на предстоящее мероприятие.

> [!NOTE]
> Вы можете использовать шаблоны Word только на устройствах с Microsoft Word 2019 и операционной системой Windows.

Вы можете использовать сущности в [!INCLUDE[prod_short](includes/prod_short.md)] в качестве источника данных для шаблона и добавить поля слияния, чтобы персонализировать документы для каждой сущности. Поля слияния берутся из сущности в [!INCLUDE[prod_short](includes/prod_short.md)]. Когда вы применяете шаблон Word к сущности, данные из полей слияния вставляются в документ.

На странице **Шаблоны Word** вы можете использовать мастер настройки, чтобы загрузить ZIP-файл, содержащий DataSource.txt и файл шаблона Word для сущности. После настройки шаблона и добавления полей слияния вы используете тот же мастер для отправки шаблона. Вы можете использовать только шаблоны Word и файлы источников данных, которые вы загружаете из [!INCLUDE[prod_short](includes/prod_short.md)], и вы должны хранить файлы в том же месте.

> [!NOTE]
> Когда вы выбираете сущность, для которой нужно создать шаблон, в списке отображаются все сущности в [!INCLUDE[prod_short](includes/prod_short.md)]. Однако вы не можете создавать шаблоны для всех сущностей. Если имя сущности содержит специальные символы, такие как **/**, **.**, **_** или **-**, вы не можете создать шаблон для нее. Имя сущности отображается в столбце **Метка объекта**.

Когда вы настраиваете шаблон в Word, на вкладке **Рассылки** вы можете добавить поля слияния, выбрав **Вставить поле слияния**.

> [!NOTE]
> Вы не можете использовать поля слияния, если имя поля содержит 40 или более символов. Например, вы не можете использовать поле "Company__Information_Customs_Permit_Date", потому что оно состоит из 40 символов. 

Когда ваш шаблон Word будет готов, на странице **Шаблоны Word** вы можете выбрать **Применить** для создания документов. Вы можете создать один документ, содержащий разделы для каждой сущности, или разделить операцию, чтобы создать новый документ для каждой сущности.

## <a name="to-create-a-word-template"></a>Чтобы создать шаблон Word
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Шаблоны Word**, затем выберите соответствующую ссылку.
2. Выполните шаги в мастере настройки. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="see-also"></a>См. также
[Управление макетами отчетов и документов](ui-manage-report-layouts.md)  
