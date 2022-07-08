---
title: Создание и изменение пользовательских макетов для отчетов и документов
description: Узнайте, как создать пользовательские макеты, с помощью которых можно персонализировать внешний вид отчета при его просмотре, печати или сохранении.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.search.form: 9650, 9652
ms.date: 03/06/2022
ms.author: edupont
ms.openlocfilehash: 81073838cc6bfd1858a3b3d18cd554b62080704a
ms.sourcegitcommit: 00a8acc82cdc90e0d0db9d1a4f98a908944fd50a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "9075347"
---
# <a name="legacy-create-and-modify-custom-report-layouts"></a>(Устарело) Создание и изменение пользовательских макетов отчетов

[!INCLUDE[legacy-custom-layouts](includes/legacy-custom-layouts.md)]

По умолчанию отчеты имеют встроенный макет отчета. Макет может быть макетом отчета RDLC, макетом отчета Word или обоими типами макетов. Вы не можете изменять встроенные макеты, но можете создавать собственные макеты. Отчет может иметь несколько пользовательских макетов отчетов.

> [!NOTE]  
> В [!INCLUDE[prod_short](includes/prod_short.md)] термин "отчет" также означает внешние документы, такие как счета продажи и подтверждения заказов, которые вы отправляете клиентам в виде PDF-файлов.

Чтобы создать пользовательский макет, либо скопируйте существующий пользовательский макет, либо добавьте новый пользовательский макет. Пользовательские макеты часто основаны на встроенном макете. При добавлении нового пользовательского макета можно добавить тип макета отчета RDLC или Word, или оба типа. Новый пользовательский макет основывается на встроенном макете отчета при его наличии. Если для типа нет встроенного макета, создается новый пустой макет. Вам придется изменить и разработать этот пустой макет с нуля. Дополнительные сведения о макетах отчетов RDLC и Word, встроенных и пользовательских макетах и др. см. в разделе [Управление макетами отчетов](ui-manage-report-layouts.md).  

> [!TIP]
> Используйте финансовые отчеты для получения сведений о финансовых данных, сохраненных в плане счетов. Дополнительные сведения см. в разделе [Подготовка финансовой отчетности с помощью финансовых отчетов и категорий счетов](bi-how-work-account-schedule.md).

После определения пользовательских макетов отчетов их можно выбрать на страницах карточки клиента и карточки поставщика. Макеты будут использоваться при создании документов для этого клиента или поставщика. Для получения дополнительной информации см. [Определение макетов документов для клиентов и поставщиков](ui-define-customer-vendor-document-layouts.md).

