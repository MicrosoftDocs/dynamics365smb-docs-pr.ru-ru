---
title: Назначение уровня приоритета поставщику | Документация Майкрософт
description: Вы можете назначать номера поставщика для их приоритизации и поддержки функции предложений платежей в Business Central.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier, payment priority
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 2586e9a5af338bee79bf73b494a7a653b6bfc2f2
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2312536"
---
# <a name="prioritize-vendors"></a><span data-ttu-id="dccec-103">Назначение приоритетов поставщикам</span><span class="sxs-lookup"><span data-stu-id="dccec-103">Prioritize Vendors</span></span>
<span data-ttu-id="dccec-104">В [!INCLUDE[d365fin](includes/d365fin_md.md)] предлагаются различные виды оплат поставщикам, например оплаты, которые должны быть произведены быстро, или оплаты, для которых возможны скидки.</span><span class="sxs-lookup"><span data-stu-id="dccec-104">[!INCLUDE[d365fin](includes/d365fin_md.md)] can suggest various payments to vendors, for example, payments that will be due soon or payments where a discount is available.</span></span> <span data-ttu-id="dccec-105">Дополнительные сведения см. в разделе [Предложение оплаты поставщикам](payables-how-suggest-vendor-payments.md).</span><span class="sxs-lookup"><span data-stu-id="dccec-105">For more information, see [Suggest Vendor Payments](payables-how-suggest-vendor-payments.md).</span></span>

<span data-ttu-id="dccec-106">Во-первых, следует назначить приоритеты поставщикам путем назначения им номеров.</span><span class="sxs-lookup"><span data-stu-id="dccec-106">First, you must prioritize your vendors by assigning numbers to them.</span></span>

## <a name="to-prioritize-vendors"></a><span data-ttu-id="dccec-107">Назначение приоритета поставщикам</span><span class="sxs-lookup"><span data-stu-id="dccec-107">To prioritize vendors</span></span>
1. <span data-ttu-id="dccec-108">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Поставщики**, а затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="dccec-108">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span></span>
2. <span data-ttu-id="dccec-109">Выберите соответствующего поставщика, а затем выберите **Правка**.</span><span class="sxs-lookup"><span data-stu-id="dccec-109">Select the relevant vendor, and then choose **Edit**.</span></span>
3. <span data-ttu-id="dccec-110">В поле **Приоритет** введите номер.</span><span class="sxs-lookup"><span data-stu-id="dccec-110">In the **Priority** field, enter a number.</span></span>

<span data-ttu-id="dccec-111">В [!INCLUDE[d365fin](includes/d365fin_md.md)] самый нижний номер (за исключением 0) рассматривается как номер с наивысшим приоритетом.</span><span class="sxs-lookup"><span data-stu-id="dccec-111">[!INCLUDE[d365fin](includes/d365fin_md.md)] considers the lowest number, except 0, to have the highest priority.</span></span> <span data-ttu-id="dccec-112">Так, например, если используются 1, 2 и 3, то 1 будет иметь наивысший приоритет.</span><span class="sxs-lookup"><span data-stu-id="dccec-112">So, for example, if you use 1, 2, and 3, then 1 will have the highest priority.</span></span>

<span data-ttu-id="dccec-113">Если назначать приоритет для поставщика не требуется, оставьте поле **Приоритет** пустым.</span><span class="sxs-lookup"><span data-stu-id="dccec-113">If you do not want to prioritize a vendor, leave the **Priority** field blank.</span></span> <span data-ttu-id="dccec-114">В случае же использования средства предложения с учетом приоритетов, поставщик, с пустым полем "Приоритет", будет числиться после всех поставщиков, которые имеют номер приоритета.</span><span class="sxs-lookup"><span data-stu-id="dccec-114">Then, if you use the payment suggestion feature, the vendor will be listed after all the vendors that have a priority number.</span></span> <span data-ttu-id="dccec-115">В случае необходимости можно вводить столько уровней приоритета, сколько требуется.</span><span class="sxs-lookup"><span data-stu-id="dccec-115">You can enter as many priority levels as necessary.</span></span>

## <a name="see-also"></a><span data-ttu-id="dccec-116">См. также</span><span class="sxs-lookup"><span data-stu-id="dccec-116">See Also</span></span>
[<span data-ttu-id="dccec-117">Настройка покупки</span><span class="sxs-lookup"><span data-stu-id="dccec-117">Setting Up Purchasing</span></span>](purchasing-setup-purchasing.md)  
[<span data-ttu-id="dccec-118">Управление кредиторской задолженностью</span><span class="sxs-lookup"><span data-stu-id="dccec-118">Managing Payables</span></span>](payables-manage-payables.md)  
<span data-ttu-id="dccec-119">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="dccec-119">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
