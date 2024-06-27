---
title: Общие сведения о Microsoft Fabric и Business Central
description: 'Получение обзора использования Microsoft Fabric для получения аналитических сведений, бизнес-аналитики и ключевых показателей эффективности из данных Business Central.'
author: kennienp
ms.topic: overview
ms.search.keywords: 'account schedule, analysis, reporting, financial report, business intelligence, KPI'
ms.search.form: '6316, 6317'
ms.reviewer: bholtorf
ms.date: 04/24/2024
ms.author: kepontop
ms.custom: bap-template
ms.service: dynamics-365-business-central
---
# Общие сведения о Microsoft Fabric и Business Central

[!INCLUDE[microsoft_fabric](includes/microsoft_fabric.md)] &mdash; это комплексное аналитическое решение с полным спектром возможностей, включая перемещение данных, озера данных, инжиниринг данных, интеграцию данных, обработку и анализ данных, аналитику в реальном времени и бизнес-аналитику на единой платформе, обеспечивающей безопасность данных, управление ими и обеспечение соответствия нормативным требованиям. Вашей организации больше не нужно объединять отдельные аналитические службы от нескольких поставщиков. Вместо этого используйте оптимизированное решение, которое легко подключить, внедрить и использовать.

> [!NOTE]
> Подробные сведения о плане выпуска Microsoft Fabric см. в статье [aka.ms/FabricRoadmap](https://aka.ms/FabricRoadmap)
> 
> Регулярная публикация этой дорожной карты поможет вам быть в курсе усовершенствований [!INCLUDE[microsoft_fabric](includes/microsoft_fabric.md)].

## Какое место [!INCLUDE[microsoft_fabric](includes/microsoft_fabric.md)] занимает в аналитике [!INCLUDE[prod_short](includes/prod_short.md)]

[!INCLUDE[prod_short](includes/prod_short.md)] поставляется с множеством готовых отчетов и возможностей анализа данных, таких как финансовая отчетность, открываемая в Excel, и режим анализа списков и запросов. Кроме того, можно без труда определять отчеты Power BI, которые считывают данные из стандартных и пользовательских API, определять системы показателей Power BI и встраивать все это непосредственно в клиент [!INCLUDE[prod_short](includes/prod_short.md)]. Но для пользователей с более сложными сценариями обработки и анализа данных или бизнес-аналитики, требующими более глубокого инжиниринга данных или интеграции данных [!INCLUDE[microsoft_fabric](includes/microsoft_fabric.md)] может быть хорошим вариантом. 

## OneLake

Ключевым компонентом предложения [!INCLUDE[microsoft_fabric](includes/microsoft_fabric.md)] является OneLake. OneLake — это единое логическое озеро данных для всей организации. Вы можете представить себе OneLake как OneDrive для данных. Вы получаете озеро данных как услугу без необходимости создавать его самостоятельно. OneLake автоматически поставляется вместе с каждым арендатором [!INCLUDE[microsoft_fabric](includes/microsoft_fabric.md)] и не предполагает инфраструктуры, которой нужно будет управлять. Все данные, поступающие в OneLake, автоматически участвуют в стандартном управлении данными, включая отслеживание происхождения данных, защиту данных, сертификацию и интеграцию каталогов. Эта служба устраняет разрозненность данных, позволяя различным частям организации работать независимо и при этом вносить вклад одно и то же озеро данных.

[!INCLUDE[microsoft_fabric](includes/microsoft_fabric.md)] хранит ваши данные в OneLake в открытом формате. Для структурированных табличных данных этот формат *Delta Parquet*. Формат Delta Parquet позволяет любому аналитическому механизму в [!INCLUDE[microsoft_fabric](includes/microsoft_fabric.md)] осуществлять доступ к данным из других аналитических систем. Таким образом, специалисты по работе с данными могут гибко использовать инструменты на свой выбор.


## См. также
[Использование Power BI с Business Central](admin-powerbi.md)   

[!INCLUDE[footer-include](includes/footer-banner.md)]
