---
title: Как заблокировать покупки от поставщиков
description: Вы можете заблокировать включение поставщиков в какие-либо транзакции или просто заблокировать новые платежи им.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 9cb31546dcefaba5f15cb630467d759812d48c81
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3916755"
---
# <a name="block-vendors"></a><span data-ttu-id="93a5a-103">Блокировка поставщиков</span><span class="sxs-lookup"><span data-stu-id="93a5a-103">Block Vendors</span></span>
<span data-ttu-id="93a5a-104">Можно заблокировать поставщика, например из-за несостоятельности, чтобы этого поставщика нельзя было добавить в документы покупки или чтобы никакие платежи не могли быть учтены для этого поставщика.</span><span class="sxs-lookup"><span data-stu-id="93a5a-104">You can block a vendor, for example because of insolvency, so that the vendor cannot be added to purchase documents or so that no payments can be posted for the vendor.</span></span>

<span data-ttu-id="93a5a-105">В следующей таблице описаны разные варианты блокировки поставщиков.</span><span class="sxs-lookup"><span data-stu-id="93a5a-105">The following table describes the options for blocking vendors.</span></span>  

|<span data-ttu-id="93a5a-106">Параметр</span><span class="sxs-lookup"><span data-stu-id="93a5a-106">Option</span></span>|<span data-ttu-id="93a5a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="93a5a-107">Description</span></span>|  
|--------------------|------------|  
|<span data-ttu-id="93a5a-108">**Пусто**</span><span class="sxs-lookup"><span data-stu-id="93a5a-108">**Blank**</span></span>|<span data-ttu-id="93a5a-109">Транзакции разрешены для данного поставщика.</span><span class="sxs-lookup"><span data-stu-id="93a5a-109">Transactions are allowed for this vendor.</span></span>|
|<span data-ttu-id="93a5a-110">**Оплата**</span><span class="sxs-lookup"><span data-stu-id="93a5a-110">**Payment**</span></span>|<span data-ttu-id="93a5a-111">Новые платежи не могут быть созданы для этого поставщика.</span><span class="sxs-lookup"><span data-stu-id="93a5a-111">New payments cannot be created for this vendor.</span></span>|  
|<span data-ttu-id="93a5a-112">**Все**</span><span class="sxs-lookup"><span data-stu-id="93a5a-112">**All**</span></span>|<span data-ttu-id="93a5a-113">Все транзакции запрещены для данного поставщика.</span><span class="sxs-lookup"><span data-stu-id="93a5a-113">No transactions are allowed for this vendor.</span></span>|  

## <a name="to-block-a-vendor"></a><span data-ttu-id="93a5a-114">Для блокировки поставщика</span><span class="sxs-lookup"><span data-stu-id="93a5a-114">To block a vendor</span></span>  
1. <span data-ttu-id="93a5a-115">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Поставщики**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="93a5a-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span></span>
2. <span data-ttu-id="93a5a-116">Выберите поставщика, которого требуется заблокировать.</span><span class="sxs-lookup"><span data-stu-id="93a5a-116">Select the vendor that you want to block.</span></span>
3. <span data-ttu-id="93a5a-117">В поле **Заблокировано** выберите один из вариантов блокировки.</span><span class="sxs-lookup"><span data-stu-id="93a5a-117">In the **Blocked** field, choose one of the options for blocking.</span></span>

## <a name="see-also"></a><span data-ttu-id="93a5a-118">См. также</span><span class="sxs-lookup"><span data-stu-id="93a5a-118">See Also</span></span>  
[<span data-ttu-id="93a5a-119">Регистрация новых поставщиков</span><span class="sxs-lookup"><span data-stu-id="93a5a-119">Register New Vendors</span></span>](purchasing-how-register-new-vendors.md)  
[<span data-ttu-id="93a5a-120">Осуществление платежей</span><span class="sxs-lookup"><span data-stu-id="93a5a-120">Making Payments</span></span>](payables-make-payments.md)  
[<span data-ttu-id="93a5a-121">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="93a5a-121">Managing Payables</span></span>](payables-manage-payables.md)
