---
title: Обмен данными
description: 'Обменивайтесь электронными деловыми документами, например банковскими файлами, между Business Central и внешними сторонами.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'exchange data, external files, electronic documents, AMC Banking, OCT, SEPA'
ms.date: 06/10/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="exchanging-data"></a>Обмен данными
Доступен обмен данными между [!INCLUDE[prod_short](includes/prod_short.md)] и внешними файлами или потоками в связи с выполнением бизнес-задач общего характера, таких как отправка и получение электронных документов и импорт или экспорт банковских файлов.  

Прежде чем отправлять и получать электронные документы и импортировать или экспортировать банковские файлы, необходимо настроить платформу обмена данными для обработки файлов или потоков данных. Кроме того, вы должны настроить связанные области, такие как клиенты, которым вы отправляете электронные счета, и расширение AMC Banking 365 Fundamentals, если вы распространяете преобразования банковских файлов для внешних поставщиков услуг. Дополнительные сведения см. в разделе [Настройка обмена данными](across-set-up-data-exchange.md).  

 В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.  

|**Чтобы**|**Смотрите**|  
|------------|-------------|  
|Преобразование записей документов о продажах в [!INCLUDE[prod_short](includes/prod_short.md)] в стандартизированный формат и отправка их в виде электронных документов, пригодных для получения системами клиентов.|[Отправка электронных документов](sales-how-to-send-electronic-documents.md)|  
|Отправьте PDF-файл или графический файл поставщику служб OCR и получите его обратно в виде электронного документа, который может быть преобразован в записи документа в [!INCLUDE[prod_short](includes/prod_short.md)].|[Использование OCR для преобразования PDF-файлов и файлов изображений в электронные документы](across-how-use-ocr-pdf-images-files.md)|  
|Получение электронных документов из службы OCR или службы обмена документами в едином формате, который преобразуется в соответствующие записи документов в [!INCLUDE[prod_short](includes/prod_short.md)].|[Получение и преобразование электронных документов](purchasing-how-to-receive-and-convert-electronic-documents.md)|  
|Подготовьтесь к импорту файла банковской выписки на страницу **Журнал выверки платежей** в качестве первого шага выверки платежей или страницу **Выверка банковского счета** в качестве первого шага выверки банковских счетов.|[Настройка службы Envestnet Yodlee Bank Feeds](bank-how-setup-bank-statement-service.md)|  
|Экспортируйте платежи со страницы **Журнал платежей** в файл банка, загружаемый в электронный банковский счет для обработки.|[Экспорт платежей в банковский файл](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md#exporting-payments-to-a-bank-file)|
|Выполнение электронных платежей согласно стандарту кредитового перевода SEPA в ЕС.|[Выполнение платежей с помощью расширения AMC Banking 365 Fundamentals или кредитного перевода SEPA](finance-make-payments-with-bank-data-conversion-service-or-sepa-credit-transfer.md)|  
|Проинструктируйте банк, чтобы он переводил суммы платежей из банковских счетов ваших клиентов на счет вашей организации в соответствии с настройкой прямого дебета SEPA.|[Создание операций погашения прямого дебета SEPA и их экспорт в файл банка](finance-collect-payments-with-sepa-direct-debit.md#creating-sepa-direct-debit-collection-entries-and-export-to-a-bank-file)|  
|Для обновления страницы **Валюты** воспользуйтесь поставщиком службы для курсов валют.|[Обновление валютных курсов](finance-how-update-currencies.md)|  
|Просмотрите, какие элементы файлов сопоставляются с полями [!INCLUDE[prod_short](includes/prod_short.md)] при импорте файлов выписок SEPA CAMT.|[Сопоставление полей при импорте файлов SEPA CAMT](across-field-mapping-when-importing-sepa-camt-files.md)|  
|Экспорт данных для отчетности Интрастат в [!INCLUDE[prod_short](includes/prod_short.md)].|[Настройка отчетности Интрастат](finance-how-setup-report-intrastat.md)|
|Просмотрите, какие поля [!INCLUDE[prod_short](includes/prod_short.md)] сопоставляются с элементами файла при экспорте файлов платежей с помощью расширения AMC Banking 365 Fundamentals.|[Сопоставление полей при экспорте файлов платежей с использованием расширения AMC Banking 365 Fundamentals](across-field-mapping-when-exporting-payment-files-using-bank-data-conversion-service.md)|  

## <a name="see-also"></a>См. также
[Настройка обмена данными](across-set-up-data-exchange.md)  
[Электронный обмен данными](across-data-exchange.md)  
[Выставление счетов продажи](sales-how-invoice-sales.md)   
[Регистрация покупок](purchasing-how-record-purchases.md)  
[Входящие документы](across-income-documents.md)  
[Общие бизнес-функции](ui-across-business-areas.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
