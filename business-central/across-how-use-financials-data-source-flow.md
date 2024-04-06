---
title: Использование потоков Power Automate в Business Central
description: Настройте и используйте потоки Power Automate для создания и изменения данных Business Central.
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.service: dynamics-365-business-central
ms.topic: conceptual
ms.search.keywords: 'workflow, OData, Power App, SOAP, Power Automate,'
ms.search.form: '1500,'
ms.date: 08/31/2023
ms.custom: bap-template
---

<!-- Line 41 says there are three cloud flow types, but the table lists four. Should line 41 change? -->


# <a name="use-power-automate-flows-in-"></a>Использование потоков Power Automate в [!INCLUDE[prod_short](includes/prod_short.md)]

В составе [!INCLUDE[prod_short](includes/prod_short.md)] вы получаете лицензию на Microsoft Power Automate. Эта лицензия позволяет вам использовать данные [!INCLUDE[prod_short](includes/prod_short.md)] как часть рабочего процесса в Microsoft Power Automate. Вы можете создавать потоки и подключаться к своим данным из внутренних и внешних источников посредством соединителя [!INCLUDE [prod_short](includes/prod_short.md)].

Потоки Power Automate запускаются событиями, такими как создание, изменение или удаление записи. Также они могут запускаться по заданному пользователем расписанию или по запросу.

> [!NOTE]
> Администраторы могут ограничить доступ к Power Automate. Если вы обнаружите, что у вас нет доступа к некоторым или всем функциям, описанным в этой статье, обратитесь к своему администратору. Если вы хотите узнать, как управлять доступом к Power Automate в качестве администратора, см. статью [ Настройка интеграции с Power Automate](/dynamics365/business-central/dev-itpro/powerplatform/power-automate-setup).

<!-- You must have a valid account with both [!INCLUDE[prod_short](includes/prod_short.md)] and Power Automate. --> 

> [!TIP]
> Кроме Power Automate, в [!INCLUDE[prod_short](includes/prod_short.md)] можно использовать шаблоны рабочего процесса утверждения. Хотя это две отдельные системы для создания рабочих процессов, любой шаблон рабочего процесса утверждения, созданный в Power Automate, добавляется в список рабочих процессов в [!INCLUDE[prod_short](includes/prod_short.md)]. Подробнее см. в разделе [Рабочие процессы](across-workflow.md).

## <a name="about-power-automate-flows"></a>О потоках Power Automate

Power Automate — это служба, которая позволяет создавать автоматизированные рабочие процессы (или потоки) между приложениями и службами, такими как [!INCLUDE[prod_short](includes/prod_short.md)]. Умение писать код для создания потоков Power Automate практически не требуется. Они могут быть связаны с широким спектром событий и ответов, таких как:

- Изменения записей
- Обновления внешних файлов
- Учтенные документы
- Различные службы Майкрософт и и сторонние службы, такие как Microsoft Outlook, Excel, Dataverse, Teams, SharePoint, Power Apps и т. д.

Существует три разных типа облачных потоков, с которыми вы можете работать:

|Тип потока|Описанием|
|---------|-----------|
|Автоматизированный поток|Этот тип потока запускается автоматически по событию. В [!INCLUDE[prod_short](includes/prod_short.md)] событием может быть создание, изменение или удаление записи или документа. Так, например, новый счет продажи может инициировать поток для запроса утверждения, для которого могут быть заданы разные события в зависимости от ответа утверждающего. При отрицательном ответе отправителю запроса на утверждение отправляется уведомление и электронное письмо. Положительный ответ одновременно обновляет электронную таблицу Excel, расположенную в папке SharePoint, и отправляет обновление в чат Teams. Автоматизированные потоки могут запускаться как внутренними, так и внешними событиями в [!INCLUDE[prod_short](includes/prod_short.md)].|
|Поток утверждения|Потоки утверждения также являются автоматизированными потоками в Power Automate, но они предназначены специально для запроса утверждения при внесении изменений в записи и данные. Вы можете использовать потоки утверждения в Power Automate в качестве альтернативы [функции рабочих процессов утверждения](across-use-workflows.md), предусмотренной в [!INCLUDE[prod_short](includes/prod_short.md)]. |
|Поток по расписанию|Этот тип потока также запускается автоматически, но периодически в запланированные дату и время. |
|Мгновенный поток|Этот тип потока запускается по запросу, то есть пользователь должен запускать его вручную с помощью кнопки или действия в другом приложении или устройстве, в данном случае в клиенте [!INCLUDE[prod_short](includes/prod_short.md)]. Мгновенные потоки работают аналогично пакетным ярлыкам, выполняя несколько длительных шагов с помощью нескольких нажатий кнопок и запуская их с определенных страниц или таблиц. Например, поток может добавить кнопку в меню действий на странице **Поставщики**, чтобы блокировать платежи поставщику и, в то же время, отправлять настраиваемые электронные письма контактному лицу поставщика и закупщикам вашей компании, а также обновлять контакт в Outlook. |

