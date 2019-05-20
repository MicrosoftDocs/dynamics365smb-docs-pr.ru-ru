---
title: Связывание и синхронизация записей вручную | Документы Майкрософт
description: Синхронизация сопоставления таблиц интеграции позволяет синхронизировать данные во всех записях в таблице в Business Central и объекте Dynamics 365 for Sales, которые связаны.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: crm, sales, couple, decouple, synchronize
ms.date: 04/01/2019
ms.author: bholtorf
ms.openlocfilehash: 36f1a0fe8c50744d9ce13d1e6c3c899f4ceaf5e4
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1245409"
---
# <a name="couple-and-synchronize-records-manually"></a><span data-ttu-id="6f50d-103">Связывание и синхронизация записей вручную</span><span class="sxs-lookup"><span data-stu-id="6f50d-103">Couple and Synchronize Records Manually</span></span>
<span data-ttu-id="6f50d-104">В этом разделе описана процедура связывания одной или нескольких записей [!INCLUDE[d365fin](includes/d365fin_md.md)] с записями в [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6f50d-104">This topic describes how to couple one or more records in [!INCLUDE[d365fin](includes/d365fin_md.md)] with records in [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="6f50d-105">Связывание записей позволяет просматривать сведения [!INCLUDE[crm_md](includes/crm_md.md)] из [!INCLUDE[d365fin](includes/d365fin_md.md)] и наоборот.</span><span class="sxs-lookup"><span data-stu-id="6f50d-105">Coupling records lets you view [!INCLUDE[crm_md](includes/crm_md.md)] information from [!INCLUDE[d365fin](includes/d365fin_md.md)], and vice versa.</span></span> <span data-ttu-id="6f50d-106">Связывание также позволяет синхронизировать данные между записями.</span><span class="sxs-lookup"><span data-stu-id="6f50d-106">The coupling also enables you to synchronize data between the records.</span></span> <span data-ttu-id="6f50d-107">Можно связать существующие записи или создать и связать новые записи.</span><span class="sxs-lookup"><span data-stu-id="6f50d-107">You can couple existing records, or create and couple new records.</span></span>

> [!Note]
> <span data-ttu-id="6f50d-108">Связывание и синхронизация данных с [!INCLUDE[crm_md](includes/crm_md.md)] доступны только в том случае, если системный администратор создал подключение между [!INCLUDE[d365fin](includes/d365fin_md.md)] и [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="6f50d-108">Coupling and synchronizing data with [!INCLUDE[crm_md](includes/crm_md.md)] is available only if your system administrator has created a connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="6f50d-109">Быстрый способ проверить — это открыть карточку **Клиент** и найти действие **Настроить связывание**.</span><span class="sxs-lookup"><span data-stu-id="6f50d-109">A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action.</span></span> <span data-ttu-id="6f50d-110">Если действие доступно, приложения подключены.</span><span class="sxs-lookup"><span data-stu-id="6f50d-110">If the action is available, the apps are connected.</span></span>   

## <a name="to-couple-a-record"></a><span data-ttu-id="6f50d-111">Связывание записи</span><span class="sxs-lookup"><span data-stu-id="6f50d-111">To couple a record</span></span>  
1.  <span data-ttu-id="6f50d-112">В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте карточку для записи, которую требуется связать.</span><span class="sxs-lookup"><span data-stu-id="6f50d-112">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="6f50d-113">Например, карточка клиента или контакта.</span><span class="sxs-lookup"><span data-stu-id="6f50d-113">For example, the Customer or Contact card.</span></span>  

    <span data-ttu-id="6f50d-114">Можно также открыть страницу списка и выбрать запись, которую следует связать.</span><span class="sxs-lookup"><span data-stu-id="6f50d-114">You can also just open the list page and select the record that you want to couple.</span></span>  

2.  <span data-ttu-id="6f50d-115">Выберите действие **Настроить связывание**.</span><span class="sxs-lookup"><span data-stu-id="6f50d-115">Choose the **Set Up Coupling** action.</span></span>  
3.  <span data-ttu-id="6f50d-116">Заполните поля, затем выберите **ОК**.</span><span class="sxs-lookup"><span data-stu-id="6f50d-116">Fill in the fields, and then choose **OK**.</span></span>  

## <a name="to-synchronize-a-single-record"></a><span data-ttu-id="6f50d-117">Синхронизация одной записи</span><span class="sxs-lookup"><span data-stu-id="6f50d-117">To synchronize a single record</span></span>  
1.  <span data-ttu-id="6f50d-118">В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте карточку для записи, которую требуется связать.</span><span class="sxs-lookup"><span data-stu-id="6f50d-118">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="6f50d-119">Например, карточка клиента или контакта.</span><span class="sxs-lookup"><span data-stu-id="6f50d-119">For example, the Customer or Contact card.</span></span>  
2.  <span data-ttu-id="6f50d-120">Выберите действие **Синхронизировать сейчас**.</span><span class="sxs-lookup"><span data-stu-id="6f50d-120">Choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="6f50d-121">Если запись можно синхронизировать из [!INCLUDE[d365fin](includes/d365fin_md.md)] с [!INCLUDE[crm_md](includes/crm_md.md)] или из [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)], выберите параметр, определяющий направление обновления данных, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="6f50d-121">If a record can be synchronized either from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[crm_md](includes/crm_md.md)] or from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], select the option that specifies the direction of data update, and then choose **OK**.</span></span>  

## <a name="to-synchronize-multiple-records"></a><span data-ttu-id="6f50d-122">Синхронизация нескольких записей</span><span class="sxs-lookup"><span data-stu-id="6f50d-122">To synchronize multiple records</span></span>  
1.  <span data-ttu-id="6f50d-123">В [!INCLUDE[d365fin](includes/d365fin_md.md)] откройте страницу списка для записи, например страницы списка "Клиенты" или "Контакты".</span><span class="sxs-lookup"><span data-stu-id="6f50d-123">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the list page for the record, such as the Customers or Contacts list pages.</span></span>  
2.  <span data-ttu-id="6f50d-124">Выберите записи, который требуется синхронизировать, затем выберите действие **Синхронизировать сейчас**.</span><span class="sxs-lookup"><span data-stu-id="6f50d-124">Select the records that you want to synchronize, and then choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="6f50d-125">Если записи можно синхронизировать из [!INCLUDE[d365fin](includes/d365fin_md.md)] с [!INCLUDE[crm_md](includes/crm_md.md)] или из [!INCLUDE[crm_md](includes/crm_md.md)] с [!INCLUDE[d365fin](includes/d365fin_md.md)], выберите параметр, определяющий направление обновления данных, а затем нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="6f50d-125">If records can be synchronized either from [!INCLUDE[d365fin](includes/d365fin_md.md)] to [!INCLUDE[crm_md](includes/crm_md.md)] or from [!INCLUDE[crm_md](includes/crm_md.md)] to [!INCLUDE[d365fin](includes/d365fin_md.md)], select the option that specifies the direction of data update, and then choose **OK**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6f50d-126">См. также</span><span class="sxs-lookup"><span data-stu-id="6f50d-126">See Also</span></span>  
[<span data-ttu-id="6f50d-127">Использование Dynamics 365 for Sales из Business Central</span><span class="sxs-lookup"><span data-stu-id="6f50d-127">Using Dynamics 365 for Sales from Business Central</span></span>](marketing-integrate-dynamicscrm.md)
