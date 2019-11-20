---
title: Малоценные основные средства в России
description: Российские усовершенствования включают управление основными средствами, которые нельзя амортизировать.
author: DianaMalina
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2019
ms.reviewer: edupont
ms.author: soalex
ms.openlocfilehash: 46a4691a6f3c0d13f51823bfffff022b7de80989
ms.sourcegitcommit: 319023e53627dbe8e68643908aacc6fd594a4957
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/04/2019
ms.locfileid: "2554581"
---
# <a name="undepreciable-fixed-assets"></a><span data-ttu-id="02425-103">Малоценные основные средства</span><span class="sxs-lookup"><span data-stu-id="02425-103">Undepreciable Fixed Assets</span></span>

<span data-ttu-id="02425-104">Функция малоценных основных средств позволяет списывать для основных средств всю сумму, за которую они были приобретены, в момент ввода в эксплуатацию.</span><span class="sxs-lookup"><span data-stu-id="02425-104">The undepreciable fixed assets feature enables you to repay fixed assets with the whole amount of their acquisition at the time of their release.</span></span> <span data-ttu-id="02425-105">Кроме того, автоматически создаются записи количеств для этих основных средств, чтобы хранить записи о существовании и движении этих ОС в терминах количества.</span><span class="sxs-lookup"><span data-stu-id="02425-105">It also automatically creates quantity records for these fixed assets in order to keep records of their existence and movements in quantitative terms.</span></span>  

<span data-ttu-id="02425-106">Создайте книгу амортизации для хранения записей количеств основных средств, для которых во время ввода в эксплуатацию будет списываться сумма, по которой они приобретены.</span><span class="sxs-lookup"><span data-stu-id="02425-106">Create a depreciation book to keep records of the quantities of fixed assets that will be repaid at the time of release for the amount that they were acquired for.</span></span> <span data-ttu-id="02425-107">Дополнительные сведения см. в разделе [Настройка книги количественного учета](How-to-Set-Up-a-Quantity-Book.md).</span><span class="sxs-lookup"><span data-stu-id="02425-107">For more information, see [Set Up a Quantity Book](How-to-Set-Up-a-Quantity-Book.md).</span></span>  

## <a name="to-set-up-an-undepreciable-fixed-asset"></a><span data-ttu-id="02425-108">Настройка малоценного основного средства</span><span class="sxs-lookup"><span data-stu-id="02425-108">To set up an undepreciable fixed asset</span></span>

1. <span data-ttu-id="02425-109">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Основные средства**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="02425-109">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Fixed Assets**, and then choose the related link.</span></span>

2. <span data-ttu-id="02425-110">В окне **Карточка основного средства** на экспресс-вкладке **Амортизация** выберите поле **Неамортизируемое ОС**.</span><span class="sxs-lookup"><span data-stu-id="02425-110">In the **Fixed Asset Card** window, on the **Depreciation** FastTab, select the **Undepreciable FA** field.</span></span>

3. <span data-ttu-id="02425-111">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="02425-111">Choose the **OK** button.</span></span>

## <a name="to-create-a-purchase-order-for-an-undepreciable-fixed-asset"></a><span data-ttu-id="02425-112">Создание заказа на покупку для малоценного основного средства</span><span class="sxs-lookup"><span data-stu-id="02425-112">To create a purchase order for an undepreciable fixed asset</span></span>

1. <span data-ttu-id="02425-113">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказ на покупку**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="02425-113">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Order**, and then choose the related link.</span></span>
2. <span data-ttu-id="02425-114">Выберите действие **Учет**.</span><span class="sxs-lookup"><span data-stu-id="02425-114">Choose the **Post** action.</span></span>
3. <span data-ttu-id="02425-115">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="02425-115">Choose the **OK** button.</span></span>

## <a name="to-create-a-release-order-for-an-undepreciable-fixed-asset"></a><span data-ttu-id="02425-116">Создание заказа на ввод в эксплуатацию для малоценного основного средства</span><span class="sxs-lookup"><span data-stu-id="02425-116">To create a release order for an undepreciable fixed asset</span></span>

1. <span data-ttu-id="02425-117">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](../../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Акты ввода в эксплуатацию ОС**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="02425-117">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **FA Releases**, and then choose the related link.</span></span>
2. <span data-ttu-id="02425-118">Откройте акт ввода.</span><span class="sxs-lookup"><span data-stu-id="02425-118">Open a release.</span></span>
3. <span data-ttu-id="02425-119">В окне **Акт ввода в эксплуатацию ОС** выберите действие **Учесть**.</span><span class="sxs-lookup"><span data-stu-id="02425-119">In the **FA Release Act** window, choose the **Post** action.</span></span>
4. <span data-ttu-id="02425-120">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="02425-120">Choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="02425-121">См. также</span><span class="sxs-lookup"><span data-stu-id="02425-121">See Also</span></span>

[<span data-ttu-id="02425-122">Основные Средства</span><span class="sxs-lookup"><span data-stu-id="02425-122">Fixed Assets</span></span>](../../fa-manage.md)  