Вы можете также использовать пользовательские макеты отчетов для добавления содержимого в сообщения электронной почты. Макеты отчетов могут сэкономить время и помочь обеспечить согласованность за счет повторного использования одного и того же содержимого при общении с клиентами. Чтобы использовать пользовательские макеты отчетов с сообщениями электронной почты, тип файла макета должен быть Word. Вы не можете использовать тип файлов RDLC. Для получения дополнительной информации см. раздел [Настройка повторно используемых текстов и макетов сообщений электронной почты](admin-how-setup-email.md#set-up-reusable-email-texts-and-layouts). 

## <a name="to-create-a-custom-layout"></a>Создание пользовательского макета

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Выбор макета отчета**, а затем выберите связанную ссылку.

    На странице **Выбор макета отчета** перечислены все доступные отчеты для организации, которая указана в поле **Название организации** в верхней части страницы.
2. В поле **Название организации** выберите организацию, для которой требуется создать макет отчета.
3. Выберите строку отчета, для которого требуется создать макет, а затем выберите действие **Пользовательские макеты**.  

   Будет открыта страница **Пользовательские макеты отчетов**, содержащая все пользовательские макеты, доступные для выбранного отчета.
4. Если требуется создать копию существующего пользовательского макета, выберите существующий пользовательский макет в списке, затем выберите действие **Копировать**.  

   Копия пользовательского макета появится на странице **Пользовательские макеты отчетов**, и в поле *Описание* будет содержать слово **Копия**.
5. Если требуется добавить новый пользовательский макет, основанный на встроенном макете, выполните следующие шаги:  
   1. Выберите действие **Создать**. Появится страница **Вставить встроенный макет для отчета**. Поля **Код** и **Название** заполняются автоматически.
   2. Чтобы добавить тип пользовательского макета отчета Word, включите выключатель **Вставить макет Word**.
   3. Чтобы добавить тип пользовательского макета отчета RDLC, включите выключатель **Вставить макет RDLC**.
   4. Нажмите кнопку **ОК**.  

    Новый пользовательский макет появится на странице **Пользовательские макеты отчетов**. Если новый макет основан на встроенном макете, он содержит текст **Копия встроенного макета** в поле **Описание**. Если у отчета нет встроенного макета, то новый макет содержит текст **Новый макет** в поле **Описание**, что означает, что пользовательский макет не заполнен.
6. По умолчанию поле **Название организации** не заполнено, это означает, что пользовательский макет будет доступен для отчета во всех организациях. Чтобы сделать пользовательский макет доступным только для определенной организации, выберите **Правка**, а затем в поле **Название организации** добавьте требуемую организацию.

Пользовательский макет создан. Теперь пользовательский макет можно изменять при необходимости.

> [!TIP]
> Вы можете экспортировать результаты отчета в файл Excel для просмотра полного набора данных, включая все столбцы, но без макета. Файл Excel может помочь вам убедиться, что отчет возвращает ожидаемые данные, или найти проблему. Для получения дополнительной информации см. [Анализ данных отчета с помощью Excel](report-analyze-excel.md).

## <a name="modifying-a-custom-layout"></a><a name="ModifyCustomLayout"></a>Изменение пользовательского макета

Чтобы изменить макет отчета, вы должны сначала экспортировать макет отчета в виде файла на свой компьютер или в сеть. Затем откройте экспортированный документ и внесите изменения. По завершении внесения изменений необходимо импортировать макет отчета.

### <a name="to-modify-a-custom-layout"></a>Изменение пользовательского макета

1. Экспорт пользовательского макета производится со страницы **Пользовательские макеты отчетов**. Если эта страница еще не открыта, выполните поиск и откройте страницу **Выбор макета отчета**, выберите отчет, содержащий макет, который вы хотите изменить, затем выберите действие **Пользовательские макеты**.  
2. На странице **Пользовательские макеты отчетов** выберите макет, который требуется изменить, выберите действие **Экспортировать макет**, затем выберите **Сохранить** или **Сохранить как**, чтобы сохранить документ макета отчета в папке компьютера или в сети.  
3. Откройте сохраненный документ макета отчета и внесите изменения.

   Если вы изменяете макет Word, откройте документ макета в Word. Подробности редактирования см. в [Работа с макетами Word](ui-how-add-fields-word-report-layout.md)<!--the next section [Making Changes to the Report Layout](ui-how-create-custom-report-layout.md#MakeChangesToLayout)-->.

   Макеты отчета RDLC обеспечивают больше возможностей, чем макеты отчета Word. Дополнительные сведения об изменении макета отчета RDLC см. в разделе [Разработка макетов отчетов RDLC](/dynamics-nav/Designing-RDLC-Report-Layouts).

   По завершении обязательно сохраните изменения.

4. Вернитесь на страницу **Пользовательские макеты отчетов**, выберите макет отчета, который вы экспортировали и изменили, затем выберите действие **Импортировать макет**.  

5. В диалоговом окне **Импорт** выберите **Выбрать**, чтобы найти и выбрать измененный документ макета отчета, затем выберите **Открыть**.

> [!IMPORTANT]
> Не забудьте импортировать измененный документ макета отчета. В противном случае новый макет отчета будет недоступен.

<!--
##  <a name="MakeChangesToLayout"></a> Create and Modify Custom Report Layouts

To make general formatting and layout changes, such as changing text font, adding and modifying a table, or removing a data field, just use the basic editing features of Word, like you do with any Word document.

If you're designing a Word report layout from scratch or adding new data fields, then start by adding a table that includes rows and columns that will eventually hold the data fields.

> [!TIP]  
> Show the table gridlines so that you see the boundaries of table cells. Remember to hide the gridlines when you're done editing. To show or hide table gridlines, select the table, and then under **Layout** on the **Table** tab, choose **View Gridlines**.

### Embedding Fonts in Word Layouts for Consistency

To ensure that reports always display and print with the intended fonts, wherever users open or print the reports, you can embed the fonts in the Word document. However, embedding fonts can significantly increase the size of the Word files. For more information about embedding fonts in Word, see [Embed fonts in Word, PowerPoint, or Excel](https://support.office.com/article/Embed-fonts-in-Word-PowerPoint-or-Excel-cb3982aa-ea76-4323-b008-86670f222dbc).

###  <a name="RemoveField"></a> Removing Label and Data Fields in Word Layouts

 Label and data fields of a report are contained in content controls in Word. The following figure illustrates a content control when it's selected in the Word document.  

 ![Content control for field in Word report layout.](media/nav_wordreportlayouts_contentcontrol.png "NAV_WordReportLayouts_ContentControl")  

 The name of the label or data field name displays in the content control. In the example, the field name is CompanyAddr1.  

### To remove a label or data field  

1. Right-click the field that you want to delete, and then choose **Remove Content Control**.  

     The content control is removed, but the field name remains as text.  

2. Delete the remaining text as needed.  

### Adding data fields

Adding data fields from a report dataset is a more advanced and requires some knowledge of the report dataset. For information about adding fields for data, labels, data, and images, see [Add Fields to a Word Report Layout](ui-how-add-fields-word-report-layout.md).  -->

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/change-documents-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Управление макетами отчетов](ui-manage-report-layouts.md)  
[Смена текущего макета отчета](ui-how-change-layout-currently-used-report.md)  
[Импорт и экспорт пользовательского макета отчета или документа](ui-how-import-and-export-report-layout.md)  
[Работа с отчетами, пакетными заданиями и XMLport](ui-work-report.md)  
[Подготовка финансовой отчетности с помощью финансовых отчетов и категорий счетов](bi-how-work-account-schedule.md)  
[Бизнес-аналитика](bi.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]