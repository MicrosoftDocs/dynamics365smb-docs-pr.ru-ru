---
title: Настройка предпочтительных способов отправки документов продажи | Документация Майкрософт
description: Описывается порядок настройки предпочитаемого способа отправки документов продажи, например электронная почта, PDF, электронные документы и т. д.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: email, PDF, electronic document
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 18f9fdf997608cc75fbf2736cc7a834787a8b414
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5387573"
---
# <a name="set-up-document-sending-profiles"></a><span data-ttu-id="4653b-103">Настройка профилей отправки документов</span><span class="sxs-lookup"><span data-stu-id="4653b-103">Set Up Document Sending Profiles</span></span>
<span data-ttu-id="4653b-104">Для каждого клиента можно настроить предпочтительный способ отправки документов продажи, так что не придется каждый раз выбирать вариант отправки при выборе действия **Учесть и отправить**.</span><span class="sxs-lookup"><span data-stu-id="4653b-104">You can set each customer up with a preferred method of sending sales documents, so that you do not have to select a sending option every time you choose the **Post and Send** action.</span></span>

<span data-ttu-id="4653b-105">На странице **Профили отправки документов** можно настроить различные профили отправки, которые затем можно будет выбирать в поле **Профиль отправки документов** в карточке клиента.</span><span class="sxs-lookup"><span data-stu-id="4653b-105">On the **Document Sending Profiles** page, you set up different sending profiles that you can select from in the **Document Sending Profile** field on a customer card.</span></span> <span data-ttu-id="4653b-106">Вы можете установить флажок **По умолчанию**, чтобы указать, что профиль отправки документа является профилем по умолчанию для всех клиентов, кроме тех, у которых в поле **Профиль отправки документов** указан иной профиль.</span><span class="sxs-lookup"><span data-stu-id="4653b-106">You can select the **Default** check box to specify that the document sending profile is the default profile for all customers, except for customers where the **Document Sending Profile** field is filled with another sending profile.</span></span>

<span data-ttu-id="4653b-107">При выборе действия **Учесть и отправить** в документе продажи появляется диалоговое окно **Учесть и отправить подтверждение**, в котором отображается используемый профиль отправки — либо установленный для данного клиента, либо профиль по умолчанию для всех клиентов.</span><span class="sxs-lookup"><span data-stu-id="4653b-107">When you choose the **Post and Send** action on a sales document, the **Post and Send Confirmation** dialog box shows the sending profile used, either the one set up for the customer or the default for all customers.</span></span> <span data-ttu-id="4653b-108">В этом диалоговом окне можно изменить профиль отправки для конкретного документа продаж.</span><span class="sxs-lookup"><span data-stu-id="4653b-108">In the dialog box, you can change the sending profile for the sales document.</span></span> <span data-ttu-id="4653b-109">Дополнительные сведения см. в разделе [Выставление счетов продажи](sales-how-invoice-sales.md).</span><span class="sxs-lookup"><span data-stu-id="4653b-109">For more information, see [Invoice Sales](sales-how-invoice-sales.md).</span></span>
<br><br>  

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4jzHH?rel=0]

## <a name="to-set-up-a-document-sending-profile"></a><span data-ttu-id="4653b-110">Настройка профиля отправки документов</span><span class="sxs-lookup"><span data-stu-id="4653b-110">To set up a document sending profile</span></span>
1. <span data-ttu-id="4653b-111">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Профили отправки документов**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="4653b-111">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Document Sending Profiles**, and then choose the related link.</span></span>
2. <span data-ttu-id="4653b-112">На странице **Профили отправки документов** выберите действие **Создать**.</span><span class="sxs-lookup"><span data-stu-id="4653b-112">On the **Document Sending Profiles** page, choose the **New** action.</span></span>
3. <span data-ttu-id="4653b-113">Заполните соответствующим образом поля.</span><span class="sxs-lookup"><span data-stu-id="4653b-113">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-specify-a-sending-profile-on-a-customer-card"></a><span data-ttu-id="4653b-114">Определение профиля отправки в карточке клиента</span><span class="sxs-lookup"><span data-stu-id="4653b-114">To specify a sending profile on a customer card</span></span>
1. <span data-ttu-id="4653b-115">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиенты**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="4653b-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="4653b-116">Откройте карточку клиента, для которого нужно настроить профиль отправки.</span><span class="sxs-lookup"><span data-stu-id="4653b-116">Open the card of the customer who you want to set up a sending profile for.</span></span>
3. <span data-ttu-id="4653b-117">В поле **Профиль отправки документов** выберите профиль, настроенный, как описано в предыдущей процедуре.</span><span class="sxs-lookup"><span data-stu-id="4653b-117">In the **Document Sending Profile** field, select a profile that you have set up as described in the previous procedure.</span></span>

## <a name="see-also"></a><span data-ttu-id="4653b-118">См. также</span><span class="sxs-lookup"><span data-stu-id="4653b-118">See Also</span></span>
[<span data-ttu-id="4653b-119">Настройка продаж</span><span class="sxs-lookup"><span data-stu-id="4653b-119">Setting Up Sales</span></span>](sales-setup-sales.md)  
[<span data-ttu-id="4653b-120">Продажи</span><span class="sxs-lookup"><span data-stu-id="4653b-120">Sales</span></span>](sales-manage-sales.md)  
<span data-ttu-id="4653b-121">[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4653b-121">[Working with [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)</span></span>


[!INCLUDE[footer-include](includes/footer-banner.md)]