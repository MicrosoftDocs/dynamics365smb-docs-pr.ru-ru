---
title: "Советы и подсказки — службы RapidStart Services | Документы Майкрософт"
description: "При настройке организаций с помощью служб RapidStart Services можно воспользоваться некоторыми советами и подсказками для упрощения реализации."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 03/05/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 4e8dc4436b01f69292a01afbc7a5d0381b544a77
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="tips-and-tricks-rapidstart-services"></a><span data-ttu-id="f7390-103">Советы и подсказки. Службы RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="f7390-103">Tips and Tricks: RapidStart Services</span></span>
<span data-ttu-id="f7390-104">При настройке организаций с помощью служб RapidStart Services можно воспользоваться некоторыми советами и подсказками для упрощения реализации.</span><span class="sxs-lookup"><span data-stu-id="f7390-104">When you configure companies using RapidStart Services, there are some tips and tricks that you can take advantage of to help your implementation go smoothly.</span></span>  

## <a name="take-advantage-of-configuration-templates"></a><span data-ttu-id="f7390-105">Воспользуйтесь шаблонами конфигураций</span><span class="sxs-lookup"><span data-stu-id="f7390-105">Take advantage of configuration templates</span></span>  
<span data-ttu-id="f7390-106">Шаблоны конфигураций помогают упростить процесс внедрения.</span><span class="sxs-lookup"><span data-stu-id="f7390-106">Configuration templates can help you streamline your implementation process.</span></span> <span data-ttu-id="f7390-107">Используя их, можно включить аналогичные клиентов в сегменты, а затем разработать протокол реализации, обрабатывающий всех клиентов в сегменте подобным образом.</span><span class="sxs-lookup"><span data-stu-id="f7390-107">By using them, you can include similar customers in segments and then develop an implementation protocol that treats all customers in a segment in a similar manner.</span></span> <span data-ttu-id="f7390-108">В этом способе можно применить уровень предварительных настроек к каждому сегменту и продолжить быстрое внедрение.</span><span class="sxs-lookup"><span data-stu-id="f7390-108">In that way, you can apply a level of preconfiguration to each segment and continue with a rapid implementation.</span></span>  

## <a name="configuration-questionnaires"></a><span data-ttu-id="f7390-109">Анкеты конфигурации</span><span class="sxs-lookup"><span data-stu-id="f7390-109">Configuration questionnaires</span></span>  
<span data-ttu-id="f7390-110">Чтобы упростить процесс заполнения анкеты конфигурации, определите значения по умолчанию в соответствии с оптимальными методами работы.</span><span class="sxs-lookup"><span data-stu-id="f7390-110">To aid the process of filling out a configuration questionnaire, consider defining default answers to indicate best practices.</span></span>  

## <a name="batch-creation-of-journal-lines"></a><span data-ttu-id="f7390-111">Пакетное создание строк журнала</span><span class="sxs-lookup"><span data-stu-id="f7390-111">Batch creation of journal lines</span></span>  
<span data-ttu-id="f7390-112">Рекомендуется использовать инструменты переноса данных, предоставленные для переноса записей журнала.</span><span class="sxs-lookup"><span data-stu-id="f7390-112">We recommend that you use the data migration tools provided to migrate journal entries.</span></span> <span data-ttu-id="f7390-113">В противном случае при использовании пакетного задания для создания строки журнала, он имеет ограниченный объем и генерирует предварительно созданные по умолчанию поля в журнале.</span><span class="sxs-lookup"><span data-stu-id="f7390-113">Otherwise, if you use a batch job to create journal lines, that has a limited scope and only generates pre-default fields into a journal.</span></span> <span data-ttu-id="f7390-114">Остальные поля журнала необходимо затем заполнить вручную.</span><span class="sxs-lookup"><span data-stu-id="f7390-114">The rest of the journal then has to be completed manually.</span></span>  

## <a name="migrating-transactions"></a><span data-ttu-id="f7390-115">Перенос транзакций</span><span class="sxs-lookup"><span data-stu-id="f7390-115">Migrating transactions</span></span>  
<span data-ttu-id="f7390-116">Рекомендуется переносить начальные сальдо в указанном ниже порядке.</span><span class="sxs-lookup"><span data-stu-id="f7390-116">We recommend that you migrate opening balances in the following order.</span></span>  

1.  <span data-ttu-id="f7390-117">Выполните миграцию начальных сальдо без использования вложенных книг счетов Главной книги.</span><span class="sxs-lookup"><span data-stu-id="f7390-117">Migrate general ledger opening balances without using the general ledger account subledgers.</span></span> <span data-ttu-id="f7390-118">Используйте определенные корреспондирующие счета с начальным сальдо для каждой книги.</span><span class="sxs-lookup"><span data-stu-id="f7390-118">Use specific opening balance offsetting accounts, one set up for each subledger.</span></span> <span data-ttu-id="f7390-119">Настройте корреспондирующие счета, чтобы включить непосредственный учет.</span><span class="sxs-lookup"><span data-stu-id="f7390-119">Set up the offsetting accounts to enable direct postings.</span></span>  
2.  <span data-ttu-id="f7390-120">Перенесите открытые операции книги клиентов.</span><span class="sxs-lookup"><span data-stu-id="f7390-120">Migrate open customer ledger entries.</span></span>  
3.  <span data-ttu-id="f7390-121">Перенесите открытые операции книги, связанные товарами.</span><span class="sxs-lookup"><span data-stu-id="f7390-121">Migrate open item ledger entries.</span></span>  
4.  <span data-ttu-id="f7390-122">Выполните миграцию открытых операций основных средств.</span><span class="sxs-lookup"><span data-stu-id="f7390-122">Migrate open fixed asset entries.</span></span>  

## <a name="see-also"></a><span data-ttu-id="f7390-123">См. также</span><span class="sxs-lookup"><span data-stu-id="f7390-123">See Also</span></span>  
[<span data-ttu-id="f7390-124">Настройка компании с помощью служб RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="f7390-124">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="f7390-125">Администрация</span><span class="sxs-lookup"><span data-stu-id="f7390-125">Administration</span></span>](admin-setup-and-administration.md)

