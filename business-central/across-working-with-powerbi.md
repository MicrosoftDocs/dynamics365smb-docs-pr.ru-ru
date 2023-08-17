---
title: Работа с отчетами Power BI в Business Central | Документация Майкрософт
description: 'Получение аналитических сведений, бизнес-аналитики и ключевых показателей эффективности из данных Business Central с помощью Power BI.'
author: jswymer
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'account schedule, analysis, reporting, financial report, business intelligence, KPI'
ms.date: 04/01/2021
ms.author: jswymer
---
# <a name="work-with-power-bi-reports-in-"></a>Работа с отчетами Power BI в [!INCLUDE [prod_short](includes/prod_short.md)]

В этой статье вы узнаете некоторые основные сведения о просмотре ответов Power BI в [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="overview"></a>Обзор

Отчеты Power BI дают вам представление о вашем [!INCLUDE[prod_short](includes/prod_short.md)]. Различные страницы в [!INCLUDE [prod_short](includes/prod_short.md)] включают часть отчетов Power BI, которая может отображать отчеты Power BI. Ролевой центр — это типичная страница, на которой вы увидите часть отчетов Power BI. Некоторые страницы со списками, например **Элементы**, также включают часть Power BI.

[!INCLUDE [prod_short](includes/prod_short.md)] работает вместе со службой Power BI. Отчеты для отображения в [!INCLUDE [prod_short](includes/prod_short.md)] хранятся в службе Power BI. В [!INCLUDE [prod_short](includes/prod_short.md)] вы можете переключить отчет, отображаемый в части Power BI, на любой отчет Power BI, который доступен в вашей службе Power BI. При первом входе в [!INCLUDE [prod_short](includes/prod_short.md)] и пока вы не подключитесь к службе Power BI части будут пустыми, как показано здесь:

![Часть Power BI в Business Central.](./media/power-bi-part.png)

## <a name="get-started"></a>Начало работы

### <a name="prerequisites"></a>Предварительные требования

Если вы используете [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises, он должен быть включен для интеграции Power BI. Эту задачу обычно выполняет администратор. Дополнительные сведения см. в разделе [Настройка [!INCLUDE[prod_short](includes/prod_short.md)] On-Premises для интеграции Power BI](admin-powerbi-setup.md#setup).

> [!NOTE]
> [!INCLUDE[prod_short](includes/prod_short.md)] Online уже настроен для интеграции с Power BI.

### <a name="sign-up-power-bi"></a>Регистрация на Power BI

Прежде чем вы сможете использовать Power BI с помощью [!INCLUDE[prod_short](includes/prod_short.md)], вам нужно зарегистрироваться в службе Power BI. Если вы еще не зарегистрировались, перейдите на [https://powerbi.microsoft.com](https://powerbi.microsoft.com). При регистрации используйте рабочий адрес электронной почты и пароль.

## <a name="connect-to-power-bi---one-time-only"></a><a name="connect"></a>Подключение к Power BI — только один раз

При первом входе в [!INCLUDE [prod_short](includes/prod_short.md)] вы, вероятно, увидите пустую часть Power BI (как показано на предыдущем рисунке) на различных страницах. Первое, что нужно сделать, это подключиться к вашей учетной записи Power BI. После подключения вы можете просматривать отчеты. Вам нужно выполнить этот шаг только один раз.

1. Выберите **Начало работы с Power BI** в части **Отчеты Power BI**.
2. Запускается мастер настройки **Настройка отчетов Power BI в Business Central**. Выберите **Далее**, чтобы продолжить.
3. На странице **Проверьте свою лицензию Power BI**. Выполните один из следующих шагов:

    - Если вы еще не зарегистрировались на Power BI, выберите [Перейти на домашнюю страницу Power BI](https://powerbi.microsoft.com). Зарегистрируйте учетную запись, затем вернитесь в [!INCLUDE[prod_short](includes/prod_short.md)] и закончите настройку.

    - Если у вас уже есть лицензия, выберите **Далее**.
4. На следующей странице [!INCLUDE[prod_short](includes/prod_short.md)] теперь загрузит демонстрационный отчет в Power BI. Этот шаг займет несколько минут, поэтому выполняется в фоновом режиме. Чтобы завершить настройку, выберите **Далее**, затем **Готово**.

Начнется процесс подключения. В процессе [!INCLUDE [prod_short](includes/prod_short.md)] обменивается данными со службой Power BI, чтобы определить, есть ли у вас действующие учетная запись и лицензия Power BI. Как только ваша лицензия будет подтверждена, отчет Power BI по умолчанию отображаются на странице. Если там отчет не отображается, вы можете выбрать отчет из части.

> [!TIP]
> С [!INCLUDE [prod_short](includes/prod_short.md)] Online этот шаг автоматически отправит отчеты Power BI по умолчанию, используемые в [!INCLUDE [prod_short](includes/prod_short.md)], в вашу рабочую область Power BI.

#### <a name="from--on-premises"></a>Из [!INCLUDE [prod_short](includes/prod_short.md)] On-premises

Присоединение к Power BI из [!INCLUDE [prod_short](includes/prod_short.md)] похоже на случай Online. Однако вам может быть предложено на странице **РАЗРЕШЕНИЯ СЛУЖБЫ AZURE ACTIVE DIRECTORY** предоставить доступ к службам Power BI. Чтобы предоставить доступ, выберите **Авторизовать службы Azure**, затем **Принять**.

После подключения вы можете выбрать отчет из части Power BI на страницах.

## <a name="work-with-power-bi-reports"></a>Работа с отчетами Power BI

### <a name="show-reports-on-list-pages"></a>Отображение отчетов на страницах списков

[!INCLUDE[prod_long](includes/prod_long.md)] включает информационную панель Power BI на нескольких ключевых страницах списка. Эта информационная панель предоставляет дополнительные сведения о данных в списке. При перемещении между строками в списке отчет обновляется и фильтруется в соответствии с выбранной операцией.

Чтобы узнать, как создавать отчеты для страниц списков, см. раздел [Создание отчетов Power BI для отображения данных списка в [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-powerbi-reports-factbox.md).

> [!TIP]
> Если вы не видите информационную панель Power BI, она может быть скрыта в вашей рабочей области персонализацией. Выберите значок ![Параметры](media/ui-experience/settings_icon_small.png "Значок настроек для ролевого центра"), а затем выберите действие **Персонализация**. Дополнительные сведения см. в разделе [Персонализация рабочей области](ui-personalization-user.md).
>
> Или, если у вас более старая версия Business Central, перейдите на панель действий, выберите **Действия** > **Отображение** > **Показать/скрыть отчеты Power BI**.

### <a name="switch-reports"></a>Переключение отчетов

Часть Power BI на странице может отображать любой отчет Power BI, который вам доступен. Чтобы переключиться на просмотр другого отчета, выберите действие **Выбрать отчет** из раскрывающегося списка команд вверху части.  

Страница **Выбор отчетов Power BI** показывает список всех отчетов Power BI, к которым у вас есть доступ. Этот список извлекается из любого из ваших собственных рабочих пространств или рабочих пространств, к которым вам предоставлен доступ в службе Power BI. Выберите поле **Включить** для каждого отчета, который вы хотите отобразить на домашней странице, затем нажмите **ОК**. Вы вернетесь на страницу, и появится последний включенный отчет. Используя раскрывающийся список команд, используйте команды **Назад** и **Далее** для перехода между отчетами.  

### <a name="get-more-reports"></a>Получить больше отчетов

Если вы не видите никаких отчетов на странице **Выбор отчетов Power BI** или не видите нужный отчет, выберите **Получить отчеты**. Это действие позволяет искать отчеты в двух местах: *Моя организация* или *Службы*.

- Выберите **Моя Организация**, чтобы перейти к службам Power BI. Отсюда вы можете просматривать отчеты в вашей организации, на просмотр которых вам было предоставлено право. Затем вы можете добавить их в свою рабочую область.
- Выберите **Службы**, чтобы перейти в Microsoft AppSource, где вы можете установить приложения Power BI.  

> [!TIP]
> При наличии Power BI Desktop вы также можете создавать новые отчеты Power BI. Затем, как только эти отчеты будут опубликованы в вашей рабочей области Power BI, они появятся на странице **Выбор отчетов Power BI**.  

### <a name="manage-and-modify-reports"></a>Управление отчетами и их изменение

Вы можете внести изменения в отчет в части Power BI. Внесенные вами изменения будут опубликованы в службе Power BI. Если отчет доступен другим пользователям, они также увидят изменения, если вы не сохраните изменения в новом отчете.

Чтобы изменить отчет, выберите действие **Управление отчетом** из раскрывающегося списка команд в части Power BI. Затем начинайте вносить изменения. Когда вы закончите вносить изменения, выберите **Файл** > **Сохранить**. Если это общий отчет и вы не хотите вносить изменения для всех пользователей, выберите **Сохранить как**, чтобы избежать внесения этого изменения для всех пользователей.

После возвращения в ролевой центр появится обновленный отчет. Если вы использовали вариант **Сохранить как**, нужно будет выбрать **Выбрать отчет**, затем включить новый отчет, чтобы его увидеть.

> [!NOTE]
> Эта возможность недоступна с [!INCLUDE [prod_short](includes/prod_short.md)] On-Premises.

### <a name="upload-reports"></a><a name="upload"></a>Отправка отчетов

Отчеты Power BI можно распространять среди пользователей в виде файлов .pbix. Если у вас есть файлы .pbix, вы можете загрузить их и поделиться ими со всеми пользователями [!INCLUDE [prod_short](includes/prod_short.md)]. Отчеты становятся общими внутри каждой организации в [!INCLUDE [prod_short](includes/prod_short.md)].  

Чтобы отправить отчет, выберите действие **Отправить отчет** из раскрывающегося списка команд в части **Отчеты Power BI**. Затем найдите файл .pbix, который определяет отчеты, которыми вы хотите поделиться. Можно изменить имя по умолчанию для файла.  

После отправки отчета в вашу рабочую область Power BI он автоматически отправляется в рабочие области Power BI других пользователей.

> [!NOTE]
> Для отправки отчета необходимы разрешения пользователя СУПЕР в [!INCLUDE[prod_short](includes/prod_short.md)]. Кроме того, вы не можете отправлять отчеты с помощью [!INCLUDE [prod_short](includes/prod_short.md)] On-Premises. В локальной версии On-Premises вы загружаете отчеты прямо в вашу рабочую область Power BI. Дополнительные сведения см. в разделе [Работа с данными [!INCLUDE [prod_short](includes/prod_short.md)] в Power BI](across-working-with-business-central-in-powerbi.md).

## <a name="fixing-problems"></a>Устранение проблем

Однако если что-то работает некорректно, в этом разделе предложено обходное решение для типичных проблем.  

### <a name="you-dont-have-a-power-bi-account"></a>У вас нет учетной записи Power BI

Учетная запись Power BI не была настроена. Чтобы получить действительную учетную запись Power BI, у вас должна быть лицензия, и вы должны были предварительно войти в Power BI, чтобы создать рабочую область Power BI.

### <a name="message-there-are-no-enabled-reports-choose-select-report-to-see-a-list-of-reports-that-you-can-display"></a>Сообщение: "Включенные отчеты отсутствуют. Нажмите кнопку "Выбрать отчет", чтобы увидеть список отчетов, которые можно открыть.

Это сообщение появляется, если отчет по умолчанию не удалось развернуть на вашей рабочей области Power BI. Или он развернут, но не был успешно обновлен. Перейдите к отчету в своей рабочей области Power BI, выберите **Набор данных**, **Настройки**, затем вручную обновите учетные данные. После успешного обновления набора данных вернитесь в [!INCLUDE[prod_short](includes/prod_short.md)] и вручную выберите отчет на странице **Выбрать отчеты**.

#### <a name="you-cant-see-a-report-on-the-select-report-page-on-a-list-page"></a>Вы не можете увидеть отчет на странице "Выбор отчета" на странице списка

Вероятно, это потому, что в названии отчета нет названия страницы списка. Очистите фильтр, чтобы получить полный список доступных отчетов Power BI.

## <a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Business Central и Power BI](admin-powerbi.md)  
[Создание отчетов Power BI для отображения данных [!INCLUDE [prod_long](includes/prod_long.md)]](across-how-use-financials-data-source-powerbi.md)  
[Обзор компонентов и архитектуры интеграции Power BI для [!INCLUDE[prod_short](includes/prod_short.md)]](admin-powerbi-overview.md)  
[Работа с данными [!INCLUDE [prod_short](includes/prod_short.md)] в Power BI](across-working-with-business-central-in-powerbi.md)  
[Power BI для потребителей](/power-bi/consumer/end-user-consumer)  
["Новый внешний вид" службы Power BI](/power-bi/service-new-look)  
[Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Документация Power BI](/power-bi/)  
[Бизнес-аналитика](bi.md)  
[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] как источника данных Power Apps](across-how-use-financials-data-source-powerapps.md)  
[Использование [!INCLUDE[prod_short](includes/prod_short.md)] в Power Automate](across-how-use-financials-data-source-flow.md)  




[!INCLUDE[footer-include](includes/footer-banner.md)]
