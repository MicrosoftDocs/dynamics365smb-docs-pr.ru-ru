---
title: Связывание и синхронизация записей вручную | Документация Майкрософт
description: Синхронизация сопоставления таблиц интеграции позволяет синхронизировать данные во всех записях в связанных таблице Business Central и объекте Dynamics 365 Sales.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: crm, sales, couple, decouple, synchronize
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: d8140f71709208a271eff5c8de415b0e95736072
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3911409"
---
# <a name="couple-and-synchronize-records-manually"></a><span data-ttu-id="fc766-103">Связывание и синхронизация записей вручную</span><span class="sxs-lookup"><span data-stu-id="fc766-103">Couple and Synchronize Records Manually</span></span>
<span data-ttu-id="fc766-104">В этом разделе описана процедура связывания одной или нескольких записей [!INCLUDE[d365fin](includes/d365fin_md.md)] с записями в Common Data Service или [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="fc766-104">This topic describes how to couple one or more records in [!INCLUDE[d365fin](includes/d365fin_md.md)] with records in Common Data Service or [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="fc766-105">Связывание записей позволяет просматривать сведения Common Data Service из [!INCLUDE[d365fin](includes/d365fin_md.md)] и наоборот.</span><span class="sxs-lookup"><span data-stu-id="fc766-105">Coupling records lets you view Common Data Service information from [!INCLUDE[d365fin](includes/d365fin_md.md)], and vice versa.</span></span> <span data-ttu-id="fc766-106">Связывание также позволяет синхронизировать данные между записями.</span><span class="sxs-lookup"><span data-stu-id="fc766-106">The coupling also enables you to synchronize data between the records.</span></span> <span data-ttu-id="fc766-107">Можно связать существующие записи или создать и связать новые записи.</span><span class="sxs-lookup"><span data-stu-id="fc766-107">You can couple existing records, or create and couple new records.</span></span>

> [!Note]
> <span data-ttu-id="fc766-108">Связывание и синхронизация данных доступны только в том случае, если системный администратор создал подключение между [!INCLUDE[d365fin](includes/d365fin_md.md)] и Common Data Service или [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="fc766-108">Coupling and synchronizing data is available only if your system administrator has created a connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and Common Data Service or [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="fc766-109">Быстрый способ проверить — это открыть карточку **Клиент** и найти действие **Настроить связывание**.</span><span class="sxs-lookup"><span data-stu-id="fc766-109">A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action.</span></span> <span data-ttu-id="fc766-110">Если действие доступно, приложения подключены.</span><span class="sxs-lookup"><span data-stu-id="fc766-110">If the action is available, the apps are connected.</span></span>   

## <a name="video-example"></a><span data-ttu-id="fc766-111">Видео с примером</span><span class="sxs-lookup"><span data-stu-id="fc766-111">Video Example</span></span>

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098376]

## <a name="to-couple-a-record"></a><span data-ttu-id="fc766-112">Связывание записи</span><span class="sxs-lookup"><span data-stu-id="fc766-112">To couple a record</span></span>  
1.  <span data-ttu-id="fc766-113">В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте карточку для записи, которую требуется связать.</span><span class="sxs-lookup"><span data-stu-id="fc766-113">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="fc766-114">Например, карточка клиента или контакта.</span><span class="sxs-lookup"><span data-stu-id="fc766-114">For example, the Customer or Contact card.</span></span>  

    <span data-ttu-id="fc766-115">Можно также открыть страницу списка и выбрать запись, которую следует связать.</span><span class="sxs-lookup"><span data-stu-id="fc766-115">You can also just open the list page and select the record that you want to couple.</span></span>  

2.  <span data-ttu-id="fc766-116">Выберите действие **Настроить связывание**.</span><span class="sxs-lookup"><span data-stu-id="fc766-116">Choose the **Set Up Coupling** action.</span></span>  
3.  <span data-ttu-id="fc766-117">Заполните поля, затем выберите **ОК**.</span><span class="sxs-lookup"><span data-stu-id="fc766-117">Fill in the fields, and then choose **OK**.</span></span>  

## <a name="to-synchronize-a-single-record"></a><span data-ttu-id="fc766-118">Синхронизация одной записи</span><span class="sxs-lookup"><span data-stu-id="fc766-118">To synchronize a single record</span></span>  
1.  <span data-ttu-id="fc766-119">В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте карточку для записи, которую требуется связать.</span><span class="sxs-lookup"><span data-stu-id="fc766-119">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="fc766-120">Например, карточка клиента или контакта.</span><span class="sxs-lookup"><span data-stu-id="fc766-120">For example, the Customer or Contact card.</span></span>  
2.  <span data-ttu-id="fc766-121">Выберите действие **Синхронизировать сейчас**.</span><span class="sxs-lookup"><span data-stu-id="fc766-121">Choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="fc766-122">Если запись можно синхронизировать в одном направлении, выберите параметр, определяющий направление обновления данных, затем выберите **ОК**.</span><span class="sxs-lookup"><span data-stu-id="fc766-122">If a record can be synchronized in one direction, select the option that specifies the direction of data update, and then choose **OK**.</span></span>  

## <a name="to-synchronize-a-single-record-from-crm_md"></a><span data-ttu-id="fc766-123">Синхронизация одной записи из [!INCLUDE[crm_md](includes/crm_md.md)]</span><span class="sxs-lookup"><span data-stu-id="fc766-123">To synchronize a single record from [!INCLUDE[crm_md](includes/crm_md.md)]</span></span>  
1.  <span data-ttu-id="fc766-124">В [!INCLUDE[crm_md](includes/crm_md.md)] откройте форму для записи, которую требуется связать.</span><span class="sxs-lookup"><span data-stu-id="fc766-124">In [!INCLUDE[crm_md](includes/crm_md.md)], open the form for the record you want to couple.</span></span> <span data-ttu-id="fc766-125">Например, форма карточки организации или карточки контакта.</span><span class="sxs-lookup"><span data-stu-id="fc766-125">For example, the Account card or Contact card form.</span></span>  
2.  <span data-ttu-id="fc766-126">Выберите действие **[!INCLUDE[d365fin](includes/d365fin_md.md)]** на ленте, чтобы открыть и связать запись автоматически.</span><span class="sxs-lookup"><span data-stu-id="fc766-126">Choose the **[!INCLUDE[d365fin](includes/d365fin_md.md)]** action in the ribbon to open and couple record automatically.</span></span>

> [!Note]
> <span data-ttu-id="fc766-127">Вы можете синхронизировать одну запись из [!INCLUDE[crm_md](includes/crm_md.md)] автоматически, только когда параметр **Синхр. только связанные записи** отключен, и установлено направление синхронизации "Двунаправленная" или "Из таблицы интеграции" на странице **Сопоставление таблиц интеграции** для записи.</span><span class="sxs-lookup"><span data-stu-id="fc766-127">You can synchronize a single record from [!INCLUDE[crm_md](includes/crm_md.md)] automatically only when **Sync. Only Coupled Records** is disabled and the synchronization direction is set to Bidirectional or From Integration Table on the **Integration Table Mapping** page for the record.</span></span> <span data-ttu-id="fc766-128">Дополнительные сведения см. в разделе [Сопоставление таблиц и полей для синхронизации](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).</span><span class="sxs-lookup"><span data-stu-id="fc766-128">For more information, see [Mapping the Tables and Fields to Synchronize](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).</span></span>     

## <a name="to-synchronize-multiple-records"></a><span data-ttu-id="fc766-129">Синхронизация нескольких записей</span><span class="sxs-lookup"><span data-stu-id="fc766-129">To synchronize multiple records</span></span>  
1.  <span data-ttu-id="fc766-130">В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте страницу списка для записи, например страницы списка "Клиенты" или "Контакты".</span><span class="sxs-lookup"><span data-stu-id="fc766-130">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the list page for the record, such as the Customers or Contacts list pages.</span></span>  
2.  <span data-ttu-id="fc766-131">Выберите записи, который требуется синхронизировать, затем выберите действие **Синхронизировать сейчас**.</span><span class="sxs-lookup"><span data-stu-id="fc766-131">Select the records that you want to synchronize, and then choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="fc766-132">Если записи можно синхронизировать в одном направлении, выберите параметр, определяющий направление, затем выберите **ОК**.</span><span class="sxs-lookup"><span data-stu-id="fc766-132">If records can be synchronized in one direction, select the option that specifies the direction, and then choose **OK**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fc766-133">См. также</span><span class="sxs-lookup"><span data-stu-id="fc766-133">See Also</span></span>  
[<span data-ttu-id="fc766-134">Использование Dynamics 365 Sales из Business Central</span><span class="sxs-lookup"><span data-stu-id="fc766-134">Using Dynamics 365 Sales from Business Central</span></span>](marketing-integrate-dynamicscrm.md)
