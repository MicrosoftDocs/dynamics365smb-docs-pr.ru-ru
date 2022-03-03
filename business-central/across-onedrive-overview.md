---
title: Business Central и OneDrive для бизнес-интеграции
description: Вы можете использовать OneDrive для бизнеса для хранения, управления и обмена файлами, например отчетами или вложенными файлами.
author: bholtorf
ms.topic: overview
ms.workload: na
ms.search.keywords: ''
ms.date: 06/11/2021
ms.author: bholtorf
ms.openlocfilehash: f2c8efa4a32ef18ee4db25919c7e4405649d54bb
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2022
ms.locfileid: "8141467"
---
# <a name="business-central-and-onedrive-for-business-integration"></a>Business Central и OneDrive для бизнес-интеграции
OneDrive для бизнеса — это облачная служба хранения, входящая в состав Microsoft 365. [!INCLUDE[prod_short](includes/prod_short.md)] позволяет легко хранить, управлять и делиться файлами с другими людьми через OneDrive. Когда файл находится в вашем OneDrive, вы можете воспользоваться разнообразными возможностями совместной работы с помощью онлайн-версий продуктов Microsoft, таких как Word, Excel и PowerPoint. Например, вы можете поделиться документом Word, а затем вы и ваши коллеги сможете редактировать его вместе в режиме реального времени. OneDrive также позволяет открывать другие типы файлов, например PDF-файлы. 

## <a name="getting-started"></a>Приступая к работе
Мы создали связь между [!INCLUDE[prod_short](includes/prod_short.md)] Online и OneDrive, так что приступить к работе очень легко. Единственное требование — чтобы пользователи открыли OneDrive по крайней мере один раз. 

На большинстве страниц, где доступны файлы, например в папке входящих отчетов или в файлах, прикрепленных к записям, вы найдете действие **Открыть в OneDrive**.

:::image type="content" source="media/Open in OneDrive.PNG" alt-text="Действие Открыть в OneDrive":::

 
:::image type="content" source="media/OneDrive attachment.PNG" alt-text="Делитесь вложениями файлов в OneDrive":::

Когда вы используете действие **Открыть в OneDrive** впервые, [!INCLUDE[prod_short](includes/prod_short.md)] делает следующее в вашем OneDrive:

1. Создает папку с именем [!INCLUDE[prod_short](includes/prod_short.md)]. 
2. В папке [!INCLUDE[prod_short](includes/prod_short.md)] он создает другую папку с тем же именем, что и компания, в которой вы работаете. Если вы работаете в нескольких компаниях, он создаст папку для компании, в которой вы работаете, при использовании действия **Открыть в OneDrive**. 
3. Помещает копию выбранного файла в папку, а затем открывает файл. В следующий раз, когда вы воспользуетесь действием, оно только скопирует и откроет файл. 

Папка и ее содержимое остаются личными, пока вы не решите поделиться ими с другими. Например, вы можете решить поделиться контентом с одним или несколькими коллегами или даже с людьми за пределами вашей организации. Дополнительные сведения см. в разделе [Общий доступ к файлам и папкам OneDrive](https://support.microsoft.com/en-us/office/share-onedrive-files-and-folders-9fcc2f7d-de0c-4cec-93b0-a82024800c07).

> [!NOTE]
> Вы также можете подключить свою локальную версию [!INCLUDE[prod_short](includes/prod_short.md)] к OneDrive. Однако есть несколько кое-что, что нужно сделать, чтобы заставить это работать. Дополнительные сведения см. в разделе [Настройка локальной версии Business Central](admin-onedrive-integration.md#configuring-business-central-on-premises).

## <a name="see-also"></a>См. также
[Управление интеграцией OneDrive с Business Central](admin-onedrive-integration.md)  
[Открытие файлов Business Central в OneDrive](across-share-onedrive.md)  
[Часто задаваемые вопросы по OneDrive](admin-onedrive-faq.md)