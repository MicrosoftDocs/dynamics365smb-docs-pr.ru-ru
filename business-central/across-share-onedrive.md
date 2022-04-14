---
title: Открытие файлов Business Central в OneDrive
description: Узнайте, как вы можете обмениваться данными Business Central через OneDrive для бизнеса.
author: jswymer
ms.topic: conceptual
ms.workload: na
ms.search.keywords: ''
ms.date: 02/28/2022
ms.author: jswymer
ms.openlocfilehash: 2e1cc04d265541c87244dcd6c13b14327f07cc2f
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "8516425"
---
# <a name="opening-and-sharing-business-central-files-in-onedrive"></a>Открытие файлов Business Central и общий к ним доступ в OneDrive

[!INCLUDE[prod_short](includes/prod_short.md)] позволяет легко хранить, управлять и делиться файлами с другими людьми через OneDrive для бизнеса. На большинстве страниц, где доступны файлы, например в папке входящих отчетов или в файлах, прикрепленных к записям, вы найдете действия **Открыть в OneDrive** и **Поделиться**.


:::image type="content" source="media/onedrive-overview-report-inbox-w-outline.png" alt-text="Действия Открыть в OneDrive и Поделиться для отчетов":::


:::image type="content" source="media/one-drive-attachments-w-outline.png" alt-text="Действия Открыть в OneDrive и Поделиться для вложений":::

<!--
:::image type="content" source="media/Open in OneDrive.PNG" alt-text="The Open in OneDrive action":::

 
:::image type="content" source="media/OneDrive attachment.PNG" alt-text="Share file attachments in OneDrive":::
-->

## <a name="open-in-onedrive"></a>Открыть в OneDrive

Действие **Открыть в OneDrive** копирует файл на ваш OneDrive и открывает файл в своих онлайн-приложениях, таких как Excel Online, Word Online и PowerPoint Online. 

<!--## Working with Different Types of Files-->

Когда вы выбираете **Открыть в OneDrive**, [!INCLUDE[prod_short](includes/prod_short.md)] определяет файлы Excel, Word и PowerPoint и открывает их в своих онлайн-приложениях, то есть в Excel Online, Word Online и PowerPoint Online. Вы можете комментировать, редактировать и сотрудничать с другими, не выходя из браузера.

Для других популярных типов файлов, таких как PDF, текстовые файлы и изображения, OneDrive дает средства просмотра файлов, которые предлагают функции для печати, совместного использования и т. д. Если файл нельзя просмотреть в OneDrive, вам может быть предложено загрузить его.

## <a name="share"></a>Доля

Действие **Поделиться** копирует файл в ваш OneDrive и позволяет поделиться файлом с другими людьми и узнать, с кем вы уже поделились файлом. Когда вы выбираете действие **Поделиться**, откроется следующая страница.

:::image type="content" source="media/share-to-onedrive-dialog.PNG" alt-text="Поделиться файлом в OneDrive":::

Если вы знакомы с OneDrive, вы можете узнать страницу. У вас есть два варианта поделиться файлом: **Отправить ссылку** и **Копировать ссылку**.

- **Отправить ссылку** позволяет делиться файлами с конкретными людьми. Люди, которым вы поделитесь файлом, получат электронное письмо со ссылкой на файл. Файл также появится в разделе **Общие** их OneDrive. Начните с ввода адресов электронной почты или имен контактов в **Поле имени, группы или электронной почты**.

- **Копировать ссылку** копирует ссылку на файл в OneDrive, поэтому вы можете использовать ссылку в других местах, таких как Facebook, Twitter или электронная почта. 

Прежде чем отправлять или копировать ссылку, установите разрешение на файл, которое вы хотите задать для людей. Вы можете увидеть текущую настройку в разделе **Отправить ссылку** и **Копировать ссылку**. В большинстве случаев будет **Любой, у кого есть ссылка, может редактировать, чтобы открыть ссылку** в зависимости от настроек, установленных вашим администратором. Чтобы изменить разрешения, выберите ссылку и внесите изменения на странице **Настройки ссылки**.

