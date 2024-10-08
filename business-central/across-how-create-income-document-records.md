---
title: Создание записей входящих документов
description: 'Используйте различные функции на странице "Входящие документы", чтобы просматривать квитанции о расходах, управлять задачами распознавания текста, конвертировать файлы входящих документов и прикреплять внешние файлы.'
author: jswymer
ms.topic: how-to
ms-service: dynamics-365-business-central
ms.search.keywords: 'electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice'
ms.date: 02/27/2024
ms.author: jswymer
ms.custom: bap-template
ms.reviewer: jswymer
ms.service: dynamics-365-business-central
---
# <a name="create-incoming-document-records"></a>Создание записей входящих документов

На странице **Входящие документы** можно использовать различные функции для просмотра квитанций по расходам, управления задачами OCR, а также преобразования входящих файлов документов, вручную и автоматически, в соответствующие документы либо строки журналов. Внешние файлы можно прикреплять на любом этапе обработки, в том числе к учтенным документам и к полученным записям поставщика, клиента и главной книги.

Чтобы зарегистрировать внешний документ в [!INCLUDE[prod_short](includes/prod_short.md)], сначала создайте или завершите запись входящего документа. Эти задачи можно выполнить вручную или можно сфотографировать внешний документ, чтобы создать запись входящего документа с вложенным файлом изображения.

Перед использованием функции **Входящие документы** необходимо выполнить обязательную настройку. Дополнительные сведения см. в разделе [Настройка входящих документов](across-how-setup-income-documents.md).

## <a name="approve-or-reject-an-incoming-document"></a>Утверждение или отклонение входящего документа

Если вы настроили функцию **Входящие документы**, чтобы требовать утверждения для создания документов, пользователи с соответствующими правами должны утвердить записи перед их обработкой. Дополнительные сведения см. в разделе [Настройка утверждающих для записей входящих документов](across-how-setup-income-documents.md#to-set-up-approvers-of-incoming-document-records).

1. Выберите ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать") значок, введите **Входящие документы**, а затем выберите связанную ссылку.
2. Выберите строку с документом, который необходимо утвердить или отклонить, а затем выберите действие **Утвердить** или **Отклонить**.

При утверждении записи входящего документа в строке этого документа устанавливается флажок **Выпущено**. Например, пользователь, который отвечает за создание счетов на покупку, может перейти к обработке записи.

## <a name="create-an-incoming-document-record-by-taking-a-photo"></a>Создание записи входящего документа путем съемки фото

> [!NOTE]  
> Следующая процедура применяется только к клиентам [!INCLUDE[prod_short](includes/prod_short.md)] для планшетов и телефонов.

1. В центре ролей выберите плитку **Создать входящий документ по данным камеры**, а затем перейдите к шагу 4.
2. Или выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Входящие документы**, затем выберите связанную ссылку.
3. На странице **Входящие документы** выберите **Создать**, затем выберите **Создать из камеры**. Камера планшета или телефона включится.
4. Сделайте фотографию документа, например приходной накладной, которую требуется обработать как входящий документ, затем нажмите кнопку **Использовать**.

    Создается новая запись входящего документа с прикрепленным изображением.

## <a name="attach-an-image-to-an-incoming-document-record-by-taking-a-photo"></a>Прикрепление изображения к записи входящего документа путем съемки фото

> [!NOTE]  
> Следующая процедура применяется только к клиентам [!INCLUDE[prod_short](includes/prod_short.md)] для планшетов и телефонов.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Входящие документы**, затем выберите связанную ссылку.
2. Откройте карточку для существующей записи входящего документа.
3. На странице записи документа выберите **Обработать**, затем выберите **Прикрепить изображение с камеры**. Камера планшета или телефона включится.
4. Сделайте фотографию документа, например приходной накладной, которую требуется обработать как входящий документ, затем нажмите кнопку **Использовать**.

    Изображение прикрепляется к записи входящего документа.

## <a name="create-an-incoming-document-record-manually"></a>Создание записи входящего документа вручную

1. Выберите значок ![Лампочка, которая открывает функцию «Что вы хотите сделать»](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Входящие документы**, затем выберите связанную ссылку.
2. Выберите **Создать**, затем выберите действие **Создать из файла**.  
3. На странице **Вставка файла** выполните одно из следующих действий, чтобы прикрепить файл, представляющий входящий документ:

   [!INCLUDE[file-upload](includes/file-upload.md)]

4. Также можно выбрать действие **Создать**, а затем выполнить следующие действия:

    1. Чтобы вложить файл, выберите **Обработка** > **Вложить файл**.
    2. На странице **Вставка файла** перетащите выбранный файл, представляющий соответствующий входящий документ, или выберите **щелкните здесь, чтобы выбрать файл**.
    3. На странице **Входящий документ** заполните поля по мере необходимости. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="see-also"></a>См. также

[Использование OCR для преобразования PDF-файлов и файлов изображений в электронные документы](across-how-use-ocr-pdf-images-files.md)
[Создание записей входящих документов непосредственно из документов и операций](across-how-connect-disconnect-income-document-records.md)
[Поиск учтенных документов без записей входящих документов](across-how-find-posted-documents-without-income-document-records.md)
[Входящие документы](across-income-documents.md)  
[Покупки](purchasing-manage-purchasing.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
