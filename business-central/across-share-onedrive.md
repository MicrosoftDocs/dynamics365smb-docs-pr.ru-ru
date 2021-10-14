---
title: Использование OneDrive для бизнеса с Business Central
description: Вы можете использовать OneDrive для бизнеса для хранения, управления и обмена файлами, например отчетами или вложенными файлами.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.workload: na
ms.search.keywords: ''
ms.date: 06/11/2021
ms.author: bholtorf
ms.openlocfilehash: 92896af6888ef5c39288d511e61d343d3e384a83
ms.sourcegitcommit: 6ad0a834fc225cc27dfdbee4a83cf06bbbcbc1c9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2021
ms.locfileid: "7589489"
---
# <a name="opening-business-central-files-in-onedrive"></a>Открытие файлов Business Central в OneDrive
[!INCLUDE[prod_short](includes/prod_short.md)] позволяет легко хранить, управлять и делиться файлами с другими людьми через OneDrive для бизнеса. На большинстве страниц, где доступны файлы, например в папке входящих отчетов или в файлах, прикрепленных к записям, вы найдете действие **Открыть в OneDrive**.

:::image type="content" source="media/Open in OneDrive.PNG" alt-text="Действие Открыть в OneDrive":::

 
:::image type="content" source="media/OneDrive attachment.PNG" alt-text="Делитесь вложениями файлов в OneDrive":::

## <a name="working-with-different-types-of-files"></a>Работа с разными типами файлов
Когда вы выбираете **Открыть в OneDrive**, [!INCLUDE[prod_short](includes/prod_short.md)] определяет файлы Excel, Word и PowerPoint и открывает их в своих онлайн-приложениях, то есть в Excel Online, Word Online и PowerPoint Online. Вы можете комментировать, редактировать и сотрудничать с другими, не выходя из браузера. 

Для других популярных типов файлов, таких как PDF, текстовые файлы и изображения, OneDrive дает средства просмотра файлов, которые предлагают функции для печати, совместного использования и т. д. Если файл нельзя просмотреть в OneDrive, вам может быть предложено загрузить его. 

## <a name="managing-multiple-copies-of-a-file"></a>Управление несколькими копиями файла
Когда вы выбираете **Открыть в OneDrive**, файл копируется из [!INCLUDE[prod_short](includes/prod_short.md)] в вашу папку в OneDrive. Если вы отредактируете файл в OneDrive, копии файла будут другими. Чтобы обновить [!INCLUDE[prod_short](includes/prod_short.md)] до актуального файла, удалите существующий файл из [!INCLUDE[prod_short](includes/prod_short.md)], а затем отправьте последнюю копию.

Кроме того, когда вы используете действие Открыть в OneDrive и файл с таким именем уже существует в OneDrive, [!INCLUDE[prod_short](includes/prod_short.md)] предоставит выбор: заменить файл или оставить оба файла. Если вы решите сохранить оба файла, новый файл будет скопирован в OneDrive и его имени файла присваивается суффикс, например "Items (2).xlsx", а исходный файл не изменяется. 

Если вы решите заменить файл, новый файл будет добавлен в журнал версий этого файла. Исходный файл не теряется, и вы можете просмотреть или восстановить предыдущие версии файла. 

## <a name="accessing-your-onedrive"></a>Доступ к вашему OneDrive
Вы можете получить доступ к своему OneDrive на странице **Мои параметры**, выбрав ссылку в поле **Облачное хранилище**.

:::image type="content" source="media/my-settings-cloud-storage.PNG" alt-text="Поле облачного хранилища в Мои параметры":::

<!--## Extending the Connection to OneDrive
You can create an extension and connect it to... For more information, see...-->

## <a name="see-also"></a>См. также
[Интеграция Business Central и OneDrive](across-onedrive-overview.md)  
[Управление интеграцией OneDrive с Business Central](admin-onedrive-integration.md)  
[Часто задаваемые вопросы по OneDrive](admin-onedrive-faq.md)