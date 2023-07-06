---
title: Управление интеграцией OneDrive с Business Central
description: 'Узнайте о том, что вы можете сделать для управления интеграцией между Business Central и OneDrive для бизнеса.'
author: jswymer
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'OneDrive, share, browser'
ms.date: 02/28/2022
ms.author: jswymer
---
# <a name="managing-onedrive-integration-with-business-central"></a><a name="managing-onedrive-integration-with-business-central"></a><a name="managing-onedrive-integration-with-business-central"></a>Управление интеграцией OneDrive с Business Central

В этой статье представлен обзор того, что администратор может делать для управления интеграцией OneDrive для бизнеса с [!INCLUDE[prod_short](includes/prod_short.md)]. Пользователи [!INCLUDE[prod_short](includes/prod_short.md)] Online могут использовать функции "Открыть в OneDrive" и "Поделиться" за счет автоматической интеграции, не требующей дополнительной настройки. Мастер настройки **Настройка OneDrive Setup** позволяет предоставить в распоряжение пользователей еще больше функций OneDrive, например открытие файлов Excel в OneDrive &mdash; или же отключить все эти функции.  

## <a name="configure-onedrive-for-integration-with-business-central"></a><a name="configure-onedrive-for-integration-with-business-central"></a><a name="configure-onedrive-for-integration-with-business-central"></a>Настройка OneDrive для интеграции с Business Central

В этом разделе рассматриваются требования, которые должны выполняться в OneDrive для бизнеса для настройки интеграции с Business Central, а также задача, выполняемая для управления этой интеграцией.

### <a name="minimum-requirements"></a><a name="minimum-requirements"></a><a name="minimum-requirements"></a>Минимальные требования

* У каждого пользователя должна быть лицензия на [!INCLUDE[prod_short](includes/prod_short.md)] и OneDrive в составе плана Microsoft 365.
* OneDrive должны быть настроены для каждого пользователя.

### <a name="managing-privacy"></a><a name="managing-privacy"></a><a name="managing-privacy"></a>Управление конфиденциальностью

> [!IMPORTANT]
> Если вы решили развернуть Business Central и OneDrive в разных странах или регионах, файлы, созданные Business Central и помещенные в OneDrive, могут пересекать границы мест расположения данных. Не забудьте свериться с политиками вашей организациями и законодательными требованиями в отношении мест хранения данных, прежде чем включать подключение к OneDrive.

Администраторы и конечные пользователи контролируют контент, хранящийся в OneDrive, и эти данные принадлежат исключительно вашей организации. Для получения дополнительной информации см. [Как SharePoint и OneDrive защищают ваши данные в облаке](/sharepoint/safeguarding-your-data). Вы также можете прочесть наше [Заявление о конфиденциальности Microsoft](https://privacy.microsoft.com/en-us/privacystatement), в котором объясняется, какие данные обрабатывает Microsoft, как Microsoft обрабатывает их и для каких целей.

Включая это подключение к службе, вы соглашаетесь:

а) на передачу данных из этого экземпляра Dynamics 365 Business Central поставщику службы, который будет использовать их в соответствии со своими условиями и политикой конфиденциальности; б) с тем, что уровни соответствия поставщика службы могут отличаться от уровней соответствия Dynamics 365 Business Central; а также в) что корпорация Майкрософт может передавать вашу контактную информацию поставщику этой службы, если она понадобится ему для обеспечения работы службы и устранения неполадок.

## <a name="configure-business-central"></a><a name="configure-business-central"></a><a name="configure-business-central"></a>Настройка Business Central

В Business Central Online подключение между Business Central и OneDrive настраивается автоматически, и функции OneDrive по умолчанию готовы к использованию пользователями. Если вы хотите отключить некоторые или все функции, вы можете использовать мастер настройки **Настройка OneDrive** в клиенте Business Central.

Настройка локальных версий Business Central происходит иначе, потому что подключение между Business Central и OneDrive в этом случае не настроено автоматически. Вам необходимо сделать это вручную. Дополнительные сведения см. в статье [Настройка интеграции OneDrive с локальной версией Business Central](admin-onedrive-integration-onpremises.md).

### <a name="about-multiple-environments"></a><a name="about-multiple-environments"></a><a name="about-multiple-environments"></a>О нескольких средах

Интеграция с OneDrive настраивается для среды, то есть заданные вами параметры будут применяться ко всем организациям в этой среде. Если у вашей организации несколько сред, вам придется настроить интеграцию с OneDrive для каждой из них.

### <a name="prerequisites"></a><a name="prerequisites"></a><a name="prerequisites"></a>Предварительные требования

- Разрешение на вставку, изменение и удаление (imd) в отношении таблицы **Document Service Scenario** (как минимум)

