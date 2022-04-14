---
title: Business Central и OneDrive для бизнес-интеграции
description: Вы можете использовать OneDrive для бизнеса для хранения, управления и обмена файлами, например отчетами или вложенными файлами.
author: jswymer
ms.topic: overview
ms.workload: na
ms.search.keywords: ''
ms.date: 02/28/2022
ms.author: jswymer
ms.openlocfilehash: 371c090e321992ec2fdc0ee7cb218feaa6b16d9a
ms.sourcegitcommit: 8a12074b170a14d98ab7ffdad77d66aed64e5783
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "8521232"
---
# <a name="business-central-and-onedrive-for-business-integration"></a>Business Central и OneDrive для бизнес-интеграции

OneDrive для бизнеса — это облачная служба хранения, входящая в состав Microsoft 365. [!INCLUDE[prod_short](includes/prod_short.md)] позволяет легко хранить, управлять и делиться файлами с другими людьми через OneDrive. Когда файл находится в вашем OneDrive, вы можете воспользоваться разнообразными возможностями совместной работы с помощью онлайн-версий продуктов Microsoft, таких как Word, Excel и PowerPoint. Например, вы можете поделиться документом Word, а затем вы и ваши коллеги сможете редактировать его вместе в режиме реального времени. OneDrive также позволяет открывать другие типы файлов, например PDF-файлы. 

## <a name="getting-started"></a>Приступая к работе

Мы создали связь между [!INCLUDE[prod_short](includes/prod_short.md)] Online и OneDrive, так что приступить к работе очень легко. Единственное требование — чтобы пользователи открыли OneDrive по крайней мере один раз. 

На большинстве страниц, где доступны файлы, например в папке входящих отчетов или в файлах, прикрепленных к записям, вы найдете действие **Открыть в OneDrive** и **Поделиться**.

:::image type="content" source="media/onedrive-overview-report-inbox-w-outline.png" alt-text="Действия Открыть в OneDrive и Поделиться для отчетов":::


:::image type="content" source="media/one-drive-attachments-w-outline.png" alt-text="Действия Открыть в OneDrive и Поделиться для вложений":::

|Выберите...|Кому...|Дополнительные сведения...|
|---------|-----|----------------|
|Открыть в OneDrive|Копировать файл в папку Business Central в вашем OneDrive и открыть файл.|[Открыть в OneDrive](across-share-onedrive.md#open-in-onedrive) |
|Доля|Скопируйте файл к себе в OneDrive и поделитесь с другими людьми.|[Поделиться в OneDrive](across-share-onedrive.md#share) |

<!--
When you use the **Open in OneDrive** action for the first time, [!INCLUDE[prod_short](includes/prod_short.md)] does the following in your OneDrive:

1. Creates a folder named [!INCLUDE[prod_short](includes/prod_short.md)]. 
2. In the [!INCLUDE[prod_short](includes/prod_short.md)] folder, it creates another folder with the same name as the company you're working in. If you work in more than one company, it will create a folder for the company you're working in when you use the **Open in OneDrive** action. 
3. Puts a copy of the file you selected in the folder, and then opens the file. The next time you use the action, it only copies and opens the file. 

The folder and its content are private until you decide to share them with others. For example, you might decide to share content with one or more of your coworkers, or even people outside of your organization. For more information, see [Share OneDrive files and folders](https://support.microsoft.com/en-us/office/share-onedrive-files-and-folders-9fcc2f7d-de0c-4cec-93b0-a82024800c07).
-->

> [!NOTE]
> Вы также можете подключить свою локальную версию [!INCLUDE[prod_short](includes/prod_short.md)] к OneDrive. Однако есть несколько кое-что, что нужно сделать, чтобы заставить это работать. Дополнительные сведения см. в разделе [Настройка локальной версии Business Central](admin-onedrive-integration.md#configuring-business-central-on-premises).

## <a name="see-also"></a>См. также
[Управление интеграцией OneDrive с Business Central](admin-onedrive-integration.md)  
[Открытие файлов Business Central в OneDrive](across-share-onedrive.md)  
[Часто задаваемые вопросы по OneDrive](admin-onedrive-faq.md)