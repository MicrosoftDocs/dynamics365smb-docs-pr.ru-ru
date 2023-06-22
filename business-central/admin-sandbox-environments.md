---
title: Среды-песочницы
description: 'Узнайте о том, как специализированная среда может помочь вам безопасно исследовать, изучать, демонстрировать, разрабатывать, устранять неполадки и тестировать Business Central.'
author: SusanneWindfeldPedersen
ms.topic: conceptual
ms.reviewer: edupont
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'sandbox, demo, develop'
ms.date: 12/20/2021
ms.author: solsen
---
# <a name="sandbox-environments-in-includeprodshortincludesprodshortmd" />Среды-песочницы в [!INCLUDE[prod_short](includes/prod_short.md)]

В [!INCLUDE[prod_short](includes/prod_short.md)] Online вы можете легко получить безопасную среду, в которой тестировать, обучать или устранять неполадки, не нарушая рабочие процессы вашей компании или бизнес-данные. Такая непроизводственная среда называется *песочницей*. В среде песочницы, изолированной от производственной среды, можно безопасно исследовать, обучать, демонстрировать, разрабатывать и тестировать сервисы без риска повлиять на данные или настройки производственной среды.  

> [!TIP]
> Вы открыли эту статью после того, как выбрали название своей среды [!INCLUDE [prod_short](includes/prod_short.md)] в верхней панели? В настоящее время вы не можете изменить имя или среду таким образом. Вместо этого вы должны попросить своего администратора изменить имя или попросить его поделиться ссылкой на другую среду.

Ваш администратор управляет средами-песочницами в [центре администрирования](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments?toc=/dynamics365/business-central/toc.json).  

Например, если вы хотите создать "песочницу" для сравнительного тестирования, ваш администратор может создать выделенную среду в центре администрирования. Дополнительные сведения см. в разделе [Рабочая среда и среда песочницы](/dynamics365/business-central/dev-itpro/administration/environment-types) в документации для разработчиков и администраторов.  

Вы также можете безопасно использовать песочницы для обучения, например, для прохождения пути обучения с сайта [Обучение Microsoft](/training/dynamics365/business-central?WT.mc_id=dyn365bc_landingpage-docs), потому что это безопасная среда для экспериментов. Если что-то пойдет не так, вы просто удалите песочницу и начнете заново.  

Когда вы закончите, вы можете удалить песочницу с помощью центра администрирования.  

> [!NOTE]
> Технически среды-песочницы сильно отличаются от рабочих сред. Ваш администратор может создать песочницу, которая включает производственные данные, но это по-прежнему песочница, и вы не можете, например, запросить экспорт базы данных. Дополнительные сведения см. в разделе [Среды-песочницы](/dynamics365/business-central/dev-itpro/administration/environment-types#sandbox-environments) в документации для разработчиков и администраторов.

Среда "песочницы" не менее полезна, потому что она включает в себя несколько удобных функций:

* [Повышенное удобство работы пользователей](#advanced-user-experience)  
<!--* [Complete sample data](#complete-sample-data)  -->
* [Конструктор](#designer)  

## <a name="advanced-user-experience" />Повышенное удобство работы пользователей

Можно включить и попробовать полные функциональные возможности стандартной версии [!INCLUDE[prod_short](includes/prod_short.md)] в среде арендатора песочницы, задав поле **Опыт** на странице **Информация о компании** на *Premium*. Найдите страницу **Информация о компании** в :::image type="content" source="media/ui-experience/settings_icon_small.png" alt-text="Значок настроек."::: меню.  

После того как вы включили вариант настройки *Premium*, вы получаете доступ ко всем стандартным профилям (ролям) и ролевым центрам стандартной версии. Кроме того, вы можете связаться с партнером по перепродаже для демонстрации возможностей. Для получения дополнительной информации прочитайте раздел [Как найти партнера по перепродаже?](across-faq.yml#how-do-i-find-a-reselling-partner).  

### <a name="complete-sample-data" />Полные демонстрационные данные

В ситуациях, когда вам нужны дополнительные примеры данных, обратитесь к своему партнеру по перепродаже.
<!-- In the sandbox environment, you can also create a new company with the **Advanced Evaluation - Complete Sample Data** option so that you can take training or step through walkthroughs that require additional sample data, such as [Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations](walkthrough-receiving-and-putting-away-in-basic-warehousing.md).   -->

<!--#### To create a company with complete sample data in a sandbox

1. Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Companies**, and then choose the related link.  
2. Choose the **New** action, and then choose **Create New Company**.  
3. In the **Assisted Setup for Creating a Company** page, choose **Next**.  
4. Specify a name for the new company, and then, in the **Select the data and setup to get started** field, choose **Advanced Evaluation - Complete Sample Data**.  
5. Complete the rest of the assisted setup guide.  

When the assisted setup guide completes, you can start exploring the new company with the complete sample data. For more information, see [Creating New Companies in [!INCLUDE[prod_short](includes/prod_short.md)]](about-new-company.md).  -->

## <a name="designer" />Конструктор

В среде "песочницы" включен **Конструктор**. Вы можете активировать конструктора, выбрав значок дизайна ![Конструктор.](./media/across-sandbox/sandbox-inclient-design-icon.png) на странице или выбрав пункт меню **Дизайн** в ![Параметры](media/ui-experience/settings_icon_small.png) Меню параметров.  

Для получения дополнительной информации см. [Использование конструктора](/dynamics365/business-central/dev-itpro/developer/devenv-inclient-designer) в документации разработчика и администратора (только на английском языке).  

<!-- ![In-client Designer.](./media/across-sandbox/sandbox-inclient-designer.png) -->

## <a name="see-related-microsoft-trainingtrainingmodulesadmin-online-dynamics--business-central" />См. соответствующее [обучение Microsoft](/training/modules/admin-online-dynamics-365-business-central/)

## <a name="see-also" />См. также

[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Пробные версии и подписки [!INCLUDE[prod_long](includes/prod_long.md)]](/dynamics365/business-central/dev-itpro/administration/trials-subscriptions)  
[Управление средами в центре администрирования Business Central](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments)  
[Рабочая среда и среда песочницы](/dynamics365/business-central/dev-itpro/administration/environment-types)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
