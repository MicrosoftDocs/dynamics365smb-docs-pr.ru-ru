---
title: Создание записей входящих документов из документов
description: Для хранения внешних бизнес-документов следует прикрепить эти файлы документов к связанным записям входящих документов.
author: jswymer
ms.topic: how-to
ms.search.keywords: 'electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice'
ms.date: 02/27/2024
ms.author: jswymer
ms.reviewer: jswymer
ms-service: dynamics-365-business-central
ms.custom: bap-template
ms.service: dynamics-365-business-central
---
# <a name="create-incoming-document-records-directly-from-documents-and-entries"></a>Создание записей входящих документов непосредственно из документов и операций

Для хранения внешних бизнес-документов в [!INCLUDE[prod_short](includes/prod_short.md)] следует прикрепить эти файлы документов к связанным записям входящих документов. Если документ, например счет на покупку, не был изначально создан как запись входящего документа, в любое время сохраняется возможность создать и подключить к нему запись входящего документа. Кроме того, файлы входящих документов можно прикрепить к учтенным документам покупки и продажи, а также к операциям книги поставщиков, покупателей и главной книги, на информационной панели **Файлы входящих документов**, например, на страницах **Учтенные счета покупок** и **Книга операций по поставщикам**.

На страницах **План счетов** и **Операции главной книги** с помощью функции поиска можно найти операции главной книги для учтенных документов покупки и продажи, которые не имеют записей входящих документов, и затем централизованно связать их с существующими записями или создать новые записи с прикрепленными файлами документов. Дополнительные сведения см. в разделе [Поиск учтенных документов без записей входящих документов](across-how-find-posted-documents-without-income-document-records.md).

В перечисленных ниже процедурах показано, как прикрепить файл к записи книги поставщиков или существующему счету на покупку, который не был создан на основе записи входящего документа. Прикрепление файла к учтенным документам продаж или покупок выполняется аналогичным образом.

[!INCLUDE [incoming-doc-archived-doc](includes/incoming-doc-archived-doc.md)]

## <a name="create-and-connect-an-incoming-document-record-from-a-purchase-invoice"></a>Создание записи входящего документа на основе счета на покупку и ее связывание

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок введите **Счета покупки**, а затем выберите связанную ссылку.
2. Выберите строку для счета покупки, к которому требуется прикрепить файл, а затем выберите действие **Создать входящий документ из файла**.
3. Можно также выбрать строку для счета покупки, к которому требуется прикрепить файл, а затем выбрать действие **Прикрепить файл**.
4. На странице **Вставка файла** выполните одно из следующих действий, чтобы прикрепить файл, представляющий соответствующий входящий документ:

   [!INCLUDE[file-upload](includes/file-upload.md)]


## <a name="create-and-connect-an-incoming-document-record-from-a-vendor-ledger-entry"></a>Создание записи входящего документа на основе операции книги поставщиков

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок **Поставщик — книга операций**, а затем выберите связанную ссылку.
2. Выберите строку для операции книги поставщиков, к которой требуется прикрепить файл, а затем выберите действие **Создать входящий документ из файла**.
3. Можно также выбрать строку для операции книги поставщиков, к которой требуется прикрепить файл, а затем выбрать действие **Прикрепить файл**.
4. На странице **Вставка файла** выполните одно из следующих действий, чтобы прикрепить файл, представляющий соответствующий входящий документ:

   [!INCLUDE[file-upload](includes/file-upload.md)]


## <a name="remove-a-connection-from-an-incoming-document-record-to-a-posted-document"></a>Удаление из записи входящего документа связи с учтенным документом

Файловые вложения можно удалить из неучтенных документов в любое время путем удаления связанной записи входящего документа. Если документ учтен, необходимо сначала удалить эту связь из записи входящего документа.

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Входящие документы**, а затем выберите связанную ссылку.
2. Выберите строку для записи входящего документа, связанной с учтенным документом, которые требуется удалить, а затем выберите действие **Удалить ссылку на запись**.

Связь с учтенным документом будет удалена. Теперь можно связать другую запись входящего документа с данным учтенным документом, как описано в этой статье.

## <a name="see-also"></a>См. также

[Создание записей входящих документов](across-how-create-income-document-records.md)
[Использование OCR для преобразования PDF-файлов и файлов изображений в электронные документы](across-how-use-ocr-pdf-images-files.md)
[Поиск учтенных документов без записей входящих документов](across-how-find-posted-documents-without-income-document-records.md)
[Входящие документы](across-income-documents.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
