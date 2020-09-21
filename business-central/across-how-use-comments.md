---
title: Добавление комментариев к картам и документам | Документация Майкрософт
description: Добавление дополнительной информации в счета, карты клиентов или заказы на продажу для сообщения о соглашениях, таких как особая цена или метод доставки, другим пользователям.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: tasks, work
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: f1127bd8e99f8ef6342ec240b4f42b52b11b36bb
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/09/2020
ms.locfileid: "3781889"
---
# <a name="add-comments-to-cards-and-documents"></a><span data-ttu-id="5be50-103">Добавление комментариев к картам и документам</span><span class="sxs-lookup"><span data-stu-id="5be50-103">Add Comments to Cards and Documents</span></span>
<span data-ttu-id="5be50-104">Можно добавить дополнительную информацию в счета ГК, карты клиентов или заказы на продажу для сообщения об исключениях или особых соглашениях для других пользователей.</span><span class="sxs-lookup"><span data-stu-id="5be50-104">You can add extra information to G/L accounts, customers cards, or sales orders to communicate exceptions or special agreements to other users.</span></span>
<span data-ttu-id="5be50-105">Практически все карты и документы имеют действие **Комментарии**, которые открывают страницу **Лист комментариев**, в котором можно вводить или читать комментарии.</span><span class="sxs-lookup"><span data-stu-id="5be50-105">Practically all cards and document have a **Comments** action, which opens the **Comment Sheet** page where you can write or read comments.</span></span> <span data-ttu-id="5be50-106">В документах можно также добавить комментарии к отдельным строкам.</span><span class="sxs-lookup"><span data-stu-id="5be50-106">On documents, you can also add comments to individual lines.</span></span>

<span data-ttu-id="5be50-107">Комментарии в текущих документах переносятся в связанный учтенный документ.</span><span class="sxs-lookup"><span data-stu-id="5be50-107">Comments on ongoing documents are transferred to the related posted document.</span></span> <span data-ttu-id="5be50-108">Комментарий, например, в заказе на продажу переносится в соответствующую учтенную отгрузку продажи.</span><span class="sxs-lookup"><span data-stu-id="5be50-108">For example, a comment on a sales order is transferred to a resulting posted sales shipment.</span></span>

<span data-ttu-id="5be50-109">Кроме того, можно указать, требуется ли, чтобы комментарии перемещались с одного типа документов в другой итоговый тип документа, например из заказа на продажу в счет продажи.</span><span class="sxs-lookup"><span data-stu-id="5be50-109">In addition, you can specify if you want comments to be transferred from one type of document to another resulting type of document, such as from a sales order to a sales invoice.</span></span> <span data-ttu-id="5be50-110">Это выполняется на страницах **Продажи и расчеты с дебиторами** и **Покупки и расчеты с кредиторами**, соответственно.</span><span class="sxs-lookup"><span data-stu-id="5be50-110">You do this in the **Sales & Receivables** and the **Purchases & Payables** pages respectively.</span></span>

> [!NOTE]
> <span data-ttu-id="5be50-111">Комментарии не печатаются и не выводятся в отчеты или внешние документы.</span><span class="sxs-lookup"><span data-stu-id="5be50-111">Comments are not printed or output to reports or externally-facing documents.</span></span>

<span data-ttu-id="5be50-112">Ниже описано, как добавить комментарий в карточку товара.</span><span class="sxs-lookup"><span data-stu-id="5be50-112">The following describes how to add a comment to an item card.</span></span> <span data-ttu-id="5be50-113">Шаги аналогичны для всех остальных карт и документов, за исключением строк документа, для которых действие **Комментарии** находится в меню действий строки.</span><span class="sxs-lookup"><span data-stu-id="5be50-113">The steps are similar for all other cards and documents, except on document lines, the **Comments** action is placed on a lines action menu.</span></span>

## <a name="to-add-a-comments-to-an-item-card"></a><span data-ttu-id="5be50-114">Для добавления комментариев в карточку товара</span><span class="sxs-lookup"><span data-stu-id="5be50-114">To add a comments to an item card</span></span>
1. <span data-ttu-id="5be50-115">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="5be50-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items**, and then choose the related link.</span></span>
2. <span data-ttu-id="5be50-116">Откройте соответствующую карточку товара.</span><span class="sxs-lookup"><span data-stu-id="5be50-116">Open the relevant item card.</span></span>
3. <span data-ttu-id="5be50-117">Выберите действие **Комментарии**.</span><span class="sxs-lookup"><span data-stu-id="5be50-117">Choose the **Comments** action.</span></span>
4. <span data-ttu-id="5be50-118">На странице **Лист комментариев** можно ввести любой текст, затем выбрать кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="5be50-118">On the **Comment Sheet** page, enter any text, and then choose the **OK** button.</span></span>

## <a name="see-also"></a><span data-ttu-id="5be50-119">См. также</span><span class="sxs-lookup"><span data-stu-id="5be50-119">See Also</span></span>
<span data-ttu-id="5be50-120">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5be50-120">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="5be50-121">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="5be50-121">General Business Functionality</span></span>](ui-across-business-areas.md)
