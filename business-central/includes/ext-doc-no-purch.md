---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 05/27/2021
ms.author: edupont
ms.openlocfilehash: 59376b96dcd6f755040b07784ceca53e157bcf14
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115990"
---
<span data-ttu-id="9f3e2-101">В документах закупок и журналах вы можете указать номер документа, который относится к системе нумерации поставщика.</span><span class="sxs-lookup"><span data-stu-id="9f3e2-101">On purchase documents and journals, you can specify a document number that refers to the vendor's numbering system.</span></span> <span data-ttu-id="9f3e2-102">Используйте это поле для записи номера, который поставщик присвоил заказу, счету-фактуре или кредит-ноте.</span><span class="sxs-lookup"><span data-stu-id="9f3e2-102">Use this field to record the number that the vendor assigned to the order, invoice, or credit memo.</span></span> <span data-ttu-id="9f3e2-103">Впоследствии, если нужно, можно будет осуществлять поиск учтенной записи по данному номеру.</span><span class="sxs-lookup"><span data-stu-id="9f3e2-103">You can then use the number later if, for some reason, you need to search for the posted entry using this number.</span></span>

<span data-ttu-id="9f3e2-104">В поле **Номер внеш. документа обязателен** на странице **Настройка модуля "Покупки и кредиторская задолженность"** указано, является ли обязательным ввод номера внешнего документа в следующих ситуациях:</span><span class="sxs-lookup"><span data-stu-id="9f3e2-104">The **Ext. Doc. No. Mandatory** field in the **Purchases & Payables Setup** page specifies whether it is mandatory to enter an external document number in the following situations:</span></span>

* <span data-ttu-id="9f3e2-105">В поле **Номер счета поставщика**, **Номер заказа поставщика**</span><span class="sxs-lookup"><span data-stu-id="9f3e2-105">In the **Vendor Invoice No.** field, **Vendor Order No.**</span></span> <span data-ttu-id="9f3e2-106">или **Номер кредит-ноты поставщика**</span><span class="sxs-lookup"><span data-stu-id="9f3e2-106">field, or the **Vendor Cr. Memo No.**</span></span> <span data-ttu-id="9f3e2-107">в заголовке покупки</span><span class="sxs-lookup"><span data-stu-id="9f3e2-107">field on a purchase header</span></span>

* <span data-ttu-id="9f3e2-108">В поле **Номер внешнего документа** в строке финансового журнала, где содержимое поля **Тип документа** задано как *Счет*, *Кредит-нота* или *Процент-нота*, и поле **Тип счета** задано как *Поставщик*.</span><span class="sxs-lookup"><span data-stu-id="9f3e2-108">In the **External Document No.** field on a general journal line, where the **Document Type** field is set to *Invoice*, *Credit Memo*, or *Finance Charge Memo*, and the **Account Type** field is set to *Vendor*.</span></span>

<span data-ttu-id="9f3e2-109">Если выбрано это поле, то описанные выше счет, кредит-нота или тип строки финансового журнала будет невозможно учесть без номера внешнего документа.</span><span class="sxs-lookup"><span data-stu-id="9f3e2-109">If you select this field, it will not be possible to post an invoice, a credit memo, or the type of general journal line described above without an external document number.</span></span>

<span data-ttu-id="9f3e2-110">Номер внешнего документа включается в учтенные документы, где вы можете искать по соответствующему номеру.</span><span class="sxs-lookup"><span data-stu-id="9f3e2-110">The external document number is included in posted documents where you can search by the relevant number.</span></span> <span data-ttu-id="9f3e2-111">Вы также можете выполнять поиск по внешнему номеру документа при навигации по записям книги поставщиков.</span><span class="sxs-lookup"><span data-stu-id="9f3e2-111">You can also search using the external document number when navigating on vendor ledger entries.</span></span>

<span data-ttu-id="9f3e2-112">Другой способ обработки номеров внешних документов — использовать поле **Ваша ссылка**.</span><span class="sxs-lookup"><span data-stu-id="9f3e2-112">A different way to handle external document numbers is to use the **Your Reference** field.</span></span> <span data-ttu-id="9f3e2-113">Если вы используете поле **Ваша ссылка**, номер будет включен в учтенные документы, и вы можете искать по нему так же, как и значения из полей **Номер внешнего документа**.</span><span class="sxs-lookup"><span data-stu-id="9f3e2-113">If you use the **Your Reference** field, the number will be included in posted documents, and you can search by it in the same way as for values from **External Document No.** fields.</span></span> <span data-ttu-id="9f3e2-114">Но поле недоступно в строках журнала.</span><span class="sxs-lookup"><span data-stu-id="9f3e2-114">But the field is not available on journal lines.</span></span>