## <a name="power-automate-features"></a>Функции Power Automate

Вы можете просмотреть все потоки Power Automate, доступные вам в данный момент, войдя в систему в [Power Automate](https://powerautomate.com) и выбрав **Мои потоки** на панели навигации слева. Здесь вы найдете все потоки, которые вы уже создали сами, и потоки, которыми с вами поделились администратор или коллеги.

- Мгновенные потоки также доступны для запуска непосредственно с большинства страниц списков, карточек и документов в [!INCLUDE[prod_short](includes/prod_short.md)]. Мгновенные потоки находятся в группе действий **Автоматизация** на панели действий на страницах. Чтобы запустить поток, выберите его и следуйте инструкциям. Подробнее см. в разделах ниже.

- Автоматизированные потоки [!INCLUDE[prod_short](includes/prod_short.md)] не требуют никаких действий с вашей стороны, кроме случаев, когда вы хотите изменить их или отключить. В противном случае они просто работают при срабатывании триггера. 
<!--

## <a name="automated-flows"></a>Automated flows

With Power Automate, you can create business flows directly in-house and rely on citizen developers. Automated workflows can be started by both internal and external events in [!INCLUDE[prod_short](includes/prod_short.md)], and also be set to run periodically. Learn more and get instructions on how to create flows in the [Set Up Automated Workflows](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) article in the administration content.

-->

## <a name="run-instant-flows"></a>Запуск мгновенных потоков

Мгновенные потоки открываются внутри [!INCLUDE [prod_short](includes/prod_short.md)] Online, чтобы вы оставались в контексте бизнес-процесса, над которым работаете. Вы можете запустить мгновенный поток из большинства списков, карточек или документов.

1. На панели действий выберите **Автоматизация**, а затем выберите поток из списка доступных потоков в действии **Power Automate**.

    :::image type="content" source="media/power-automate-instant-menu.svg" alt-text="Показано действие «Автоматизация» с мгновенными потоками.":::

    На некоторых страницах пункт **Автоматизация** находится внутри пункта **Еще (...)**. 
2. На панели **Run Flow** заполните все необходимые поля, затем выберите **Продолжить**, чтобы запустить поток.

> [!NOTE]
> При первом использовании пункта **Автоматизация**, возможно, вы увидите только действие **Начало работы с Power Automate**. Вы видите это действие, потому что не приняли уведомление о конфиденциальности для Microsoft Power Automate. Чтобы продолжить, выберите **Начало работы с Power Automate** и следуйте инструкциям, чтобы принять или не принимать уведомление.  
>
> :::image type="content" source="media/power-automate-action.png" alt-text="Показывает пункт «Автоматизация» на панели действий.":::

<!--

[!INCLUDE [prod_short](includes/prod_short.md)] can run a Power Automate flow from most list, card, and document pages. Once the admin has connected [!INCLUDE [prod_short](includes/prod_short.md)] with Power Automate, you'll see any flows your organization has added when you choose the **Automate** action on the relevant pages. Instant flows are run without leaving [!INCLUDE [prod_short](includes/prod_short.md)]. Learn more in the [Set Up Automated Workflows](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) article in the administration content.

These instant flows open on a page inside [!INCLUDE [prod_short](includes/prod_short.md)] online so you can remain within the context of the business process you were in the middle of. Choose the **Automate** action—on some pages nested under the **More Options** menu—choose the **Power Automate** menu item, then choose the relevant link to trigger the workflow. The connection to Power Automate is already set up for you.

Most flows require you to fill in a field or two before you choose the **Run flow** action.

> [!TIP]
> If you don't see an **Automate** action, then your [!INCLUDE [prod_short](includes/prod_short.md)] probably hasn't yet been set up to use Power Automate. Learn more from your admin.-->

## <a name="create-edit-and-manage-flows"></a>Создание и редактирование потоков, а также управление ими

Создание новых потоков, их изменение и управление существующими потоками (например, их включение или выключение) может осуществляться непосредственно в Power Automate. Однако вы можете инициировать некоторые из этих задач из меню действий «Автоматизация» в [!INCLUDE[prod_short](includes/prod_short.md)]:

:::image type="content" source="media/power-automate-menu.svg" alt-text="Показывает действие «Автоматизация» на панели действий с развернутыми действиями.":::

- Чтобы создать автоматизированный поток со страницы списка, карточки или документа, выберите **Автоматизация** > **Создать автоматизированный поток**.
- Чтобы создать поток утверждения со страницы карточки или документа, выберите **Автоматизация** > **Создать поток утверждения**.

  > [!TIP]
  > Это действие доступно только на страницах типа «карточка» и «документ», но не на страницах списков.
- Чтобы создать мгновенный поток со страницы списка, карточки или документа, выберите **Автоматизация** > **Создать действие на основе потока**.
- Чтобы открыть Power Automate со страницы списка, карточки или документа, выберите **Автоматизация** > **Управление потоками**.
<!--- To create new flows or manage existing flows from inside [!INCLUDE[prod_short](includes/prod_short.md)], got to the **Manage Power Automate Flows** page.-->

Некоторые задачи обычно выполняются администраторами или суперпользователями. Эти задачи требуют более обширных знаний о бизнес-процессах в [!INCLUDE[prod_short](includes/prod_short.md)]. Подробнее см. в следующих статьях в справке для разработчиков и ИТ-специалистов Business Central:

- [Интеграция с Power Automate](/dynamics365/business-central/dev-itpro/powerplatform/power-automate-overview)
- [Создание автоматизированных потоков](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows) (в этой статье также рассматриваются потоки утверждения)
- [Создание мгновенных потоков](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows)
- [Управление потоками Power Automate](/dynamics365/business-central/dev-itpro/powerplatform/manage-power-automate-flows)
<!-- 

## <a name="add-more-automated-flows-and-instant-flows"></a>Add more automated flows and instant flows

You can create flows through the [powerautomate.microsoft.com](https://powerautomate.microsoft.com) website. However, if your admin has switched on the capability to run Power Automate flows from inside [!INCLUDE [prod_short](includes/prod_short.md)] online, you can start the process of building a flow from the **Automate** action on the relevant pages, which can be found under the **More Options** menu depending on the page. Then choose the **Power Automate** menu item, and then choose the **Create a flow** action. Power Automate then opens in a new browser tab, and you're signed in automatically.

You can find sample templates to adapt to your company and all available trigger events, using both [!INCLUDE [prod_short](includes/prod_short.md)] and external tools, by choosing the **Connectors** menu on the Power Automate website. Learn more about available templates and triggers in the [Set Up Automated Workflows](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows) article in the administration content.

## <a name="create-and-manage-power-automate-flows"></a>Create and manage Power Automate flows

You can create new flows or manage existing Power Automate flows in [!INCLUDE [prod_short](includes/prod_short.md)] on the **Manage Power Automate Flows** page. Learn more in the [Manage Power Automate Flows](/dynamics365/business-central/dev-itpro/powerplatform/manage-power-automate-flows) article in the administration content.

<!--
You can also manage available Power Automate workflows on the **Workflows** page in [!INCLUDE[prod_short](includes/prod_short.md)]. The page lists both the built-in approval and Power Automate workflows, with options for the latter to enable/disable, delete, and view the workflow on the Power Automate website.-->

## <a name="see-also"></a>См. также

[Устранение неполадок в автоматизированных рабочих процессах [!INCLUDE[prod_short](includes/prod_short.md)]](across-flow-troubleshoot.md)  
[Подготовка к ведению бизнеса](ui-get-ready-business.md)  
[Рабочие процессы](across-workflow.md)  
[Импорт бизнес-данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Назначение разрешений пользователям и группам](ui-define-granular-permissions.md)  
[Настройка [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Финансовый менеджмент](finance.md)  
[Управление потоками Power Automate](/dynamics365/business-central/dev-itpro/powerplatform/manage-power-automate-flows)  
[Настройка автоматизированных рабочих процессов](/dynamics365/business-central/dev-itpro/powerplatform/automate-workflows)  
[Включение мгновенных потоков](/dynamics365/business-central/dev-itpro/powerplatform/instant-flows)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
