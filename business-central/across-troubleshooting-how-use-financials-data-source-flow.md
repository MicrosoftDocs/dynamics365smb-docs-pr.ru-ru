---
title: Устранение неполадок при интеграции с Microsoft Flow | Документы Майкрософт
description: Устраняйте неполадки, чтобы сделать данные Business Central доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания автоматического бизнес-процесса.
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 04/01/2019
ms.author: solsen
ms.openlocfilehash: 8a43df89261867f80ba16782cde92b040ce180c8
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2019
ms.locfileid: "925928"
---
# <a name="troubleshooting-integration-with-microsoft-flow---request-url-too-long"></a>Устранение неполадок при интеграции с Microsoft Flow — запрошенный URL-адрес слишком длинный
Можно использовать данные [!INCLUDE[d365fin](includes/d365fin_md.md)] как часть рабочего процесса в Microsoft Flow.  

> [!NOTE]  
>   Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Flow.  

При создании Microsoft Flow с помощью соединителя [!INCLUDE[d365fin](includes/d365fin_md.md)] вы можете получить сообщение об ошибке, указывающее, что запрошенный URL-адрес слишком длинный после создания потока, например: **RequestUriTooLong**.

## <a name="cause"></a>Причина
Для активации потока выполняется поиск изменений в данных. Если определяется, что данные были изменены, соединители сравнивают кэшированные данные с новыми данными, запрошенными из источника.  

Если запрос данных создается слишком длинный URL-адрес, возникнет ошибка. К распространенным причинам могут относиться следующие:
- Обычно любая исходная таблица с более 250 строками.
- Исходные таблицы, содержащие несколько тысяч записей.

## <a name="workaround"></a>Обходное решение
Выполните следующие шаги в качестве обходного решения.
1. Выберите изменение потока с ошибкой.
2. Разверните **Показать дополнительные параметры** в триггере потока.
3. В поле **Пропустить подсчет** введите количество записей для пропуска.  
Например, если для таблица, используемая как источник данных, имеет 4000 записей, введите 4000 как число записей для пропуска.
4. Обновите поток.

> [!NOTE]  
> Соединитель в данный момент находится в бета-версии. Обновления, связанные с изменением данных, будут добавлены в будущих выпусках.


## <a name="see-also"></a>См. также
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в автоматическом бизнес-процессе](across-how-use-financials-data-source-flow.md)  
[Приступая к работе](product-get-started.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Управление пользователями и разрешениями](ui-how-users-permissions.md)    
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Финансы](finance.md)  
