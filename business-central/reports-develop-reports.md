---
title: Разработка макетов отчетов и наборов данных
description: Предоставляет обзор данных Business Central.
author: kennieNP
ms.topic: conceptual
ms.devlang: al
ms.reviewer: bholtorf
ms.search.keywords: feature overview
ms.date: 02/03/2022
ms.author: kepontop
ms.service: dynamics-365-business-central
---

# <a name="developing-business-central-report-layouts-and-datasets"></a>Разработка макетов отчетов и наборов данных Business Central

Отчет в [!INCLUDE[prod_short](includes/prod_short.md)] состоит из объекта отчета, который определяет _набор данных_ отчета (какие данные доступны) и количество _макетов отчетов_ (как представлены данные).  

## <a name="developing-report-layouts"></a>Разработка макетов отчетов

Возможно, вы хотите изменить существующие макеты отчетов, представленные в [!INCLUDE[prod_short](includes/prod_short.md)]? В зависимости от технологии, используемой для макета, вы можете сделать это самостоятельно (макеты Excel и, возможно, также Word), или, возможно, вам понадобится разработчик (макеты RDLC с идеальной точностью до пикселя).

| Задача | Ссылка |
|--|--|
| Узнайте больше о различных типах макетов (Word, Excel и RDLC) | [Типы макетов (Word, Excel и RDLC)](ui-manage-report-layouts.md) |
| Узнайте, как создать новый макет отчета. | [Создание нового макета](ui-how-create-custom-report-layout.md) |
| Узнайте, какие шрифты установлены в [!INCLUDE[prod_short](includes/prod_short.md)] Online, чтобы их можно было использовать в макетах отчетов. | [Использование шрифтов в макетах](ui-fonts.md) |
| Научиться работать с макетами Word. | [Работа с макетами Word](ui-how-add-fields-word-report-layout.md) |
| Чтобы узнать, как импортировать/экспортировать файлы макета. | [Импорт/экспорт макета](ui-how-import-and-export-report-layout.md) |
| Чтобы узнать, как обновить определение макета в [!INCLUDE[prod_short](includes/prod_short.md)] на новый файл макета. | [Импорт/экспорт макета](ui-how-import-and-export-report-layout.md) |
| Чтобы узнать, как изменить макет по умолчанию для отчета. | [Изменение макета по умолчанию](ui-how-change-layout-currently-used-report.md) |
<!-- | Научиться работать с макетами Excel | [Работа с макетами Excel](ui-how-add-fields-word-report-layout.md) | -->

## <a name="developing-report-datasets"></a>Разработка наборов данных отчетов

 Чтобы изменить определения набора данных, которые определяют, какие данные доступны в отчете, вам нужен разработчик, который знает язык программирования AL и инструменты для разработки объектов отчета и расширений отчета.

| Задача | Ссылка |
|--|--|
| Узнайте, как программировать отчеты в AL | [Руководство по разработке отчетов](/dynamics365/business-central/dev-itpro/developer/devenv-reports) |
| Узнайте, как сделать отчеты эффективными | [Руководство по настройке производительности отчетов](/dynamics365/business-central/dev-itpro/performance/performance-developer#writing-efficient-reports) |

## <a name="see-also"></a>См. также

[Обзор бизнес-аналитики и отчетности](reports-use-reports.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
