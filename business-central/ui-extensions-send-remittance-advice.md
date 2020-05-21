---
title: Расширение отправки авизо | Документация Майкрософт
description: Описывается расширение отправки авизо, которое позволяет отправить по электронной почте и повторно отправить авизо из журнала платежей и операций книги поставщиков.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, remittance, advice
ms.date: 05/05/2020
ms.author: edupont
ms.openlocfilehash: 236cb83e99c2385edc09622255037a152bf41e6e
ms.sourcegitcommit: 57e31a8b92feeaf8c6c63eba147f36b38eee7679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2020
ms.locfileid: "3339926"
---
# <a name="send-remittance-advice"></a><span data-ttu-id="9d634-103">Отправить авизо</span><span class="sxs-lookup"><span data-stu-id="9d634-103">Send Remittance Advice</span></span>

<span data-ttu-id="9d634-104">Если авизо используется для уведомления поставщиков о произведенных платежах, теперь можно использовать массовую рассылку авизо по электронной почте из журнала платежей, а также повторно отправлять авизо после выполнения платежей из операций книги поставщиков с помощью профилей отправки документов.</span><span class="sxs-lookup"><span data-stu-id="9d634-104">Where remittance advice is used to notify vendors of payments being made, you can now email remittance advice in bulk from the payment journal as well as resend after payments are made from vendor ledger entries by using document sending profiles.</span></span>

> [!NOTE]
> <span data-ttu-id="9d634-105">Эта функция поддерживается только в Business Central Online и On-Premises в следующих странах: Великобритания, США, Канада, Австралия, Новая Зеландия и Южная Африка.</span><span class="sxs-lookup"><span data-stu-id="9d634-105">This functionality is only supported in Business Central online and on-premises in following countries: United Kingdom, United States, Canada, Australia, New Zealand, and South Africa.</span></span>  

<span data-ttu-id="9d634-106">Авизо можно отправить двумя разными способами:</span><span class="sxs-lookup"><span data-stu-id="9d634-106">You can send remittance advice in two different ways:</span></span>

* <span data-ttu-id="9d634-107">На странице **Журнал платежей**, выберите **Навигация**, **Платежи**, **Отправить авизо**, чтобы отправить по электронной почте авизо для одной или нескольких строк журнала платежей поставщикам</span><span class="sxs-lookup"><span data-stu-id="9d634-107">In the **Payment Journal** page, choose **Navigate**, **Payments**, **Send Remittance Advice** to email remittance advice for one or multiple payment journal lines</span></span>
* <span data-ttu-id="9d634-108">На странице **Книга операций по поставщикам** выберите **Действия**, **Функции**, **Отправить авизо**, чтобы отправить авизо по электронной почте после учета платежей поставщикам для одной или нескольких операций книги поставщиков</span><span class="sxs-lookup"><span data-stu-id="9d634-108">In the **Vendor Ledger Entries** page, choose **Actions**, **Functions**, **Send Remittance Advice** to email remittance advice after posting of vendor payments, for one or multiple vendor ledger entries</span></span>

## <a name="see-also"></a><span data-ttu-id="9d634-109">См. также</span><span class="sxs-lookup"><span data-stu-id="9d634-109">See Also</span></span>

[<span data-ttu-id="9d634-110">Предлож. оплаты поставщикам</span><span class="sxs-lookup"><span data-stu-id="9d634-110">Suggest Vendor Payments</span></span>](payables-how-suggest-vendor-payments.md)  
<span data-ttu-id="9d634-111">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="9d634-111">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)</span></span>  
<span data-ttu-id="9d634-112">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="9d634-112">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="9d634-113">Отправка документов по электронной почте</span><span class="sxs-lookup"><span data-stu-id="9d634-113">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
