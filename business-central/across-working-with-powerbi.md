---
title: Работа с отчетами Power BI в Business Central | Документация Майкрософт
description: Анализ данных, бизнес-аналитика и КПЭ на основе данных Business Central становятся проще благодаря приложениям Business Central для Power BI.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 10/01/2020
ms.author: jswymer
ms.openlocfilehash: 28e332137346aae320b73c326bb3a41d3b7e7097
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3927201"
---
# <a name="working-with-power-bi-reports-in-prodshort"></a>Работа с отчетами Power BI в [!INCLUDE [prodshort](includes/prodshort.md)]

В этой статье вы узнаете некоторые основные сведения о просмотре ответов Power BI в [!INCLUDE [prodshort](includes/prodshort.md)].

## <a name="overview"></a>Обзор

Отчеты Power BI дают вам представление о вашем [!INCLUDE[prodshort](includes/prodshort.md)]. Различные страницы в [!INCLUDE [prodshort](includes/prodshort.md)] включают часть отчетов Power BI, которая может отображать отчеты Power BI. Ролевой центр — это типичная страница, на которой вы увидите часть отчетов Power BI. Некоторые страницы со списками, например **Элементы**, также включают часть Power BI.

[!INCLUDE [prodshort](includes/prodshort.md)] работает вместе со службой Power BI. Отчеты для отображения в [!INCLUDE [prodshort](includes/prodshort.md)] хранятся в службе Power BI. В [!INCLUDE [prodshort](includes/prodshort.md)] вы можете переключить отчет, отображаемый в части Power BI, на любой отчет Power BI, который доступен в вашей службе Power BI. При первом входе в [!INCLUDE [prodshort](includes/prodshort.md)] и пока вы не подключитесь к службе Power BI части будут пустыми, как показано здесь:

![Часть Power BI в Business Central](./media/power-bi-part.png)

## <a name="prerequisites"></a>Предварительные требования

