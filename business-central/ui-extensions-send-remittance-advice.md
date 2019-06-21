---
title: Расширение отправки авизо | Документы Майкрософт
description: Описывается расширение отправки авизо, которое позволяет отправить по электронной почте и повторно отправить авизо из журнала платежей и операций книги поставщиков.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, remittance, advice
ms.date: 06/06/2019
ms.author: sgroespe
ms.openlocfilehash: 9caa026f9edec42e56a035cf8d99228ca18c3c36
ms.sourcegitcommit: 04581558f6c5488c705a7ac392cf297be10b5f4f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2019
ms.locfileid: "1621256"
---
# <a name="send-remittance-advice"></a><span data-ttu-id="5ddbe-103">Отправить авизо</span><span class="sxs-lookup"><span data-stu-id="5ddbe-103">Send Remittance Advice</span></span>
<span data-ttu-id="5ddbe-104">Если авизо используется для уведомления поставщиков о произведенных платежах, теперь можно использовать массовую рассылку авизо по электронной почте из журнала платежей, а также повторно отправлять авизо после выполнения платежей из операций книги поставщиков с помощью профилей отправки документов.</span><span class="sxs-lookup"><span data-stu-id="5ddbe-104">Where remittance advice is used to notify vendors of payments being made, you can now email remittance advice in bulk from the payment journal as well as resend after payments are made from vendor ledger entries by using document sending profiles.</span></span>

> [!NOTE]
> <span data-ttu-id="5ddbe-105">Эта функция поддерживается только в Business Central Online и On-Premises в следующих странах: Великобритания, США, Канада, Австралия, Новая Зеландия и Южная Африка.</span><span class="sxs-lookup"><span data-stu-id="5ddbe-105">This functionality is only supported in Business Central online and on-premises in following countries: United Kingdom, United States, Canada, Australia, New Zealand, and South Africa.</span></span>  

<span data-ttu-id="5ddbe-106">Авизо можно отправить двумя разными способами:</span><span class="sxs-lookup"><span data-stu-id="5ddbe-106">You can send remittance advice in two different ways:</span></span>

* <span data-ttu-id="5ddbe-107">На странице **Журнал платежей**, выберите **Навигация**, **Платежи**, **Отправить авизо**, чтобы отправить по электронной почте авизо для одной или нескольких строк журнала платежей поставщикам</span><span class="sxs-lookup"><span data-stu-id="5ddbe-107">In the **Payment Journal** page, choose **Navigate**, **Payments**, **Send Remittance Advice** to email remittance advice for one or multiple payment journal lines</span></span>
* <span data-ttu-id="5ddbe-108">На странице **Книга операций по поставщикам** выберите "Действия", "Функции", "Отправить авизо", чтобы отправить авизо по электронной почте после учета платежей поставщикам, для одной из нескольких операций журнала поставщиков</span><span class="sxs-lookup"><span data-stu-id="5ddbe-108">I the **Vendor Ledger Entries** page, choose Action, Functions, Send Remittance Advice to email remittance advice after posting of vendor payments, for one of multiple vendor ledger entries</span></span>

## <a name="see-also"></a><span data-ttu-id="5ddbe-109">См. также</span><span class="sxs-lookup"><span data-stu-id="5ddbe-109">See Also</span></span>
[<span data-ttu-id="5ddbe-110">Предлож. оплаты поставщикам</span><span class="sxs-lookup"><span data-stu-id="5ddbe-110">Suggest Vendor Payments</span></span>](payables-how-suggest-vendor-payments.md)  
<span data-ttu-id="5ddbe-111">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="5ddbe-111">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="5ddbe-112">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5ddbe-112">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
