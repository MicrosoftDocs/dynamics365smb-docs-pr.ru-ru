---
title: Редактирование учтенных документов о продажах и покупке | Документация Майкрософт
description: Узнайте о различных функциях учета для учета документов о покупке, а также о том, как можно обновлять учтенные документы.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.reviewer: edupont
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 6fbb4e458b0e4f9068b234748a3921dbca6b3222
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2300597"
---
# <a name="edit-posted-documents"></a><span data-ttu-id="f0c26-103">Изменение учтенных документов</span><span class="sxs-lookup"><span data-stu-id="f0c26-103">Edit Posted Documents</span></span>
<span data-ttu-id="f0c26-104">Иногда вам нужно обновить учтенный документ, потому что изменилась информация, относящаяся к документу.</span><span class="sxs-lookup"><span data-stu-id="f0c26-104">Sometimes you have to update a posted document because information that is relevant to the document has changed.</span></span> <span data-ttu-id="f0c26-105">Например, в учтенном документе продажи это может быть номер для отслеживания посылки агентом по доставке.</span><span class="sxs-lookup"><span data-stu-id="f0c26-105">On a posted sales document, this can be the shipping agent's package tracking number, for example.</span></span> <span data-ttu-id="f0c26-106">В учтенном документе покупки это может быть текст ссылки на платеж.</span><span class="sxs-lookup"><span data-stu-id="f0c26-106">On a posted purchase document, this can be a payment reference text.</span></span>

<span data-ttu-id="f0c26-107">Вы вносите изменения в редактируемую версию исходного документа, обозначенную текстом "**- Обновить**" в заголовке страницы.</span><span class="sxs-lookup"><span data-stu-id="f0c26-107">You perform the change on an editable version of the original document, indicated by "**- Update**" in the page title.</span></span> <span data-ttu-id="f0c26-108">Страница содержит подмножество полей исходного документа, некоторые из которых являются нередактируемыми полями, которые показаны только для информации.</span><span class="sxs-lookup"><span data-stu-id="f0c26-108">The page contains a subset of the fields on the original document, of which some are non-editable fields that are shown for information only.</span></span>

<span data-ttu-id="f0c26-109">Функциональность доступна для следующих документов в версиях для всех стран:</span><span class="sxs-lookup"><span data-stu-id="f0c26-109">The functionality is available for the following documents in all country versions:</span></span>
- <span data-ttu-id="f0c26-110">Учтенная расходная накладная продажи</span><span class="sxs-lookup"><span data-stu-id="f0c26-110">Posted Sales Shipment</span></span>
- <span data-ttu-id="f0c26-111">Учтенный счет покупки</span><span class="sxs-lookup"><span data-stu-id="f0c26-111">Posted Purchase Invoice</span></span>
- <span data-ttu-id="f0c26-112">Учтенная возвратная расходная накладная</span><span class="sxs-lookup"><span data-stu-id="f0c26-112">Posted Return Shipment</span></span>
- <span data-ttu-id="f0c26-113">Учтенные возвратные приходные накладные</span><span class="sxs-lookup"><span data-stu-id="f0c26-113">Posted Return Receipt</span></span>

<span data-ttu-id="f0c26-114">Следующие дополнительные документы могут быть отредактированы в версиях для выбранной страны:</span><span class="sxs-lookup"><span data-stu-id="f0c26-114">The following additional documents can be edited in selected country versions:</span></span>
- <span data-ttu-id="f0c26-115">ES: учтенный счет продажи, учтенная кредит-нота продажи, учтенная кредит-нота покупки</span><span class="sxs-lookup"><span data-stu-id="f0c26-115">ES: Posted Sales Invoice, Posted Sales Credit Memo, Posted Purchase Credit Memo</span></span>
- <span data-ttu-id="f0c26-116">APAC: учтенная кредит-нота продажи, учтенная кредит-нота покупки</span><span class="sxs-lookup"><span data-stu-id="f0c26-116">APAC: Posted Sales Credit Memo, Posted Purchase Credit Memo</span></span>
- <span data-ttu-id="f0c26-117">RU: учтенная кредит-нота продажи</span><span class="sxs-lookup"><span data-stu-id="f0c26-117">RU: Posted Sales Credit Memo</span></span>
- <span data-ttu-id="f0c26-118">IT: учтенная расходная накладная на перемещение, учтенная сервисная расходная накладная</span><span class="sxs-lookup"><span data-stu-id="f0c26-118">IT: Posted Transfer Shipment, Posted Service Shipment</span></span>

## <a name="to-edit-a-posted-sales-shipment"></a><span data-ttu-id="f0c26-119">Чтобы отредактировать учтенную расходную накладную продажи</span><span class="sxs-lookup"><span data-stu-id="f0c26-119">To edit a posted sales shipment</span></span>
<span data-ttu-id="f0c26-120">Далее поясняется, как редактировать учтенную расходную накладную продажи.</span><span class="sxs-lookup"><span data-stu-id="f0c26-120">The following explains how to edit a posted sales shipment.</span></span> <span data-ttu-id="f0c26-121">Шаги аналогичны для других поддерживаемых документов.</span><span class="sxs-lookup"><span data-stu-id="f0c26-121">The steps are similar for the other supported documents.</span></span>

1. <span data-ttu-id="f0c26-122">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Учтенные расходные накладные продажи**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="f0c26-122">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Posted Sales Shipments**, and then choose the related link.</span></span>
2. <span data-ttu-id="f0c26-123">Выберите документ, который требуется изменить, затем выберите действие **Обновить документ**.</span><span class="sxs-lookup"><span data-stu-id="f0c26-123">Select the document that you want to edit, and then choose the **Update Document** action.</span></span> <span data-ttu-id="f0c26-124">Либо откройте документ, затем выберите действие.</span><span class="sxs-lookup"><span data-stu-id="f0c26-124">Alternatively, open the document and then choose the action.</span></span>
3. <span data-ttu-id="f0c26-125">На странице **Учт. расх. накладная продажи - обновление** измените поле **Номер трасс. посылки**,</span><span class="sxs-lookup"><span data-stu-id="f0c26-125">On the **Posted Sales Shipment - Update** page, edit the **Package Tracking No.**</span></span> <span data-ttu-id="f0c26-126">например.</span><span class="sxs-lookup"><span data-stu-id="f0c26-126">field, for example.</span></span>
4. <span data-ttu-id="f0c26-127">Нажмите кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="f0c26-127">Choose the **OK** button.</span></span>

<span data-ttu-id="f0c26-128">Учтенная расходная накладная продажи обновлена.</span><span class="sxs-lookup"><span data-stu-id="f0c26-128">The posted sales shipment is updated.</span></span>

## <a name="see-also"></a><span data-ttu-id="f0c26-129">См. также</span><span class="sxs-lookup"><span data-stu-id="f0c26-129">See Also</span></span>
[<span data-ttu-id="f0c26-130">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="f0c26-130">General Business Functionality</span></span>](ui-across-business-areas.md)  
[<span data-ttu-id="f0c26-131">Покупки</span><span class="sxs-lookup"><span data-stu-id="f0c26-131">Purchasing</span></span>](purchasing-manage-purchasing.md)  
[<span data-ttu-id="f0c26-132">Учет документов и журналов</span><span class="sxs-lookup"><span data-stu-id="f0c26-132">Posting Documents and Journals</span></span>](ui-post-documents-journals.md)  
<span data-ttu-id="f0c26-133">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f0c26-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>