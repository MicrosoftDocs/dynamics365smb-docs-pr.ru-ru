---
title: Добавить ссылку на страницу или отчет о ролевом центре
description: 'Используя значок закладки, вы можете добавить действие, которое открывает страницу или отчет из навигационного меню вашего ролевого центра.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.search.form: null
ms.date: 07/25/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="bookmark-a-page-or-report-on-your-role-center"></a>Добавьте закладку на страницу или отчет о вашем ролевом центре

Используя значок закладки, вы можете добавить действие, которое открывает страницу или отчет из навигационного меню вашего ролевого центра. Закладки позволяют быстро открывать нужный контент или бизнес-задачи. Вы добавляете закладку с целевой страницы или отчета, то есть с экрана, на который должна открываться ссылка в ролевом центре.

Значок закладки отображается в правом верхнем углу страницы, а также в окне **Что вы хотите сделать**, где можно быстро создать закладки для нескольких страниц или отчетов. Если для страницы уже существует закладка, значит, значок темный, а во всплывающей подсказке написано "Закладка добавлена".

## <a name="bookmark-the-target-page"></a>Добавьте целевую страницу в закладки

1. Откройте любую страницу, на которую вы хотите получить ссылку в своем ролевом центре.
2. Выберите ![Закладка.](media/ui_bookmark_icon.png "Закладка") значок.

Действие, названное в честь страницы, теперь добавлено в меню навигации вашего ролевого центра.

## <a name="bookmark-the-target-report"></a>Добавьте целевой отчет в закладки

1. Откройте любую страницу запроса отчета, ссылку на которую вы хотите получить в своем ролевом центре.
2. Выберите ![Закладка.](media/ui_bookmark_icon.png "Закладка") значок.

Действие, названное в честь отчета, теперь добавлено в меню навигации вашего ролевого центра.

## <a name="bookmark-a-page-or-report-from-the-tell-me-window"></a>Добавьте закладку на страницу или отчет из окна Tell Me

1. Откройте окно **Что вы хотите сделать** и введите, например, **Заказы на продажу**.
2. Наведите курсор на результат поиска страницы или отчета **Заказы на продажу**, а затем выберите значок ![Закладка.](media/ui_bookmark_icon.png "Закладка") значок.

Действие, названное в честь страницы или отчета, теперь добавляется в меню навигации вашего ролевого центра.

## <a name="frequently-asked-questions"></a>Часто задаваемые вопросы

### <a name="can-i-reorganize-my-bookmarks"></a>Могу ли я реорганизовать свои закладки?

Да. Вы можете персонализировать свой ролевой центр и расположить действия в более оптимальной последовательности или переместить их в существующие группы или подгруппы.  
Подробнее: [Персонализация рабочей области](ui-personalization-user.md).

### <a name="how-do-i-remove-a-bookmark"></a>Как удалить закладку?

На целевой странице или в отчете снова выберите значок закладки, чтобы удалить соответствующее действие из ролевого центра. Вы также можете персонализировать свой ролевой центр и временно скрыть действия, не удаляя их полностью.

### <a name="where-do-i-find-my-bookmarks"></a>Где мне найти мои закладки?

При добавлении закладки на страницу или в отчет новое действие добавляется в верхнее навигационное меню на вашем текущем главном экране (ролевой центр). Если у вас много действий, вам может потребоваться нажать кнопку **Еще**, чтобы отобразить все из них, потому что новое действие всегда добавляется в конец списка.
<!-- Should we add a screenshot here? -->

### <a name="i-dont-have-a-bookmark-icon-is-something-wrong"></a>У меня нет значка закладки. Что-то не так?

Возможность добавлять закладки на страницы или отчеты является одной из многих функций персонализации Business Central. Если значок закладки не отображается, вероятно, ваш администратор отключил персонализацию.

### <a name="why-cant-i-bookmark-certain-pages-or-reports"></a>Почему я не могу добавить в закладки определенные страницы или отчеты?

Не все страницы и отчеты могут быть добавлены в закладки. Когда страница или отчет запускаются в каком-то особом контексте, регулируемом бизнес-приложением, значок закладки не отображается. Например, страницы, которые не могут быть найдены в окне **Что вы хотите сделать**, но запускаются иначе, не содержат значка закладки. Аналогично, на страницах запроса отчетов, которые используются только для сбора фильтров без запуска отчета, значок закладки не отображается.

  См. технические подробности о [RunRequestPage](/dynamics365/business-central/dev-itpro/developer/methods-auto/report/reportinstance-runrequestpage-method) и [FilterPageBuilder](/dynamics365/business-central/dev-itpro/developer/methods-auto/filterpagebuilder/filterpagebuilder-data-type).

### <a name="when-clearing-my-personalization-will-my-bookmarks-also-be-cleared"></a>При очистке персонализации будут ли также очищены мои закладки?

Да. Закладки находятся в меню навигации. Если вы удалите изменения в меню навигации на любой странице или удалите все настройки персонализации в ролевом центре, все ваши новые действия будут удалены навсегда.

### <a name="why-does-the-bookmark-icon-continue-to-indicate-its-still-not-bookmarked"></a>Почему значок закладки продолжает указывать на то, что она все еще не добавлена в закладки?

При добавлении закладки новое действие добавляется в меню навигации в ролевом центре, а при последующих посещениях страницы или отчета отображается темный значок закладки. Если вы персонализируете свой ролевой центр и реорганизуете свои действия, переместив их в группы, значок закладки больше не будет темным, и вы сможете добавить еще одну закладку на ту же страницу или отчет. Это позволяет добавить несколько действий на одну страницу или отчет и распределить их по разным группам.

### <a name="why-does-my-link-to-a-report-display-a-different-report"></a>Почему по моей ссылке на отчет отображается другой отчет?

Некоторые отчеты могут быть заменены другими отчетами после применения расширения к Business Central. Когда происходит замена, текст нового действия не обновляется и по-прежнему содержит имя исходного отчета, но ссылка при этом ведет на более новый отчет. Чтобы исправить текст нового действия, вы можете удалить новое действие и добавить его снова.
<!-- For more information on report substitution, see this link UNAVAILABLE AT THIS TIME -->

### <a name="is-bookmarking-available-for-xmlports"></a>Доступны ли закладки для XMLports?

Кол-во В настоящее время добавление действий для открытия XMLports невозможно из пользовательского интерфейса.

### <a name="will-my-bookmarks-be-translated-when-i-change-my-language-in-business-central"></a>Будут ли мои закладки переведены, если я изменю язык в Business Central?

При добавлении нового действия любой переведенный текст, который был доступен в то время, используется в закладке. Если новый переведенный текст будет добавлен позже, то новое действие не будет включать более новые переводы.

### <a name="why-cant-i-add-text-in-a-page-right-after-opening-it-with-the-bookmark"></a>Почему я не могу добавить текст на страницу сразу после ее открытия с помощью закладки?

Когда страница добавлена в закладки, она всегда будет открываться в режиме просмотра из закладки &mdash; даже если она была в режиме редактирования, когда была добавлен в закладки. Выбор значка **Внести изменения в страницу** ![Показывает значок карандаша для редактирования страницы.](media/edit-pencil.png) позволит вам добавлять текст в редактируемые поля.

## <a name="see-also"></a>См. также

[Персонализация вашей рабочей области](ui-personalization-user.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Изменение базовых параметров](ui-change-basic-settings.md)  
[Изменение набора отображаемых функций](ui-experiences.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
