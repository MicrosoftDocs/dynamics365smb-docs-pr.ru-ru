---
title: Использование Business Central с Outlook | Документация Майкрософт
description: Эта служба обладает глубокой интеграцией с Microsoft 365, что позволяет вам вести бизнес и взаимодействовать по электронной почте с клиентами и поставщиками непосредственно из Outlook.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: SMTP, mail, Microsoft 365
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 2c8746098081a8f0b961f6ab2efd11c491104acc
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115390"
---
# <a name="using-business-central-as-your-business-inbox-in-outlook"></a>Использование Business Central в качестве папки "Входящие" для бизнеса в Outlook

В [!INCLUDE[prod_short](includes/prod_short.md)] появилась возможность управления бизнес-взаимодействиями с клиентами и поставщиками непосредственно в Microsoft Outlook. С помощью надстроек [!INCLUDE[prod_short](includes/prod_short.md)] Outlook вы можете просматривать финансовые данные, связанные с клиентами и поставщиками, а также создавать и отправлять финансовые документы, такие как предложения и счета.  

## <a name="getting-the-add-in"></a>Получение надстройки
Легко начать работать с надстройкой [!INCLUDE[prod_short](includes/prod_short.md)] for Outlook. В руководстве мастера настройки **Настройка папки "Входящие" для бизнеса в Outlook** можно настроить связь для себя или для организации, если организация использует Microsoft 365. Просто укажите свое имя пользователя и пароль Microsoft 365, если будет предложено, и сообщите нам, если вы хотите получить образец сообщения электронной почты. После этого надстройки [!INCLUDE[prod_short](includes/prod_short.md)] будут автоматически добавлены в Outlook. Для получения дополнительной информации см. [Минимальные требования для Outlook ](product-requirements.md#outlook).  

Затем при открытии Outlook отобразится сообщение электронной почты от *администратора Dynamics 365 Business Central*. Новые надстройки будут добавлены в ленту Outlook, а в браузере вы сможете видеть надстройки [!INCLUDE[prod_short](includes/prod_short.md)] непосредственно над телом сообщения электронной почты. Надстройки будут обновляться периодически, и вы будете получать уведомления о том, что новая версия готова к использованию в Outlook.  

> [!TIP]
> Если вы используете новую веб-версию Outlook, то надстройки [!INCLUDE[prod_short](includes/prod_short.md)] могут быть скрыты в пункте **Другие действия**. Если вы часто используете надстройку, вы можете закрепить ее так, чтобы она всегда была видна сразу. Для получения дополнительной информации см. [Использование надстроек в Outlook в Интернете ](https://support.office.com/article/using-add-ins-in-outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce?ns=OLWAO365B&version=16).  

Если вы работаете с более чем одной компанией [!INCLUDE[prod_short](includes/prod_short.md)], вы можете легко переключаться между компаниями в Outlook. На панели действий надстройки выберите **Другие действия**, а затем вы можете увидеть вариант для переключения между компаниями.  

<!--TEMP-->
> [!NOTE]
> Переключение между компаниями требует [!INCLUDE[prod_short](includes/prod_short.md)] 2019 выпуска волны 2 или позже, как объявлено в [плане выпуска](/dynamics365-release-plan/2019wave2/dynamics365-business-central/switch-between-companies-business-inbox-outlook).

Некоторые организации, использующие Microsoft 365, ограничивают права пользователей на развертывание надстроек. Поэтому вам следует убедиться, что вы используете подписку Microsoft 365, включающую электронную почту и позволяющую развертывать надстройки. Если вы хотите попробовать надстройку в любом случае, вы можете [попробовать Microsoft 365 бесплатно](https://www.microsoft.com/microsoft-365/try).  

## <a name="using-the-contact-insights-add-in"></a>Использование надстройки Contact Insights
Допустим, вы получили сообщение электронной почты от клиента, который желает получить предложение по определенным товарам. Непосредственно в Outlook вы можете открыть надстройку [!INCLUDE[prod_short](includes/prod_short.md)], которая распознает отправителя как клиента и откроет карточку клиента для этой компании. На этой панели вы видите обзорные сведения о клиенте, а также возможность просматривать более подробную информацию в конкретных документах. Можно также просмотреть историю продаж для клиента. Если это новый контакт, его можно создать как нового клиента в [!INCLUDE[prod_short](includes/prod_short.md)], не выходя из Outlook.  

В надстройке вы можете создать предложение по продаже и отправить его клиенту, не выходя из Outlook. Вся информация, которая вам нужна для отправки предложения продаже, доступна в рабочем почтовом ящике в Outlook.  
После ввода данных вы можете учесть предложение. Затем его можно отправить по электронной почте. [!INCLUDE[prod_short](includes/prod_short.md)] создает PDF-файл с предложением по продаже и прикрепляет его к сообщению электронной почты, черновик которого вы создаете в надстройке.  

Аналогично, если вы получаете сообщение электронной почты от поставщика, вы можете использовать надстройку для работы с поставщиками и счетами покупки.  

Иногда необходимо просмотреть больше полей, чем отображается в надстройке, например если вам нужно заполнить строки счета. Чтобы у вас было больше места для работы, вы можете открыть надстройку на отдельной странице. Она все еще будет частью Outlook, но более просторной. По мере ввода данных в документа в раскрывающемся представлении изменения автоматически сохраняются. После завершения ввода данных в документ можно нажать кнопку **ОК**. При выборе области надстройки в Outlook документ будет автоматически обновлен с учетом изменений, внесенных в раскрывающемся окне.  

## <a name="creating-invoices-from-your-meeting-appointments"></a>Создание счетов для встреч
Некоторые организации регистрируют все оплачиваемые встречи в календаре Outlook. С помощью [!INCLUDE[prod_short](includes/prod_short.md)] можно создать счет для клиента непосредственно из календарной позиции. Откройте встречу, откройте надстройку [!INCLUDE[prod_short](includes/prod_short.md)], найдите существующую информацию или создайте счет либо другой документ продажи прямо здесь.  

## <a name="doing-quick-document-lookup"></a>Быстрый поиск документов
Надстройка "Ссылки на документы [!INCLUDE[prod_short](includes/prod_short.md)] позволяет быстро находить документы, упоминаемые в сообщениях электронной почты. Надстройка доступна для сообщения электронной почты, если номер документа распознан в теле сообщения. Открытие надстройки позволяет быстро перейти к документу.  

Например, если вы получили сообщение электронной почты, содержащее текст *S-QUO100*, [!INCLUDE[prod_short](includes/prod_short.md)] определит, что это предложение по продаже, и вы можете открыть этот документ в Outlook. В Outlook нажмите кнопку **Ссылки на документ** непосредственно над телом сообщения электронной почты. В Outlook Web App выберите текст *S-QUO1001* в теле сообщения электронной почты.  

В надстройке "Ссылки на документы" вы можете изменять документ и выполнять с ним другие действия, как в [!INCLUDE[prod_short](includes/prod_short.md)].

## <a name="adding-the-add-ins-manually"></a>Добавление надстроек вручную
В некоторых случаях надстройки не добавляются автоматически в Outlook. Даже если вы или ваш коллега запускает руководство по сопровождаемой настройке от имени организации, [!INCLUDE[prod_short](includes/prod_short.md)] может не отобразиться в Outlook. При возникновении этой проблемы вы можете добавить надстройки [!INCLUDE[prod_short](includes/prod_short.md)] вручную.  

Прежде всего, необходимо проверить, что у вас есть доступ к надстройкам в учетной записи Microsoft 365. Просто откройте ваш Outlook в браузере, откройте сообщение, выберите **Больше действий** (...) в верхней части сообщения, затем в нижней части списка выберите **Получить надстройки**. При этом открывается страница **Надстройки для Outlook**, где вы можете включить [!INCLUDE[prod_short](includes/prod_short.md)] для вашего Outlook. Затем при переходе назад в Outlook приложение [!INCLUDE[prod_short](includes/prod_short.md)] должно быть доступно.  

Аналогичным образом, в настольном клиенте Outlook можно проверить, что приложение [!INCLUDE[prod_short](includes/prod_short.md)] перечислено на странице **Получить надстройки**.  

В обоих случаях, если [!INCLUDE[prod_short](includes/prod_short.md)] все еще отсутствует, необходимо получить файлы манифеста надстройки. Для получения более подробных сведений обратитесь к системному администратору Microsoft 365.

## <a name="using-other-email-accounts"></a>Использование других учетных записей электронной почты

Надстройки предназначены для использования с Microsoft 365. Если вы используете [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, ваш администратор узнает, можете ли вы использовать надстройки [!INCLUDE[prod_short](includes/prod_short.md)] в Outlook. Для получения дополнительной информации см. статьи [Какой адрес электронной почты можно использовать с [!INCLUDE[prod_short](includes/prod_short.md)]?](/dynamics365/business-central/across-faq#email), [Функции, которые требуют особых обстоятельств](/dynamics365/business-central/dev-itpro/features-not-implemented-on-premises#features-that-require-specific-circumstances?toc=/dynamics365/business-central/toc.json) и раздел [Почему надстройка Outlook не работает для моих пользователей?](/dynamics365/business-central/dev-itpro/faq#why-doesnt-the-outlook-add-in-work-for-my-users?toc=/dynamics365/business-central/toc.json) в общем разделе вопросов и ответов в материалах по администрированию.  

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/alternative-interfaces-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Подготовьтесь к ведению бизнеса](ui-get-ready-business.md)  
[Получение Business Central на моем мобильном устройстве](install-mobile-app.md)  
[Отправка документов по электронной почте](ui-how-send-documents-email.md)  
[Финансы](finance.md)  
[Продажи](sales-manage-sales.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Минимальные требования для Outlook](product-requirements.md#outlook)  
[Использование надстроек в Outlook в Интернете](https://support.office.com/article/Using-Add-ins-in-Outlook-on-the-web-8f2ce816-5df4-44a5-958c-f7f9d6dabdce?appver=OWB150)  


[!INCLUDE[footer-include](includes/footer-banner.md)]