---
title: Советы и подсказки — RapidStart Services | Документация Майкрософт
description: При настройке организаций с помощью RapidStart Services можно воспользоваться некоторыми советами и подсказками для упрощения реализации.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: acdac865286577b30f9fe036cca8a50eb7e143a0
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2019
ms.locfileid: "2878990"
---
# <a name="tips-and-tricks-rapidstart-services"></a><span data-ttu-id="13dab-103">Советы и подсказки: RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="13dab-103">Tips and Tricks: RapidStart Services</span></span>
<span data-ttu-id="13dab-104">При настройке организаций с помощью RapidStart Services можно воспользоваться некоторыми советами и подсказками для упрощения реализации.</span><span class="sxs-lookup"><span data-stu-id="13dab-104">When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.</span></span>  

## <a name="take-advantage-of-configuration-templates"></a><span data-ttu-id="13dab-105">Воспользуйтесь шаблонами конфигураций</span><span class="sxs-lookup"><span data-stu-id="13dab-105">Take advantage of configuration templates</span></span>  
<span data-ttu-id="13dab-106">Шаблоны конфигураций помогают упростить процесс внедрения.</span><span class="sxs-lookup"><span data-stu-id="13dab-106">Configuration templates can help you streamline your implementation process.</span></span> <span data-ttu-id="13dab-107">Используя их, можно включить аналогичные клиентов в сегменты, а затем разработать протокол реализации, обрабатывающий всех клиентов в сегменте подобным образом.</span><span class="sxs-lookup"><span data-stu-id="13dab-107">By using them, you can include similar customers in segments and then develop an implementation protocol that treats all customers in a segment in a similar manner.</span></span> <span data-ttu-id="13dab-108">В этом способе можно применить уровень предварительных настроек к каждому сегменту и продолжить быстрое внедрение.</span><span class="sxs-lookup"><span data-stu-id="13dab-108">In that way, you can apply a level of preconfiguration to each segment and continue with a rapid implementation.</span></span>  

## <a name="configuration-questionnaires"></a><span data-ttu-id="13dab-109">Анкеты конфигурации</span><span class="sxs-lookup"><span data-stu-id="13dab-109">Configuration questionnaires</span></span>  
<span data-ttu-id="13dab-110">Чтобы упростить процесс заполнения анкеты конфигурации, определите значения по умолчанию в соответствии с оптимальными методами работы.</span><span class="sxs-lookup"><span data-stu-id="13dab-110">To aid the process of filling out a configuration questionnaire, consider defining default answers to indicate best practices.</span></span>  

## <a name="batch-creation-of-journal-lines"></a><span data-ttu-id="13dab-111">Пакетное создание строк журнала</span><span class="sxs-lookup"><span data-stu-id="13dab-111">Batch creation of journal lines</span></span>  
<span data-ttu-id="13dab-112">Рекомендуется использовать инструменты переноса данных, предоставленные для переноса записей журнала.</span><span class="sxs-lookup"><span data-stu-id="13dab-112">We recommend that you use the data migration tools provided to migrate journal entries.</span></span> <span data-ttu-id="13dab-113">В противном случае при использовании пакетного задания для создания строки журнала, он имеет ограниченный объем и генерирует предварительно созданные по умолчанию поля в журнале.</span><span class="sxs-lookup"><span data-stu-id="13dab-113">Otherwise, if you use a batch job to create journal lines, that has a limited scope and only generates pre-default fields into a journal.</span></span> <span data-ttu-id="13dab-114">Остальные поля журнала необходимо затем заполнить вручную.</span><span class="sxs-lookup"><span data-stu-id="13dab-114">The rest of the journal then has to be completed manually.</span></span>  

## <a name="migrating-transactions"></a><span data-ttu-id="13dab-115">Перенос транзакций</span><span class="sxs-lookup"><span data-stu-id="13dab-115">Migrating transactions</span></span>  
<span data-ttu-id="13dab-116">Рекомендуется переносить начальные сальдо в указанном ниже порядке.</span><span class="sxs-lookup"><span data-stu-id="13dab-116">We recommend that you migrate opening balances in the following order.</span></span>  

1.  <span data-ttu-id="13dab-117">Выполните миграцию начальных сальдо без использования вложенных книг счетов Главной книги.</span><span class="sxs-lookup"><span data-stu-id="13dab-117">Migrate general ledger opening balances without using the general ledger account subledgers.</span></span> <span data-ttu-id="13dab-118">Используйте определенные корреспондирующие счета с начальным сальдо для каждой книги.</span><span class="sxs-lookup"><span data-stu-id="13dab-118">Use specific opening balance offsetting accounts, one set up for each subledger.</span></span> <span data-ttu-id="13dab-119">Настройте корреспондирующие счета, чтобы включить непосредственный учет.</span><span class="sxs-lookup"><span data-stu-id="13dab-119">Set up the offsetting accounts to enable direct postings.</span></span>  
2.  <span data-ttu-id="13dab-120">Перенесите открытые операции книги клиентов.</span><span class="sxs-lookup"><span data-stu-id="13dab-120">Migrate open customer ledger entries.</span></span>  
3.  <span data-ttu-id="13dab-121">Перенесите открытые операции книги, связанные товарами.</span><span class="sxs-lookup"><span data-stu-id="13dab-121">Migrate open item ledger entries.</span></span>  
4.  <span data-ttu-id="13dab-122">Выполните миграцию открытых операций основных средств.</span><span class="sxs-lookup"><span data-stu-id="13dab-122">Migrate open fixed asset entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="13dab-123">См. также</span><span class="sxs-lookup"><span data-stu-id="13dab-123">See Also</span></span>  
[<span data-ttu-id="13dab-124">Настройка организации со службами RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="13dab-124">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="13dab-125">Администрация</span><span class="sxs-lookup"><span data-stu-id="13dab-125">Administration</span></span>](admin-setup-and-administration.md)
