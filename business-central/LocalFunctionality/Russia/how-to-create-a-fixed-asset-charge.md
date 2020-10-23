---
title: Создание издержек основных средств в России
description: Российские улучшения включают издержки ОС.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: d37b351de0181e197be072b7f2594f762599ea9d
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3921248"
---
# <a name="create-a-fixed-asset-charge"></a><span data-ttu-id="45015-103">Создание издержек ОС</span><span class="sxs-lookup"><span data-stu-id="45015-103">Create a Fixed Asset Charge</span></span>

<span data-ttu-id="45015-104">Ниже показано, как создать новые издержки основного средства.</span><span class="sxs-lookup"><span data-stu-id="45015-104">The following procedure shows how to create a new fixed asset charge.</span></span> 

## <a name="to-create-a-fixed-asset-charge"></a><span data-ttu-id="45015-105">Создание издержек ОС</span><span class="sxs-lookup"><span data-stu-id="45015-105">To create a fixed asset charge</span></span>

1. <span data-ttu-id="45015-106">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Карточка издержки ОС**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="45015-106">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Charge Card**, and then choose the related link.</span></span>

2. <span data-ttu-id="45015-107">На экспресс-вкладке **Общее** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="45015-107">On the **General** FastTab, fill in the fields as described in the following table.</span></span>

   | <span data-ttu-id="45015-108">Поле</span><span class="sxs-lookup"><span data-stu-id="45015-108">Field</span></span>                        | <span data-ttu-id="45015-109">Описание</span><span class="sxs-lookup"><span data-stu-id="45015-109">Description</span></span>                                                  |
   | :--------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="45015-110">**Номер**</span><span class="sxs-lookup"><span data-stu-id="45015-110">**No.**</span></span>                      | <span data-ttu-id="45015-111">Укажите код издержки основного средства.</span><span class="sxs-lookup"><span data-stu-id="45015-111">Specify the fixed asset charge code.</span></span>                         |
   | <span data-ttu-id="45015-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="45015-112">**Description**</span></span>              | <span data-ttu-id="45015-113">Укажите описание издержки ОС.</span><span class="sxs-lookup"><span data-stu-id="45015-113">Specify the description of the fixed asset charge.</span></span>           |
   | <span data-ttu-id="45015-114">**Общая товарная группа**</span><span class="sxs-lookup"><span data-stu-id="45015-114">**Gen. Prod. Posting Group**</span></span> | <span data-ttu-id="45015-115">Определите общую товарную группу учета по умолчанию, которая будет использоваться для данного кода издержки ОС.</span><span class="sxs-lookup"><span data-stu-id="45015-115">Specify the default general product posting group that will be used for the fixed asset charge code.</span></span> |
   | <span data-ttu-id="45015-116">**Товарная группа НДС**</span><span class="sxs-lookup"><span data-stu-id="45015-116">**VAT Prod. Posting Group**</span></span>  | <span data-ttu-id="45015-117">Определите товарную группу учета НДС по умолчанию, которая будет использоваться для данного кода издержки ОС.</span><span class="sxs-lookup"><span data-stu-id="45015-117">Specify the default VAT product posting group that will be used for the fixed asset charge code.</span></span> |
   | <span data-ttu-id="45015-118">**Код глобального измерения 1**</span><span class="sxs-lookup"><span data-stu-id="45015-118">**Global Dimension 1 Code**</span></span>  | <span data-ttu-id="45015-119">Укажите код глобального измерения, связанного с издержками основного средства.</span><span class="sxs-lookup"><span data-stu-id="45015-119">Specify the global dimension code that is associated with the fixed asset charge.</span></span> |
   | <span data-ttu-id="45015-120">**Код глобального измерения 2**</span><span class="sxs-lookup"><span data-stu-id="45015-120">**Global Dimension 2 Code**</span></span>  | <span data-ttu-id="45015-121">Укажите код глобального измерения, связанного с издержками основного средства.</span><span class="sxs-lookup"><span data-stu-id="45015-121">Specify the global dimension code that is associated with the fixed asset charge.</span></span> |
   | <span data-ttu-id="45015-122">**Искл. стоимость для НУ**</span><span class="sxs-lookup"><span data-stu-id="45015-122">**Exclude Cost for TA**</span></span>      | <span data-ttu-id="45015-123">Укажите, нужно ли исключать издержку основного средства из налогового учета.</span><span class="sxs-lookup"><span data-stu-id="45015-123">Select if you want to exclude the fixed asset charge from tax accounting.</span></span> |
   | <span data-ttu-id="45015-124">**Счет ГК для ОС в эксплуатации**</span><span class="sxs-lookup"><span data-stu-id="45015-124">**G/L Acc. For Released FA**</span></span> | <span data-ttu-id="45015-125">Определите счет ГК для учета суммы издержек ОС при вводе основного средства в эксплуатацию.</span><span class="sxs-lookup"><span data-stu-id="45015-125">Specify the general ledger account to post the fixed asset charge amount to when the fixed asset is released.</span></span> |
   | <span data-ttu-id="45015-126">**Код налоговой разницы для ОС**</span><span class="sxs-lookup"><span data-stu-id="45015-126">**Tax Difference Code FA**</span></span>   | <span data-ttu-id="45015-127">Укажите код налоговой разницы, связанной с издержками основного средства.</span><span class="sxs-lookup"><span data-stu-id="45015-127">Specify the tax difference code that is associated with the fixed asset charge.</span></span> |

## <a name="see-also"></a><span data-ttu-id="45015-128">См. также</span><span class="sxs-lookup"><span data-stu-id="45015-128">See Also</span></span>

[<span data-ttu-id="45015-129">Настройка основных средств</span><span class="sxs-lookup"><span data-stu-id="45015-129">Setting Up Fixed Assets</span></span>](../../fa-setup.md)  
