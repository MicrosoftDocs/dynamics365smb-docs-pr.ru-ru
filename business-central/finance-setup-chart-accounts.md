---
title: Настройка плана счетов (содержит видео)
description: В плане счетов отображаются счета главной книги, на которых хранятся финансовые данные. Можно изменить счета по умолчанию в COA и добавить новые счета.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: COA, cha of acc
ms.search.form: 16, 17, 18, 118, 386, 391
ms.date: 06/22/2021
ms.author: edupont
ms.openlocfilehash: aad8d76b248aa2cabd84598c4a97a6989c7ee170
ms.sourcegitcommit: 2ab6709741be16ca8029e2afadf19d28cf00fbc7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/14/2022
ms.locfileid: "7970941"
---
# <a name="setting-up-or-changing-the-chart-of-accounts"></a>Настройка или изменение плана счетов

В плане счетов отображаются счета главной книги, на которых хранятся финансовые данные. [!INCLUDE[prod_short](includes/prod_short.md)] включает стандартный план счетов, готовый к использованию в вашей организации.
Однако вы можете изменить счета по умолчанию и добавить новые счета.
<br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE43KO9?rel=0]

## <a name="adding-or-changing-accounts"></a>Добавление или изменение счетов

В плане счетов вы можете открыть каждый счет ГК и добавить или изменить параметры. [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]  

При необходимости для ввода названия счета ГК можно использовать несколько строк. На странице **Карточка счета ГК** в группе **Счет** выберите **Расширенные тексты**, а затем введите в одну или несколько строк копируемый текст и название счета.  

Для счетов, принадлежащих к типу счетов **Итого**, нужно заполнить поле **Группировка**. Для счетов **Сумма (до)** это поле заполняется автоматически функцией отступа. После того, как вы настроили все учетные записи, выберите действие **Процесс**, а затем выберите **Создать отступы в плане счетов**.  

> [!IMPORTANT]
> Если в полях **Группировка** для счетов **Сумма (до)** определения были введены до выполнения функции создания отступов, их следует ввести снова после выполнения этой функции, так как она производит запись значений поверх старых во всех полях **Сумма (до)**.

## <a name="deleting-accounts"></a>Удаление счетов

Вы можете удалить счет главной книги. Однако прежде чем удалять его, должно быть соблюдено следующее:  

* Сальдо счета должно быть нулевым.  
* На странице **Настройка Главной книги** должно быть задано поле **Разрешить удаление счета ГК до**, а на счете не должно быть операций книги в эту дату и после нее.  
* Если на странице **Настройка Главной книги** установлен флажок **Проверка использования счета ГК**, то счет не должен использоваться ни в одной из учетных групп или настроек учета.  

[!INCLUDE[prod_short](includes/prod_short.md)] не допускает удаления счета главной книги, на котором хранятся данные, необходимые для плана счетов.  

## <a name="see-related-training-at-microsoft-learn"></a>См. соответствующее обучение на странице [Microsoft Learn](/learn/modules/chart-accounts-dynamics-365-business-central/index)

## <a name="see-also"></a>См. также

[Главная книга и план счетов](finance-general-ledger.md)  
[Выверка банковских счетов](bank-manage-bank-accounts.md)  
[Работа с измерениями](finance-dimensions.md)  
[Импорт данных из других финансовых систем](across-import-data-configuration-packages.md)  
[Работа с финансовыми отчетами](bi-how-work-account-schedule.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Закрытие счетов отчета о прибылях и убытках во французской версии](LocalFunctionality/France/how-to-close-income-statement-accounts.md)  
[Печать отчетов о прибылях в австралийской версии](LocalFunctionality/Australia/how-to-print-income-statements.md)  
[Печать отчетов о прибылях в новозеландской версии](LocalFunctionality/NewZealand/how-to-print-income-statements.md)  
[Настройка и закрытие сальдо отчета о прибыли и убытках в испанской версии](LocalFunctionality/Spain/how-to-set-up-and-close-income-statement-balances.md)  
[Создание отступа и проверка плана счетов в испанской версии](LocalFunctionality/Spain/how-to-indent-and-validate-chart-of-accounts.md)  

## [!INCLUDE[prod_short](includes/free_trial_md.md)]


[!INCLUDE[footer-include](includes/footer-banner.md)]