Если вы используете [!INCLUDE[prodshort](includes/prodshort.md)] On-Premises, он должен быть включен для интеграции Power BI. Эту задачу обычно выполняет администратор. Дополнительные сведения см. в разделе [Настройка [!INCLUDE[prodshort](includes/prodshort.md)] On-Premises для интеграции Power BI](admin-powerbi-setup.md#setup).

> [!NOTE]
> [!INCLUDE[prodshort](includes/prodshort.md)] Online уже настроен для интеграции с Power BI.

## <a name="get-ready"></a>Подготовка

Подпишитесь на службу Power BI. Если вы еще не зарегистрировались, перейдите на [https://powerbi.microsoft.com](https://powerbi.microsoft.com). При регистрации используйте рабочий адрес электронной почты и пароль.

## <a name="connect-to-power-bi---one-time-only"></a>Подключение к Power BI — только один раз

При первом входе в [!INCLUDE [prodshort](includes/prodshort.md)] вы можете увидеть пустую часть Power BI на некоторой странице, как показано на предыдущем рисунке. Первое, что нужно сделать, это подключиться к вашей учетной записи Power BI. После подключения вы можете просматривать отчеты. Вам нужно выполнить этот шаг только один раз.

Чтобы подключиться к Power BI, выберите ссылку **Начало работы с Power BI** в части **Отчеты Power BI**.

В процессе подключения [!INCLUDE [prodshort](includes/prodshort.md)] обменивается данными со службой Power BI, чтобы определить, есть ли у вас действующие учетная запись и лицензия Power BI. Как только ваша лицензия будет подтверждена, отчет Power BI по умолчанию отображаются на странице. Если там отчет не отображается, вы можете выбрать отчет из части.

> [!TIP]
> С [!INCLUDE [prodshort](includes/prodshort.md)] Online этот шаг автоматически отправит отчеты Power BI по умолчанию, используемые в [!INCLUDE [prodshort](includes/prodshort.md)], в вашу рабочую область Power BI.

##### <a name="from-prodshort-on-premises"></a>Из [!INCLUDE [prodshort](includes/prodshort.md)] On-premises

Присоединение к Power BI из [!INCLUDE [prodshort](includes/prodshort.md)] похоже на случай Online. Однако вам будет предложено на странице **РАЗРЕШЕНИЯ СЛУЖБЫ AZURE ACTIVE DIRECTORY** предоставить доступ к службам Power BI. Чтобы предоставить доступ, выберите **Авторизовать службы Azure**, затем **Принять**.

После подключения вы можете выбрать отчет из части Power BI на страницах.

## <a name="show-power-bi-reports-on-list-pages"></a>Отображение отчетов Power BI на страницах списков

[!INCLUDE[prodlong](includes/prodlong.md)] включает информационную панель Power BI на нескольких ключевых страницах списка. Эта информационная панель предоставляет дополнительные сведения о данных в списке. При перемещении между строками в списке отчет обновляется и фильтруется в соответствии с выбранной операцией. Если вы не видите эту часть, то на панели действий выберите **Действия** > **Показать** > **Показать/скрыть отчеты Power BI**. Для получения дополнительной информации см. раздел [Создание отчетов Power BI для отображения данных списка в [!INCLUDE[prodshort](includes/prodshort.md)]](across-how-use-powerbi-reports-factbox.md).

## <a name="select-power-bi-reports"></a>Выбор отчетов Power BI

Часть Power BI на странице может отображать любой отчет Power BI, который вам доступен. Чтобы переключиться на просмотр другого отчета, выберите действие **Выбрать отчет** из раскрывающегося списка команд вверху части.  

Страница **Выбор отчетов Power BI** показывает список всех отчетов Power BI, к которым у вас есть доступ. Этот список получается из вашей рабочей области Power BI. Выберите поле **Включить** для каждого отчета, который вы хотите отобразить на домашней странице, затем нажмите **ОК**. Вы вернетесь на страницу, и появится последний включенный отчет. Используя раскрывающийся список команд, используйте команды **Назад** и **Далее** для перехода между отчетами.  

## <a name="get-reports"></a>Получение отчетов

Если вы не видите никаких отчетов на странице **Выбор отчетов Power BI** или не видите нужный отчет, выберите **Получить отчеты**. Это действие позволяет искать отчеты в двух местах: *Моя организация* или *Службы*.

- Выберите **Моя Организация**, чтобы перейти к службам Power BI. Отсюда вы можете просматривать отчеты в вашей организации, на просмотр которых вам было предоставлено право. Затем вы можете добавить их в свою рабочую область.
- Выберите **Службы**, чтобы перейти в Microsoft AppSource, где вы можете установить приложения Power BI.  

> [!TIP]
> При наличии Power BI Desktop вы также можете создавать новые отчеты Power BI. Затем, как только эти отчеты будут опубликованы в вашей рабочей области Power BI, они появятся на странице **Выбор отчетов Power BI**.  

## <a name="manage-and-modify-reports"></a>Управление отчетами и их изменение

Вы можете внести изменения в отчет в части Power BI. Внесенные вами изменения будут опубликованы в службе Power BI. Если отчет доступен другим пользователям, они также увидят изменения, если вы не сохраните изменения в новом отчете.

Чтобы изменить отчет, выберите действие **Управление отчетом** из раскрывающегося списка команд в части Power BI. Затем начинайте вносить изменения. Когда вы закончите вносить изменения, выберите **Файл** > **Сохранить**. Если это общий отчет и вы не хотите вносить изменения для всех пользователей, выберите **Сохранить как**, чтобы избежать внесения этого изменения для всех пользователей.

После возвращения в ролевой центр появится обновленный отчет. Если вы использовали вариант **Сохранить как**, нужно будет выбрать **Выбрать отчет**, затем включить новый отчет, чтобы его увидеть.

> [!NOTE]
> Эта возможность недоступна с [!INCLUDE [prodshort](includes/prodshort.md)] On-Premises.

## <a name="upload-reports"></a><a name="upload"></a>Отправка отчетов

Отчеты Power BI можно распространять среди пользователей в виде файлов .pbix. Если у вас есть файлы .pbix, вы можете загрузить их и поделиться ими со всеми пользователями [!INCLUDE [prodshort](includes/prodshort.md)]. Отчеты становятся общими внутри каждой организации в [!INCLUDE [prodshort](includes/prodshort.md)].  

Чтобы отправить отчет, выберите действие **Отправить отчет** из раскрывающегося списка команд в части **Отчеты Power BI**. Затем найдите файл .pbix, который определяет отчеты, которыми вы хотите поделиться. Можно изменить имя по умолчанию для файла.  

После отправки отчета в вашу рабочую область Power BI он автоматически отправляется в рабочие области Power BI других пользователей.

> [!NOTE]
> Для отправки отчета необходимы разрешения пользователя СУПЕР в [!INCLUDE[prodshort](includes/prodshort.md)]. Кроме того, вы не можете отправлять отчеты с помощью [!INCLUDE [prodshort](includes/prodshort.md)] On-Premises. В локальной версии On-Premises вы загружаете отчеты прямо в вашу рабочую область Power BI. Дополнительные сведения см. в разделе [Работа с данными [!INCLUDE [prodshort](includes/prodshort.md)] в Power BI](across-working-with-business-central-in-powerbi.md).

## <a name="fixing-problems"></a>Устранение проблем

Однако если что-то работает некорректно, в этом разделе предложено обходное решение для типичных проблем.  

### <a name="you-dont-have-a-power-bi-account"></a>У вас нет учетной записи Power BI

Учетная запись Power BI не была настроена. Чтобы получить действительную учетную запись Power BI, у вас должна быть лицензия, и вы должны были предварительно войти в Power BI, чтобы создать рабочую область Power BI.   

### <a name="message-there-are-no-enabled-reports-choose-select-report-to-see-a-list-of-reports-that-you-can-display"></a>Сообщение: "Включенные отчеты отсутствуют. Нажмите кнопку "Выбрать отчет", чтобы увидеть список отчетов, которые можно открыть.

Это сообщение появляется, если отчет по умолчанию не удалось развернуть на вашей рабочей области Power BI. Или он развернут, но не был успешно обновлен. Перейдите к отчету в своей рабочей области Power BI, выберите **Набор данных**, **Настройки**, затем вручную обновите учетные данные. После успешного обновления набора данных вернитесь в [!INCLUDE[prodshort](includes/prodshort.md)] и вручную выберите отчет на странице **Выбрать отчеты**.


## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/configure-powerbi-excel-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Business Central и Power BI](admin-powerbi.md)  
[Создание отчетов Power BI для отображения данных [!INCLUDE [prodlong](includes/prodlong.md)]](across-how-use-financials-data-source-powerbi.md)  
[Обзор компонентов и архитектуры интеграции Power BI для [!INCLUDE[prodshort](includes/prodshort.md)]](admin-powerbi-overview.md)  
[Работа с данными [!INCLUDE [prodshort](includes/prodshort.md)] в Power BI](across-working-with-business-central-in-powerbi.md)  
[Power BI для потребителей](/power-bi/consumer/end-user-consumer)  
["Новый внешний вид" службы Power BI](/power-bi/service-new-look)  
[Быстрый старт: подключение к данным в Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  
[Документация Power BI](/power-bi/)  
[Бизнес-аналитика](bi.md)  
[Приступая к работе](product-get-started.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных Power BI](across-how-use-financials-data-source-powerbi.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] как источника данных Power Apps](across-how-use-financials-data-source-powerapps.md)  
[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в Power Automate](across-how-use-financials-data-source-flow.md)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
