---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 05/27/2021
ms.author: edupont
ms.openlocfilehash: 50b4b331f00bdcdf030bac2332ffb5dafdfd2de6
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115993"
---
<span data-ttu-id="24e0b-101">В документах продаж и журналах вы можете указать номер документа, который относится к системе нумерации клиента.</span><span class="sxs-lookup"><span data-stu-id="24e0b-101">On sales documents and journals, you can specify a document number that refers to the customer's numbering system.</span></span> <!--You can enter a maximum of ten characters, both numbers and letters.--> <span data-ttu-id="24e0b-102">Используйте это поле для записи номера, который клиент присвоил заказу, счету-фактуре или кредит-ноте.</span><span class="sxs-lookup"><span data-stu-id="24e0b-102">Use this field to record the number that the customer assigned to the order, invoice, or credit memo.</span></span> <span data-ttu-id="24e0b-103">Впоследствии, если нужно, можно будет осуществлять поиск учтенной записи по данному номеру.</span><span class="sxs-lookup"><span data-stu-id="24e0b-103">You can then use the number later if, for some reason, you need to search for the posted entry using this number.</span></span>  

<span data-ttu-id="24e0b-104">В поле **Номер внеш. документа обязателен** на странице **Настройка модуля "Покупки и кредиторская задолженность"** указано, является ли обязательным ввод номера внешнего документа в поле **Номер внешнего документа** в заголовке продажи и поле **Номер внешнего документа** в строке финансового журнала.</span><span class="sxs-lookup"><span data-stu-id="24e0b-104">The **Ext. Doc. No. Mandatory** field on the **Sales & Receivables Setup** page specifies whether it is mandatory to enter an external document number in the **External Document No.** field on a sales header and the **External Document No.** field on a general journal line.</span></span>

<span data-ttu-id="24e0b-105">Если выбрано это поле, учесть счет или строку финансового журнала без номера внешнего документа будет невозможно.</span><span class="sxs-lookup"><span data-stu-id="24e0b-105">If you select this field, it will not be possible to post an invoice or a general journal line without an external document number.</span></span>

<span data-ttu-id="24e0b-106">Номер внешнего документа включается в учтенные документы, где вы можете искать по соответствующему номеру.</span><span class="sxs-lookup"><span data-stu-id="24e0b-106">The external document number is included in posted documents where you can search by the relevant number.</span></span> <span data-ttu-id="24e0b-107">Вы также можете выполнять поиск по внешнему номеру документа при навигации по записям книги клиента.</span><span class="sxs-lookup"><span data-stu-id="24e0b-107">You can also search using the external document number when navigating on customer ledger entries.</span></span>

<span data-ttu-id="24e0b-108">Другой способ обработки номеров внешних документов — использовать поле **Ваша ссылка**.</span><span class="sxs-lookup"><span data-stu-id="24e0b-108">A different way to handle external document numbers is to use the **Your Reference** field.</span></span> <span data-ttu-id="24e0b-109">Если вы используете поле **Ваша ссылка**, номер будет включен в учтенные документы, и вы можете искать по нему так же, как и значения из полей **Номер внешнего документа**.</span><span class="sxs-lookup"><span data-stu-id="24e0b-109">If you use the **Your Reference** field, the number will be included in posted documents, and you can search by it in the same way as for values from **External Document No.** fields.</span></span> <span data-ttu-id="24e0b-110">Но поле недоступно в строках журнала.</span><span class="sxs-lookup"><span data-stu-id="24e0b-110">But the field is not available on journal lines.</span></span>
