---
title: Создание карточек счетов кассы в России
description: Российские улучшения включают счета кассы.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2020
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 88e906f7911eb6409c0fdadce93b146bf95a72b8
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3180964"
---
# <a name="create-cash-account-cards"></a><span data-ttu-id="4c2c8-103">Создание карточек счетов кассы</span><span class="sxs-lookup"><span data-stu-id="4c2c8-103">Create Cash Account Cards</span></span>

<span data-ttu-id="4c2c8-104">Счета кассы похожи на банковские счета и создаются так же.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-104">Cash accounts are similar to bank accounts and are created identically.</span></span> <span data-ttu-id="4c2c8-105">Можно создать любое необходимое количество карточек счетов кассы.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-105">You can create as many cash account cards as needed.</span></span>

## <a name="to-create-a-cash-account-card"></a><span data-ttu-id="4c2c8-106">Создание карточек счетов кассы</span><span class="sxs-lookup"><span data-stu-id="4c2c8-106">To create a cash account card</span></span>

1. <span data-ttu-id="4c2c8-107">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Счета кассы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-107">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Cash Accounts**, and then choose the related link.</span></span>

2. <span data-ttu-id="4c2c8-108">В окне **Карточка кассы** на экспресс-вкладке **Учет** заполните поля, как описано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-108">In the **Cash Account Card** window, fill in the fields on the **Posting** FastTab as described in the following table.</span></span>

   | <span data-ttu-id="4c2c8-109">Поле</span><span class="sxs-lookup"><span data-stu-id="4c2c8-109">Field</span></span>                            | <span data-ttu-id="4c2c8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4c2c8-110">Description</span></span>                                                  |
   | :------------------------------- | :----------------------------------------------------------- |
   | <span data-ttu-id="4c2c8-111">**код валюты;**</span><span class="sxs-lookup"><span data-stu-id="4c2c8-111">**Currency Code**</span></span>                | <span data-ttu-id="4c2c8-112">Определяет код валюты, связанный со счетом кассы.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-112">Specifies the currency code that is associated with the cash account.</span></span> |
   | <span data-ttu-id="4c2c8-113">**Серия номеров приходных ордеров**</span><span class="sxs-lookup"><span data-stu-id="4c2c8-113">**Debit Cash Order No. Series**</span></span>  | <span data-ttu-id="4c2c8-114">Определяет серийные номера приходных кассовых ордеров.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-114">Specifies the serial numbers for outgoing cash orders.</span></span>       |
   | <span data-ttu-id="4c2c8-115">**Серия номеров расходных ордеров**</span><span class="sxs-lookup"><span data-stu-id="4c2c8-115">**Credit Cash Order No. Series**</span></span> | <span data-ttu-id="4c2c8-116">Определяет серийные номера расходных кассовых ордеров.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-116">Specifies the serial numbers for ingoing cash orders.</span></span>        |
   | <span data-ttu-id="4c2c8-117">**Номер последней страницы кассового отчета**</span><span class="sxs-lookup"><span data-stu-id="4c2c8-117">**Last Cash Report Page No.**</span></span>    | <span data-ttu-id="4c2c8-118">Определяет номер последней страницы напечатанного отчета "Лист Кассовой Книги".</span><span class="sxs-lookup"><span data-stu-id="4c2c8-118">Specifies the last printed cash additional sheet report page number.</span></span> |
   | <span data-ttu-id="4c2c8-119">**Банк. счет - учетная группа**</span><span class="sxs-lookup"><span data-stu-id="4c2c8-119">**Bank Acc. Posting Group**</span></span>      | <span data-ttu-id="4c2c8-120">Определяет учетную группу банковского счета, связанную со счетом кассы.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-120">Specifies the bank account posting group that is associated with the cash account.</span></span> |
   | <span data-ttu-id="4c2c8-121">**НДС (%) для документа**</span><span class="sxs-lookup"><span data-stu-id="4c2c8-121">**VAT % for Document**</span></span>           | <span data-ttu-id="4c2c8-122">Определяет процентную ставку для расчета НДС в документах банка или кассы.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-122">Specifies the VAT percentage for calculating VAT in cash or bank documents.</span></span> <span data-ttu-id="4c2c8-123">Эта ставка НДС не используется в расчетах при учете НДС.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-123">This VAT percentage is not used in VAT posting calculations.</span></span> |

3. <span data-ttu-id="4c2c8-124">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="4c2c8-124">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="4c2c8-125">См. также</span><span class="sxs-lookup"><span data-stu-id="4c2c8-125">See Also</span></span>

[<span data-ttu-id="4c2c8-126">Управление мелкими доходами/расходами</span><span class="sxs-lookup"><span data-stu-id="4c2c8-126">Petty Cash Management</span></span>](Petty-Cash-Management.md)  
[<span data-ttu-id="4c2c8-127">Управление банками и кассами</span><span class="sxs-lookup"><span data-stu-id="4c2c8-127">Bank and Cash Management</span></span>](bank-and-cash-management.md)  
