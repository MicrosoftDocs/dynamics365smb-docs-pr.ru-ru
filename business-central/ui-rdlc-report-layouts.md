---
title: Работа с макетами RDLC
description: Ознакомьтесь с макетами отчетов RDLC.
author: jswymer
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 'customized report, document layout, logo, personalize'
ms.search.form: '9650, 9652'
ms.date: 03/14/2022
ms.author: jswymer
---
# <a name="working-with-rdlc-layouts"></a><a name="working-with-rdlc-layouts"></a>Работа с макетами RDLC

Макеты RDLC основаны на клиентских макетах определения отчета (типы файла RDL или RDLC). Концепции разработки макетов RDLC аналогичны другим типам макетов. Макет определяет, какие поля отображать и как они расположены. Однако разработка макетов RDLC более сложная, чем макетов Word и Excel.

[![Показывает разные элементы макета RDLC.](media/rdlc-layout.png)](media/rdlc-layout.png#lightbox)

## <a name="required-tools"></a><a name="required-tools"></a>Необходимые средства

Чтобы изменить макеты RDL, вы можете использовать либо конструктор отчетов Microsoft SQL Server, либо Microsoft RDLC Report Designer.

- Построитель отчетов — это автономное приложение, устанавливаемое на ваш компьютер вами или администратором. При локальной установке Business Central построитель отчетов автоматически устанавливается вместе с установкой Business Central Server. Дополнительные сведения об установке построителя отчетов см. в [Установка построителя отчетов](/sql/reporting-services/install-windows/install-report-builder) в документации SQL Server.

- RDLC Report Designer — это расширение для Visual Studio 2017 и более новых версий. Вы можете загрузить и установить RDLC Report Designer в [магазине Visual Studio](https://marketplace.visualstudio.com/items?itemName=ProBITools.MicrosoftRdlcReportDesignerforVisualStudio-18001).

## <a name="create-and-modify-rdlc-layouts"></a><a name="create-and-modify-rdlc-layouts"></a>Создание и изменение макетов RDLC

Создание и изменение макетов RDLC — сложная задача, которую обычно выполняют опытные пользователи или разработчики. Основные понятия не относятся к макетам отчетов Business Central. По этой причине мы отсылаем вас к следующей документации:

- [Создать отчет макета RDL](/dynamics365/business-central/dev-itpro/developer/devenv-howto-rdl-report-layout)

    В этой статье объясняется, как создать макет отчета RDLC из кода AL.

- [Отчеты, части отчетов и определения отчетов](/sql/reporting-services/report-design/reports-report-parts-and-report-definitions-report-builder-and-ssrs?)

 Ссылки на документацию служб SQL Server Reporting Services для RDL/RDLC. Эта документация объясняет концепции  
RDL/RDLC и способы использования построителя отчетов.

> [!NOTE]
> Построитель отчетов распознает только файлы типа RDL, но не RDLC. Файлы макетов, экспортированные из Business Central, это файлы типа RDLC. Поэтому, чтобы изменить этот макет в построителе отчетов, переименуйте тип файла в RDL.

## <a name="see-related-microsoft-training"></a><a name="see-related-microsoft-training"></a>См. соответствующее [обучение Microsoft](/training/modules/change-documents-dynamics-365-business-central/index)

## <a name="see-also"></a><a name="see-also"></a>См. также

[Управление макетами отчетов](ui-manage-report-layouts.md)  
[Установите макет, используемый отчетом](ui-set-report-layout.md)  
[Приступайте к созданию макетов отчетов](ui-get-started-layouts.md)  
[Работа с отчетами, пакетными заданиями и XMLport](ui-work-report.md)  
[Бизнес-аналитика](bi.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Анализ данных отчета с помощью Excel](report-analyze-excel.md).

[!INCLUDE[footer-include](includes/footer-banner.md)]
