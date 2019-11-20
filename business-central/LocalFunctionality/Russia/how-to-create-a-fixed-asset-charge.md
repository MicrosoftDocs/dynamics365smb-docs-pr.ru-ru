---
title: Создание издержек основных средств в России
description: Российские улучшения включают издержки ОС.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 1d9c009b436d7cd0228f78f1bd315e6ddcaadd70
ms.sourcegitcommit: 319023e53627dbe8e68643908aacc6fd594a4957
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/04/2019
ms.locfileid: "2554521"
---
# <a name="create-a-fixed-asset-charge"></a><span data-ttu-id="1fa63-103">Создание издержек ОС</span><span class="sxs-lookup"><span data-stu-id="1fa63-103">Create a Fixed Asset Charge</span></span>

<span data-ttu-id="1fa63-104">Ниже показано, как создать новые издержки основного средства.</span><span class="sxs-lookup"><span data-stu-id="1fa63-104">The following procedure shows how to create a new fixed asset charge.</span></span> 

## <a name="to-create-a-fixed-asset-charge"></a><span data-ttu-id="1fa63-105">Создание издержек ОС</span><span class="sxs-lookup"><span data-stu-id="1fa63-105">To create a fixed asset charge</span></span>

1. <span data-ttu-id="1fa63-106">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Карточка издержки ОС**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="1fa63-106">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Charge Card**, and then choose the related link.</span></span>

2. <span data-ttu-id="1fa63-107">На экспресс-вкладке **Общее** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="1fa63-107">On the **General** FastTab, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="1fa63-108">Поле</span><span class="sxs-lookup"><span data-stu-id="1fa63-108">Field</span></span>                        | <span data-ttu-id="1fa63-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1fa63-109">Description</span></span>                                                  |
   | :--------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="1fa63-110">**Номер**</span><span class="sxs-lookup"><span data-stu-id="1fa63-110">**No.**</span></span>                      | <span data-ttu-id="1fa63-111">Укажите код издержки основного средства.</span><span class="sxs-lookup"><span data-stu-id="1fa63-111">Specify the fixed asset charge code.</span></span>                         |
   | <span data-ttu-id="1fa63-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1fa63-112">**Description**</span></span>              | <span data-ttu-id="1fa63-113">Укажите описание издержки ОС.</span><span class="sxs-lookup"><span data-stu-id="1fa63-113">Specify the description of the fixed asset charge.</span></span>           |
   | <span data-ttu-id="1fa63-114">**Общая товарная группа**</span><span class="sxs-lookup"><span data-stu-id="1fa63-114">**Gen. Prod. Posting Group**</span></span> | <span data-ttu-id="1fa63-115">Определите общую товарную группу учета по умолчанию, которая будет использоваться для данного кода издержки ОС.</span><span class="sxs-lookup"><span data-stu-id="1fa63-115">Specify the default general product posting group that will be used for the fixed asset charge code.</span></span> |
   | <span data-ttu-id="1fa63-116">**Товарная группа НДС**</span><span class="sxs-lookup"><span data-stu-id="1fa63-116">**VAT Prod. Posting Group**</span></span>  | <span data-ttu-id="1fa63-117">Определите товарную группу учета НДС по умолчанию, которая будет использоваться для данного кода издержки ОС.</span><span class="sxs-lookup"><span data-stu-id="1fa63-117">Specify the default VAT product posting group that will be used for the fixed asset charge code.</span></span> |
   | <span data-ttu-id="1fa63-118">**Код глобального измерения 1**</span><span class="sxs-lookup"><span data-stu-id="1fa63-118">**Global Dimension 1 Code**</span></span>  | <span data-ttu-id="1fa63-119">Укажите код глобального измерения, связанного с издержками основного средства.</span><span class="sxs-lookup"><span data-stu-id="1fa63-119">Specify the global dimension code that is associated with the fixed asset charge.</span></span> |
   | <span data-ttu-id="1fa63-120">**Код глобального измерения 2**</span><span class="sxs-lookup"><span data-stu-id="1fa63-120">**Global Dimension 2 Code**</span></span>  | <span data-ttu-id="1fa63-121">Укажите код глобального измерения, связанного с издержками основного средства.</span><span class="sxs-lookup"><span data-stu-id="1fa63-121">Specify the global dimension code that is associated with the fixed asset charge.</span></span> |
   | <span data-ttu-id="1fa63-122">**Искл. стоимость для НУ**</span><span class="sxs-lookup"><span data-stu-id="1fa63-122">**Exclude Cost for TA**</span></span>      | <span data-ttu-id="1fa63-123">Укажите, нужно ли исключать издержку основного средства из налогового учета.</span><span class="sxs-lookup"><span data-stu-id="1fa63-123">Select if you want to exclude the fixed asset charge from tax accounting.</span></span> |
   | <span data-ttu-id="1fa63-124">**Счет ГК для ОС в эксплуатации**</span><span class="sxs-lookup"><span data-stu-id="1fa63-124">**G/L Acc. For Released FA**</span></span> | <span data-ttu-id="1fa63-125">Определите счет ГК для учета суммы издержек ОС при вводе основного средства в эксплуатацию.</span><span class="sxs-lookup"><span data-stu-id="1fa63-125">Specify the general ledger account to post the fixed asset charge amount to when the fixed asset is released.</span></span> |
   | <span data-ttu-id="1fa63-126">**Код налоговой разницы для ОС**</span><span class="sxs-lookup"><span data-stu-id="1fa63-126">**Tax Difference Code FA**</span></span>   | <span data-ttu-id="1fa63-127">Укажите код налоговой разницы, связанной с издержками основного средства.</span><span class="sxs-lookup"><span data-stu-id="1fa63-127">Specify the tax difference code that is associated with the fixed asset charge.</span></span> |

## <a name="see-also"></a><span data-ttu-id="1fa63-128">См. также</span><span class="sxs-lookup"><span data-stu-id="1fa63-128">See Also</span></span>

[<span data-ttu-id="1fa63-129">Настройка основных средств</span><span class="sxs-lookup"><span data-stu-id="1fa63-129">Setting Up Fixed Assets</span></span>](../../fa-setup.md)  
