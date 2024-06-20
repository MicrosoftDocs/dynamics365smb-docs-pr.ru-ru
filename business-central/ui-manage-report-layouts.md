---
title: Управление макетами отчетов и документов
description: 'Макеты отчетов служат для персонализации документов, например для настройки шрифтов, логотипов и параметров страниц PDF-файлов, которые вы отправляете клиентам.'
author: jswymer
ms.topic: conceptual
ms.search.keywords: 'customized report, document layout, logo, personalize'
ms.search.form: '9652, 9650, 9660'
ms.date: 01/18/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---
# Обзор макетов отчетов и документов

Макет отчета контролирует содержимое и формат отчета, включая то, какие поля данных набора данных отчета отображаются в нем и как они упорядочены, а также стиль текста, изображения и т. д. В [!INCLUDE[prod_short](includes/prod_short.md)] можно изменить используемый в отчете макет, создать новый макет или изменить текущие макеты.

> [!NOTE]  
> В [!INCLUDE[prod_short](includes/prod_short.md)] термин "отчет" также означает внешние документы, такие как счета продажи и подтверждения заказов, которые вы отправляете клиентам в виде PDF-файлов.

Вы можете также использовать макеты отчетов для добавления содержимого в сообщения электронной почты. Например, макеты отчетов могут сэкономить время и помочь обеспечить согласованность за счет повторного использования одного и того же содержимого при общении с клиентами. Чтобы использовать пользовательские макеты отчетов с сообщениями электронной почты, тип файла макета должен быть Word. Вы не можете использовать тип файлов RDLC. Для получения дополнительной информации см. раздел [Настройка повторно используемых текстов и макетов сообщений электронной почты](admin-how-setup-email.md#set-up-reusable-email-texts-and-layouts). 

## Введение

В частности, макет отчета настраивает следующее:

* Поля меток и данных для включения из набора данных отчета [!INCLUDE[prod_short](includes/prod_short.md)].
* Текстовый формат, например тип, размер и цвет шрифта.
* Логотип компании и его расположение.
* Общие параметры страницы, такие как поля и фоновые изображения.

Отчет можно настроить с несколькими макетами, между которыми можно при необходимости переключаться. 

<!--You can use one of the built-in report layouts or you can create custom report layouts and assign them to your reports as needed. For more information, see [Create a Custom Report or Document Layout](ui-how-create-custom-report-layout.md).-->

Есть два важных аспекта макетов отчетов, которые будут влиять на то, как вы с ними работаете: *тип макета* и *источник макета*. Тип макета указывает тип файла, на котором основан макет. Источник макета указывает источник макета.

## Типы макета

Существует четыре типа макетов отчета, которые можно использовать в отчетах — Word, RDLC, Excel и внешний.

### Word

Макеты Word основаны на документах Word (тип файла DOCX). Макеты Word позволяют разрабатывать макеты отчетов с помощью Microsoft Word. Макет Word определяет содержимое отчета, расположение элементов отчета и их внешний вид. Документ макета Word, как правило, использует таблицы для организации содержимого, клетки которых могут содержать поля данных, текст или изображения.

[![Пример макета отчета Word для Business Central.](media/word-layout-overview.png)](media/word-layout-overview.png#lightbox) 

<!--![Example of a word report layout document for Business Central.](media/nav_wordreportlayout_edit_in_word_example.png) -->

Дополнительные сведения см. в разделе [Работа с макетами Word](ui-how-add-fields-word-report-layout.md).

### Excel

Макеты Excel основаны на книгах Microsoft Excel (тип файлов XLSX). Они позволяют создавать отчеты с использованием знакомых функций Excel для обобщения, анализа и представления данных с помощью таких средств, таких как формулы, сводные таблицы и сводные диаграммы и других.

[![Показывает пример макета Excel.](media/excel-layout-2.png)](media/excel-layout-2.png#lightbox)

Дополнительные сведения см. в разделе [Работа с макетами Excel](ui-excel-report-layouts.md).

### RDLC

Макеты RDLC основаны на клиентских макетах определения отчета (типы файла RDL или RDLC). Эти макеты создаются и изменяются с помощью SQL Server Report Builder или Microsoft RDLC Report Designer. Концепция дизайна для макетов RDLC аналогична макетам Word, где макет определяет, какие поля отображать и как они расположены. Однако разработка макетов RDLC более сложная, чем макетов Word.

[![Показывает пример макета RDLC.](media/rdlc-layout-overview.png)](media/rdlc-layout-overview.png#lightbox)

Дополнительные сведения см. в разделе [Работа с макетами RDLC](ui-rdlc-report-layouts.md).

### Внешнее

Тип внешнего макета относится к расширенному типу, специально разработанному для определенных отчетов. Сами отчеты и макеты обычно предоставляются партнерами, а не корпорацией Майкрософт. Фактический тип файла макета зависит от поставщика.

Для получения дополнительной информации см. [Построение пользовательского отчета](/dynamics365/business-central/dev-itpro/developer/devenv-report-custom-render).

## Источники макета

В дополнение к типу макеты делятся на три категории в зависимости от их источника или происхождения.

* Макеты расширения

   Макеты расширения — это макеты, которые являются частью расширения, установленного в среде. Эти макеты обычно представляют собой стандартные макеты, предоставляемые Microsoft, например, в базовом приложении. Или это могут быть макеты, включенные в расширения от других поставщиков программного обеспечения. Вы можете распознать макеты расширений на странице **Макеты отчетов**, потому что имя расширения и издатель отображаются в столбце **Расширение**.

* Заданные пользователем макеты

   Другим источником макетов является конечный пользователь. В Business Central пользователь с соответствующими разрешениями может добавлять новые макеты различными способами. Например, вы можете начать с существующего макета расширения или другого заданного пользователем макета. На странице **Макеты отчетов** заданный пользователем макет будет иметь пустой столбец **Расширение**.

   Для получения дополнительной информации см. [Приступайте к созданию макетов отчетов](ui-get-started-layouts.md).

* Пользовательские макеты

  Пользовательские макеты — это также макеты, созданные пользователями. Разница в том, что эти макеты созданы на устаревшей странице **Пользовательские макеты отчетов**, и они могут быть только типа Word и RDLC. Хотя вы по-прежнему можете создавать пользовательские макеты, они постепенно уступают место определенным пользователем макетам (см. выше).

  Дополнительные сведения см. в разделе [(Устарело) Создание и изменение пользовательских макетов отчетов](ui-how-create-custom-report-layout.md).

Для получения информации, которая поможет вам решить, какой тип лучше всего подходит для вас, см. [Решите, какой тип макета вам нужен](ui-get-started-layouts.md#decide).

> [!IMPORTANT]
> Важно помнить, что вы не можете изменять макеты расширений в клиенте Business Central. Например, вам не разрешено изменять имя или тип макета, а также загружать и заменять его другой версией. Если вы попытаетесь это сделать, появится сообщение об ошибке. Вместо этого вам придется создать заданный пользователем или пользовательский макет на основе макета расширения.

<!--
### Built-in and custom report layouts



[!INCLUDE[prod_short](includes/prod_short.md)] includes several built-in layouts. Built-in layouts are predefined layouts that are designed for specific reports. [!INCLUDE[prod_short](includes/prod_short.md)] reports will have a built-in layout as either an RDLC report layout, Word report layout, or in some cases both. You can’t modify a built-in report layout from [!INCLUDE[prod_short](includes/prod_short.md)] but you use them as a starting point for building your own custom report layouts.

Custom layouts are report layouts that you design to change the appearance of a report. You typically create a custom layout based on a built-in layout, but you can create them from scratch or from a copy of an existing custom layout. Custom layouts enable you to have multiple layouts for the same report, which you switch among as needed. For example, you can have different layouts for each [!INCLUDE[prod_short](includes/prod_short.md)] company, or you can have different layouts for the same company for specific occasions or events, like a special campaign or holiday season.


Deciding on whether to use a Word, Excel, or RDLC layout type will depend on how you want the generated report to look and your knowledge of tools for creating the layouts, like Word, Excel, and SQL Server Report Builder.

* The general design concepts for Word and RDLC layouts are similar. However each type has certain design features that affect how the generated report appears in [!INCLUDE[prod_short](includes/prod_short.md)]. This means that the same report might look different when using the Word report layout compared to the RDLC report layout.

* The process for setting up Word, Excel, and RDLC report layouts on reports is the same. The main difference is in the way you modify the layouts. Word and especially Excel layouts are typically easier to create and modify than RDLC report layouts because you use Word and Excel. RDLC report layouts are modified by using SQL Server Report builder, which targets more advanced users.

* Not all reports and document have a dataset that is optimized for use with an Excel layout. For example, aggregations and complex calculations work best with RDLC or Word layouts. The same is true for documents.

For information about how to switch the layout currently used on a report, see [Set the Layout Used by a Report](ui-set-report-layout.md).

-->
## См. также

[Обновление пользовательских макетов отчетов](ui-update-report-layouts.md)  
[Создание и изменение пользовательских макетов отчетов](ui-how-create-custom-report-layout.md)  
[Импорт и экспорт пользовательского макета отчета или документа](ui-how-import-and-export-report-layout.md)  
[Определение специальных макетов документов для клиентов и поставщиков](ui-define-customer-vendor-document-layouts.md)  
[Отправка документов по электронной почте](ui-how-send-documents-email.md)  
[Работа с отчетами, пакетными заданиями и XMLport](ui-work-report.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
