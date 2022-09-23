---
title: Поиск записей
description: В этой статье описывается, как работать с документами и записями, которые связаны
author: jswymer
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: find
ms.search.form: 344
ms.date: 05/23/2022
ms.author: jswymer
ms.openlocfilehash: 3c89d9f3044a8fd0d0fa7f811f1b2f01978e4302
ms.sourcegitcommit: 3acadf94fa34ca57fc137cb2296e644fbabc1a60
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/19/2022
ms.locfileid: "9532381"
---
# <a name="finding-related-entries-for-posted-documents"></a>Поиск связанных записей для учтенных документов 

В этой статье вы узнаете, как найти документы и записи, связанные друг с другом, на основе общей информации, например:

- Номер документа или дата проводки
- Тип делового контакта, номер или номер внешнего документа
- Серийный номер товара или номер партии

Эта функция полезна для поиска операций книги, которые стали результатом определенных транзакций. При поиске по номеру документа можно также распечатывать сводку из отчета "Операции с документами".

## <a name="get-started"></a>Начать

Функция поиска записей легко доступна практически с любой страницы нажатием клавиш Ctrl+Alt+Q. Со страниц, специально отображающих учтенные документы или записи учтенных документов &mdash; как для списков, так и для карт &mdash; вы также можете открыть эту функцию, выбрав действие **Найти записи**.

На странице **Найти записи** включает все связанные документы и операции на основе номера документа и даты учета. Страница разделена на три раздела:

- В верхнем разделе отображаются поля и действия, которые вы используете для фильтрации поиска.
- В среднем разделе отображаются связанные документы на основе результатов поиска.
- В нижнем разделе отображается информация об исходном документе, найденном при поиске.


<!--
 There are two ways to open this page:

- Choose the ![Lightbulb that opens the Tell Me feature.](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Find Entries**, and then choose the related link.

    With this way, the **Find Entries** page might be empty, and you'll have to start searching for entries from scratch.
    
- Open a page that displays posted documents or posted documents entries, either a list or a card. Then, locate and select the **Find Entries** action.

    With this way, the **Find Entries**, page will include all related documents and entries based on the document no. and posting date.


    > [!TIP]
    > If you are on a page that has the **Find Entries** action, press crtl+G to open the **Find Entries** page directly. 
-->

## <a name="search-for-entries"></a>Искать операции

Вы можете искать операции на основе информации о документе, деловом контакте или товаре. Чтобы изменить поиск, выберите **Действия**, **Найти по**, затем одно из следующих действий:

|Действие|Описание|
|------|-----------|
|Найти по документу|Просмотр операций на основе определенного номера документа или даты публикации.|
|Бизнес-контакт |Просматривайте записи на основе определенного типа контакта, контактного номера, и/или внешнего номера документа. Можно ввести информацию о документе, назначенную поставщиком или клиентом. Используйте доступные поля для поиска документов поставщика с использованием номеров, которые поставщик присвоил документам.|
|Ссылка на товар|Просмотр записей по серийному номеру или номеру партии. Можно ввести номер партии или серийный номер либо отфильтровать по номеру партии или серийному номеру, по которым необходимо выполнить поиск. Это действие используется, чтобы увидеть, где использовался конкретный номер трассировки товаров, от какого поставщика он получен или какому клиенту продан.|

После того, как вы сделаете выбор, введите релевантную поисковую информацию в поля вверху. Используйте всплывающие подсказки на полях. Когда вы закончите, выберите **Найти**, чтобы начать поиск. Если изменить любые фильтры, следует снова выбрать **Найти**.

> [!TIP]
> Несколько примеров использования **Найти записи**, см. [Отслеживание отслеживаемых предметов](inventory-how-to-trace-item-tracked-items.md) <!--and [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md). -->

## <a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/user-interface-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Работа с Business Central](ui-work-product.md)  
[Добавление действия страницы в ролевой центр](ui-bookmarks.md)  
[Трассировка товаров, трассируемых по товарам](inventory-how-to-trace-item-tracked-items.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