Функция обмена в Business Central основана на OneDrive. Чтобы узнать больше об общем доступе и разрешениях, см. [Общий доступ к файлам и папкам OneDrive](https://support.microsoft.com/en-us/office/share-onedrive-files-and-folders-9fcc2f7d-de0c-4cec-93b0-a82024800c07).

> [!NOTE]
> Действие **Поделиться** недоступно в приложении Business Central для мобильных устройств.

## <a name="first-time-sign-in-from-business-central"></a>Первый вход в систему из Business Central

Когда вы используете действие **Открыть в OneDrive** или **Поделиться** впервые, [!INCLUDE[prod_short](includes/prod_short.md)] делает следующее:

1. Открывает странице **Ознакомьтесь с условиями**. Прочтите страницу и, если вы согласны с условиями, выберите **Принимаю**, чтобы продолжить.
2. Открывает страницу **Выберите учетную запись** Выберите свою учетную запись или **используйте другую учетную запись**, если вы не видите свою, введите имя пользователя и пароль при появлении запроса.
3. Создает папку с именем [!INCLUDE[prod_short](includes/prod_short.md)] в OneDrive. 
4. В папке [!INCLUDE[prod_short](includes/prod_short.md)] он создает другую папку с тем же именем, что и компания, в которой вы работаете. Если вы работаете в нескольких компаниях, он создаст папку для компании, в которой вы работаете, при использовании действия **Открыть в OneDrive** и **Поделиться**. 
5. Помещает копию выбранного файла в папку, а затем открывает файл. В следующий раз, когда вы воспользуетесь действием, оно только скопирует и откроет файл. 

## <a name="managing-multiple-copies-of-a-file"></a>Управление несколькими копиями файла

Когда вы выбираете **Открыть в OneDrive** или **Поделиться**, файл копируется из [!INCLUDE[prod_short](includes/prod_short.md)] в вашу папку в OneDrive. Если вы отредактируете файл в OneDrive, копии файла будут другими. Чтобы обновить [!INCLUDE[prod_short](includes/prod_short.md)] до актуального файла, удалите существующий файл из [!INCLUDE[prod_short](includes/prod_short.md)], а затем отправьте последнюю копию.

Кроме того, когда файл с таким именем уже существует в OneDrive, [!INCLUDE[prod_short](includes/prod_short.md)] предоставит выбор: заменить файл или оставить оба файла. Если вы решите сохранить оба файла, новый файл будет скопирован в OneDrive с суффиксом у имени файла, например "Items (2).xlsx,". Исходный файл не изменен. 

Если вы решите заменить файл, новый файл будет добавлен в журнал версий этого файла. Исходный файл не теряется, и вы можете просмотреть или восстановить предыдущие версии файла. 

## <a name="about-your-business-central-folder-on-onedrive"></a>О вашей папке Business Central в OneDrive

Папка и ее содержимое остаются личными, пока вы не решите поделиться ими с другими. Например, вы можете решить поделиться контентом с одним или несколькими коллегами или даже с людьми за пределами вашей организации. Вы можете получить доступ к своему OneDrive на странице **Мои параметры**, выбрав ссылку в поле **Облачное хранилище**. Дополнительные сведения см. в разделе [Общий доступ к файлам и папкам OneDrive](https://support.microsoft.com/en-us/office/share-onedrive-files-and-folders-9fcc2f7d-de0c-4cec-93b0-a82024800c07).

:::image type="content" source="media/my-settings-cloud-storage.PNG" alt-text="Поле облачного хранилища в Мои параметры":::

<!--## Extending the Connection to OneDrive
You can create an extension and connect it to... For more information, see...-->

## <a name="see-also"></a>См. также
[Интеграция Business Central и OneDrive](across-onedrive-overview.md)  
[Управление интеграцией OneDrive с Business Central](admin-onedrive-integration.md)  
[Часто задаваемые вопросы по OneDrive](admin-onedrive-faq.md)