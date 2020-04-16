---
title: Расширение отправки авизо | Документация Майкрософт
description: Описывается расширение отправки авизо, которое позволяет отправить по электронной почте и повторно отправить авизо из журнала платежей и операций книги поставщиков.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, stream, remittance, advice
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: 439f9997e9ee70ff290a42e5044a9dbaff1112de
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "3190351"
---
# <a name="send-remittance-advice"></a><span data-ttu-id="5d9dc-103">Отправить авизо</span><span class="sxs-lookup"><span data-stu-id="5d9dc-103">Send Remittance Advice</span></span>
<span data-ttu-id="5d9dc-104">Если авизо используется для уведомления поставщиков о произведенных платежах, теперь можно использовать массовую рассылку авизо по электронной почте из журнала платежей, а также повторно отправлять авизо после выполнения платежей из операций книги поставщиков с помощью профилей отправки документов.</span><span class="sxs-lookup"><span data-stu-id="5d9dc-104">Where remittance advice is used to notify vendors of payments being made, you can now email remittance advice in bulk from the payment journal as well as resend after payments are made from vendor ledger entries by using document sending profiles.</span></span>

> [!NOTE]
> <span data-ttu-id="5d9dc-105">Эта функция поддерживается только в Business Central Online и On-Premises в следующих странах: Великобритания, США, Канада, Австралия, Новая Зеландия и Южная Африка.</span><span class="sxs-lookup"><span data-stu-id="5d9dc-105">This functionality is only supported in Business Central online and on-premises in following countries: United Kingdom, United States, Canada, Australia, New Zealand, and South Africa.</span></span>  

<span data-ttu-id="5d9dc-106">Авизо можно отправить двумя разными способами:</span><span class="sxs-lookup"><span data-stu-id="5d9dc-106">You can send remittance advice in two different ways:</span></span>

* <span data-ttu-id="5d9dc-107">На странице **Журнал платежей**, выберите **Навигация**, **Платежи**, **Отправить авизо**, чтобы отправить по электронной почте авизо для одной или нескольких строк журнала платежей поставщикам</span><span class="sxs-lookup"><span data-stu-id="5d9dc-107">In the **Payment Journal** page, choose **Navigate**, **Payments**, **Send Remittance Advice** to email remittance advice for one or multiple payment journal lines</span></span>
* <span data-ttu-id="5d9dc-108">На странице **Книга операций по поставщикам** выберите "Действия", "Функции", "Отправить авизо", чтобы отправить авизо по электронной почте после учета платежей поставщикам, для одной из нескольких операций журнала поставщиков</span><span class="sxs-lookup"><span data-stu-id="5d9dc-108">I the **Vendor Ledger Entries** page, choose Action, Functions, Send Remittance Advice to email remittance advice after posting of vendor payments, for one of multiple vendor ledger entries</span></span>

## <a name="see-also"></a><span data-ttu-id="5d9dc-109">См. также</span><span class="sxs-lookup"><span data-stu-id="5d9dc-109">See Also</span></span>
[<span data-ttu-id="5d9dc-110">Предлож. оплаты поставщикам</span><span class="sxs-lookup"><span data-stu-id="5d9dc-110">Suggest Vendor Payments</span></span>](payables-how-suggest-vendor-payments.md)  
<span data-ttu-id="5d9dc-111">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)] с помощью расширений](ui-extensions.md)  </span><span class="sxs-lookup"><span data-stu-id="5d9dc-111">[Customizing [!INCLUDE[d365fin](includes/d365fin_md.md)] Using Extensions ](ui-extensions.md)  </span></span>  
<span data-ttu-id="5d9dc-112">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="5d9dc-112">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