### <a name="configure-onedrive-using-onedrive-setup"></a><a name="configure-onedrive-using-onedrive-setup"></a><a name="configure-onedrive-using-onedrive-setup"></a>Настройка OneDrive с использованием мастера "Настройка OneDrive"

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Настройка OneDrive**, а затем выберите соответствующую ссылку. 
2. При первом запуске мастера настройки вы увидите страницу **Ваша конфиденциальность**. Прочитайте информацию на странице и, если вы согласны с условиями, выберите **Принимаю**, чтобы продолжить.
3. На странице **Настройка обработки файлов** вы можете выбрать один из следующих вариантов:

   [!INCLUDE[onedrive-feature-options](includes/onedrive-feature-options.md)]
4. Выберите **Далее**>**Готово**.

### <a name="switching-to-new-onedrive-integration-after-upgrade"></a><a name="switching-to-new-onedrive-integration-after-upgrade"></a><a name="switching-to-new-onedrive-integration-after-upgrade"></a>Переход на новую интеграцию с OneDrive после обновления

Мастер настройки **Настройка OneDrive** появился в волне 2 выпуска 2022 года (версия 21.0). Ранее для интеграции с OneDrive использовалась страница **Настройка подключения к SharePoint**, которая устарела и будет удалена в волне 2 выпуска 2023 года (версии 23.0). После обновления до версии 21 OneDrive будет работать как прежде. Мы, однако же, рекомендуем перейти на новую интеграцию с OneDrive. Совершение этого перехода сейчас упростит вам задачу тогда, когда страница **Настройка подключения к SharePoint** в конечном итоге будет удалена. Кроме того, это позволит вам использовать мастер настройки **Настройка OneDrive** для управления функциями OneDrive, доступными пользователям. Мастер настройки **Настройка OneDrive** позволяет перейти со старой настройки через SharePoint на новую интеграцию легко и быстро.

Для перехода просто откройте мастер настройки **Настройка OneDrive** напрямую или откройте страницу **Настройка подключения к SharePoint** и выберите **Перейти в новый интерфейс настройки OneDrive** в уведомлении вверху страницы. Следуйте инструкциям в мастере, как описано в предыдущем разделе.

## <a name="restoring-onedrive-and-"></a><a name="restoring-onedrive-and-"></a><a name="restoring-onedrive-and-"></a>Восстановление OneDrive и [!INCLUDE[prod_short](includes/prod_short.md)]

В рамках процедуры аварийного восстановления администратору может потребоваться восстановить среду [!INCLUDE[prod_short](includes/prod_short.md)] Online из резервной копии на момент в прошлом и синхронизировать хранилище OneDrive с этим моментом времени. В OneDrive предусмотрены различные инструменты для аварийного восстановления, такие как восстановление OneDrive пользователя к предыдущему моменту, восстановление предыдущей версии отдельного файла или восстановление удаленных файлов. Для получения дополнительных сведений см. следующие статьи:

* Для [!INCLUDE[prod_short](includes/prod_short.md)] см. [Восстановление среды в центре администрирования](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-backup-restore).
* Для OneDrive см. [Восстановление OneDrive](https://support.microsoft.com/en-us/office/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15?ui=en-us&rs=en-us&ad=us)

## <a name="governance"></a><a name="governance"></a><a name="governance"></a>Управление

Центр администрирования SharePoint обеспечивает широкий контроль над политиками, которые регулируют использование OneDrive во всей организации. Глобальные администраторы или пользователи, у которых есть роль администратора SharePoint, могут настраивать политики, определяющие, у кого есть доступ к OneDrive, где хранятся данные, жизненный цикл контента и многое другое. Следующие ссылки предоставляют информацию о часто используемых функциях и настройках, которые могут улучшить вашу интеграцию с [!INCLUDE[prod_short](includes/prod_short.md)]. 

* [Управление настройками общего доступа](/sharepoint/turn-external-sharing-on-or-off)
* [Используйте информационные барьеры с SharePoint](/sharepoint/information-barriers)
* [Узнайте о защите от потери данных](/microsoft-365/compliance/dlp-learn-about-dlp)
* [Установите пространство для хранения по умолчанию для пользователей OneDrive](/onedrive/set-default-storage-space)
* [Добавление и удаление администраторов для OneDrive пользователя](/sharepoint/manage-user-profiles#add-and-remove-admins-for-a-users-onedrive)
* [Запрет создания OneDrive для некоторых пользователей](/sharepoint/manage-user-profiles#disable-onedrive-creation-for-some-users)
* [Возможности Multi-Geo в OneDrive и SharePoint Online](/microsoft-365/enterprise/multi-geo-capabilities-in-onedrive-and-sharepoint-online-in-microsoft-365)

> [!NOTE]
> Некоторые функции могут быть доступны только для определенных планов.

## <a name="see-also"></a><a name="see-also"></a><a name="see-also"></a>См. также

[Интеграция Business Central и OneDrive для бизнеса](across-onedrive-overview.md)  
[Открытие файлов Business Central в OneDrive](across-share-onedrive.md)  
[Часто задаваемые вопросы по OneDrive](admin-onedrive-faq.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
