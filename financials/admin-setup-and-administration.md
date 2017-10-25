---
title: "Административные задачи в Dynamics 365 | Документы Майкрософт"
description: "Некоторые задачи в [!INCLUDE[d365fin](includes/d365fin_md.md)] требуют централизованного администрирования и настройки. Познакомьтесь с этими задачами и узнайте, что делать."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 09c3460a50088098bfe5c2fb633e76dccbac0794
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="setup-and-administration-in-dynamics-365-for-financials"></a>Настройка и администрирование в Dynamics 365 for Financials
Основные задачи администрирования обычно выполняются в организации исполнителем какой-либо одной роли. Объем этих задач может зависеть от размера организации и должностных обязанностей администратора. Среди подобных задач могут быть следующие: управление синхронизацией с базой данных работ и очередей электронной почты, задание пользователей, настройка пользовательского интерфейса и управление ключами шифрования.  

Ввод правильных значений настройки с самого начала важен для успешной работы любого нового программного обеспечения для бизнеса. [!INCLUDE[d365fin](includes/d365fin_md.md)] включает ряд руководство по настройке, помогающих настроить ключевые данные. Для получения более подробной информации см. [Настройка Dynamics 365 for Financials](setup.md).

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

Администратор или привилегированный пользователь может настроить платформу обмена данными, чтобы разрешить пользователям экспорт и импорт данные в банковских файлах и файлах зарплаты, например, для различных процессов управления денежными средствами.  

В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.   

|**Задача**|**Ссылка**|  
|------------|-------------|  
|Добавьте пользователей, управляйте разрешениями и доступом к данным, назначьте роли.|[Пользователи, профили и ролевые центры в Dynamics 365 for Financials](admin-users-profiles-roles.md)|  
|Отслеживание всех непосредственных изменений, вносимых пользователями в данные базы данных, для определения источника ошибок и изменений в данных.|[Регистрация изменений в Dynamics 365 for Financials](across-log-changes.md)|  
|Поддержка ваших решений по настройке за счет рекомендаций для выбранных полей, которые могут стать причиной неэффективной работы решения в случае неправильной настройки.|[Настройка сложных областей приложения с помощью рекомендаций](set-up-complex-application-areas-using-best-practices.md)|  
|Можно отображать страницы, модули codeunit и запросы как веб-службы.|[Практическое руководство. Публикация веб-службы](across-how-publish-web-service.md)|  
|Настройте SMTP-сервер для включения передачи сообщений электронной почты в Dynamics 365 for Financials и из него.| [Практическое руководство. Настройка электронной почты вручную или с помощью сопровождаемой настройки](madeira-how-setup-email.md)|  
|Ввод одиночных или повторяющихся запросов для создания отчетов или запуска модулей Codeunit.|[Использование очередей работ для планирования задач](admin-job-queues-schedule-tasks.md)|  
|Управление документами, удаление или сжатие документов|[Управление документами](admin-manage-documents.md)|  
|Настройка нового филиала с помощью шаблонов|[Создание новых организаций в [!INCLUDE[d365fin](includes/d365fin_md.md)]](about-new-company.md)|  

## <a name="see-also"></a>См. также
[Обзор бизнес-функций](madeira-business-functionality.md)  
[Общие бизнес-функции](ui-across-business-areas.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
[Добро пожаловать в [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)  

