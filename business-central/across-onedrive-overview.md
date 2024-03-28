---
title: Business Central и OneDrive для бизнес-интеграции
description: 'Вы можете использовать OneDrive для бизнеса для хранения, управления и обмена файлами, например отчетами или вложенными файлами. Также, если писать One Drive.'
author: jswymer
ms.topic: overview
ms.search.keywords: null
ms.date: 02/28/2022
ms.author: jswymer
ms.service: dynamics-365-business-central
---

# <a name="business-central-and-onedrive-for-business-integration"></a>Business Central и OneDrive для бизнес-интеграции

OneDrive для бизнеса — это облачная служба хранения, входящая в состав Microsoft 365. [!INCLUDE[prod_short](includes/prod_short.md)] позволяет легко хранить, управлять и делиться файлами с другими людьми через OneDrive. Когда файл находится в вашем OneDrive, вы можете пользоваться разнообразными возможностями совместной работы с помощью онлайн-версий продуктов Майкрософт, таких как Word, Excel и PowerPoint. Например, вы можете поделиться документом Word, а затем вы и ваши коллеги сможете редактировать его вместе в режиме реального времени. OneDrive также позволяет открывать другие типы файлов, например PDF-файлы. 

## <a name="get-started-with-onedrive-features"></a>Начало работы с функциями OneDrive

Если вы используете [!INCLUDE[prod_short](includes/prod_short.md)] Online, мы уже создали подключение между [!INCLUDE[prod_short](includes/prod_short.md)] Online и OneDrive, поэтому начать использовать функции OneDrive можно без каких-либо усилий. Единственное требование — чтобы пользователи открыли OneDrive по крайней мере один раз. В случае локальной версии [!INCLUDE[prod_short](includes/prod_short.md)] для начала использования этих функций администратор должен настроить подключение. Подробее см. в статье [Управление интеграцией OneDrive с Business Central](admin-onedrive-integration.md).

<!-- We've created the connection between [!INCLUDE[prod_short](includes/prod_short.md)] online and OneDrive, so it's easy to get started. The only requirement is that users have opened OneDrive at least one time. -->

### <a name="open-and-share-in-onedrive"></a>Действия "Открыть в OneDrive" и "Поделиться"

На большинстве страниц, где доступны файлы, например в папке входящих отчетов или в файлах, прикрепленных к записям, вы найдете действие **Открыть в OneDrive** и **Поделиться**.

:::image type="content" source="media/onedrive-overview-report-inbox-w-outline.png" alt-text="Действия Открыть в OneDrive и Поделиться для отчетов":::


:::image type="content" source="media/one-drive-attachments-w-outline.png" alt-text="Действия Открыть в OneDrive и Поделиться для вложений":::

|Выберите...|Кому...|Дополнительные сведения...|
|---------|-----|----------------|
|Открыть в OneDrive|Копировать файл в папку Business Central в вашем OneDrive и открыть файл.|[Открыть в OneDrive](across-share-onedrive.md#open-in-onedrive) |
|Доля|Скопируйте файл к себе в OneDrive и поделитесь с другими людьми.|[Поделиться в OneDrive](across-share-onedrive.md#share) |

### <a name="save-excel-workbooks-and-report-files-in-onedrive"></a>Сохранение книг Excel и файлов отчетов в OneDrive

После настройки интеграции с OneDrive некоторые другие знакомые функции будут автоматически использовать для сохранения файлов OneDrive вместо сохранения файлов на вашем устройстве:

- Действия **Открыть в Excel** и **Изменить в Excel** на страницах списков будут автоматически копировать файл Excel в OneDrive, а затем открывать его в Excel Online. Для получения дополнительной информации см. статью [Просмотр и редактирование в Excel](across-work-with-excel.md).
- При отправке отчета в файл Excel или Word он автоматически копируется в OneDrive, затем открывается в Excel Online или Word Online. Дополнительные сведения см. в статье [Сохранение отчета в файл](ui-work-report.md#saving-a-report-to-a-file).

Эти функции не включены по умолчанию. Но как администратор вы можете легко включить их с помощью мастера настройки **Настройка OneDrive**.

<!--
When you use the **Open in OneDrive** action for the first time, [!INCLUDE[prod_short](includes/prod_short.md)] does the following in your OneDrive:

1. Creates a folder named [!INCLUDE[prod_short](includes/prod_short.md)]. 
2. In the [!INCLUDE[prod_short](includes/prod_short.md)] folder, it creates another folder with the same name as the company you're working in. If you work in more than one company, it will create a folder for the company you're working in when you use the **Open in OneDrive** action. 
3. Puts a copy of the file you selected in the folder, and then opens the file. The next time you use the action, it only copies and opens the file. 

The folder and its content are private until you decide to share them with others. For example, you might decide to share content with one or more of your coworkers, or even people outside of your organization. For more information, see [Share OneDrive files and folders](https://support.microsoft.com/office/share-onedrive-files-and-folders-9fcc2f7d-de0c-4cec-93b0-a82024800c07) in the content for OneDrive.
-->

> [!NOTE]
> Вы также можете подключить свою локальную версию [!INCLUDE[prod_short](includes/prod_short.md)] к OneDrive. Однако есть несколько кое-что, что нужно сделать, чтобы заставить это работать. Дополнительные сведения см. в разделе [Настройка локальной версии Business Central](admin-onedrive-integration-onpremises.md).

## <a name="see-also"></a>См. также

[Управление интеграцией OneDrive с Business Central](admin-onedrive-integration.md)  
[Открытие файлов Business Central в OneDrive](across-share-onedrive.md)  
[Часто задаваемые вопросы по OneDrive](admin-onedrive-faq.md)  
