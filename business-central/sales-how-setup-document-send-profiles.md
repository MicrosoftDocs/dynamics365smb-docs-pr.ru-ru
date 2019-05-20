---
title: Настройка предпочтительных способов отправки документов продажи | Документы Майкрософт
description: Описывается порядок настройки предпочитаемого способа отправки документов продажи, например электронная почта, PDF, электронные документы и т. д.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: email, PDF, electronic document
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: a6521a6f67fa39ded3b3baa863fc0d4341aa0524
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2019
ms.locfileid: "1252439"
---
# <a name="set-up-document-sending-profiles"></a><span data-ttu-id="09b73-103">Настройка профилей отправки документов</span><span class="sxs-lookup"><span data-stu-id="09b73-103">Set Up Document Sending Profiles</span></span>
<span data-ttu-id="09b73-104">Для каждого клиента можно настроить предпочтительный способ отправки документов продажи, так что не придется каждый раз выбирать вариант отправки при выборе действия **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="09b73-104">You can set each customer up with a preferred method of sending sales documents, so that you do not have to select a sending option every time you choose the **Post and Send** action.</span></span>

<span data-ttu-id="09b73-105">На странице **Профили отправки документов** можно настроить различные профили отправки, которые затем можно будет выбирать в поле **Профиль отправки документов** в карточке клиента.</span><span class="sxs-lookup"><span data-stu-id="09b73-105">On the **Document Sending Profiles** page, you set up different sending profiles that you can select from in the **Document Sending Profile** field on a customer card.</span></span> <span data-ttu-id="09b73-106">Вы можете установить флажок **По умолчанию**, чтобы указать, что профиль отправки документа является профилем по умолчанию для всех клиентов, кроме тех, у которых в поле **Профиль отправки документов** указан иной профиль.</span><span class="sxs-lookup"><span data-stu-id="09b73-106">You can select the **Default** check box to specify that the document sending profile is the default profile for all customers, except for customers where the **Document Sending Profile** field is filled with another sending profile.</span></span>

<span data-ttu-id="09b73-107">При выборе действия **Учесть и отправить** в документе продажи появляется диалоговое окно **Учесть и отправить подтверждение**, в котором отображается используемый профиль отправки — либо установленный для данного клиента, либо профиль по умолчанию для всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="09b73-107">When you choose the **Post and Send** action on a sales document, the **Post and Send Confirmation** dialog box shows the sending profile used, either the one set up for the customer or the default for all customers.</span></span> <span data-ttu-id="09b73-108">В этом диалоговом окне можно изменить профиль отправки для конкретного документа продаж.</span><span class="sxs-lookup"><span data-stu-id="09b73-108">In the dialog box, you can change the sending profile for the sales document.</span></span> <span data-ttu-id="09b73-109">Дополнительные сведения см. в разделе [Выставление счетов продажи](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="09b73-109">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span></span>

## <a name="to-set-up-a-document-sending-profile"></a><span data-ttu-id="09b73-110">Настройка профиля отправки документов</span><span class="sxs-lookup"><span data-stu-id="09b73-110">To set up a document sending profile</span></span>
1. <span data-ttu-id="09b73-111">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Профили отправки документов**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="09b73-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Document Sending Profiles**, and then choose the related link.</span></span>
2. <span data-ttu-id="09b73-112">На странице **Профили отправки документов** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="09b73-112">On the **Document Sending Profiles** page, choose the **New** action.</span></span>
3. <span data-ttu-id="09b73-113">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="09b73-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-specify-a-sending-profile-on-a-customer-card"></a><span data-ttu-id="09b73-114">Определение профиля отправки в карточке клиента</span><span class="sxs-lookup"><span data-stu-id="09b73-114">To specify a sending profile on a customer card</span></span>
1. <span data-ttu-id="09b73-115">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиенты**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="09b73-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="09b73-116">Откройте карточку клиента, для которого нужно настроить профиль отправки.</span><span class="sxs-lookup"><span data-stu-id="09b73-116">Open the card of the customer who you want to set up a sending profile for.</span></span>
3. <span data-ttu-id="09b73-117">В поле **Профиль отправки документов** выберите профиль, настроенный, как описано в предыдущей процедуре.</span><span class="sxs-lookup"><span data-stu-id="09b73-117">In the **Document Sending Profile** field, select a profile that you have set up as described in the previous procedure.</span></span>

## <a name="see-also"></a><span data-ttu-id="09b73-118">См. также</span><span class="sxs-lookup"><span data-stu-id="09b73-118">See Also</span></span>
[<span data-ttu-id="09b73-119">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="09b73-119">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="09b73-120">Продажи</span><span class="sxs-lookup"><span data-stu-id="09b73-120">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="09b73-121">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="09b73-121">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
