---
title: "Налог с продаж в Канаде | Документы Майкрософт"
description: "Узнайте о местном налоге с продаж и налоге на товары и услуги в Канаде."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales tax, local
ms.date: 06/02/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 571b11f4f18ffd194bdfe1d1d412bca87df4b868
ms.contentlocale: ru-ru
ms.lasthandoff: 09/11/2017

---
# <a name="reporting-sales-tax-and-goodsservices-tax-in-canada"></a><span data-ttu-id="35414-103">Отчетность по налогу с продаж и налогу на товары и услуги в Канаде</span><span class="sxs-lookup"><span data-stu-id="35414-103">Reporting Sales Tax and Goods/Services Tax in Canada</span></span>
<span data-ttu-id="35414-104">В Канаде, если поставщик не имеет представительства в провинции, в которой будет совершаться покупка, поставщик будет начислять GST-налог (Goods and Services Tax) или только HST-налог (Harmonized Sales Tax).</span><span class="sxs-lookup"><span data-stu-id="35414-104">In Canada, when a vendor does not have a business presence in the province in which purchases are made, the vendor will charge the Goods and Services Tax (GST) or Harmonized Sales Tax (HST) only.</span></span> <span data-ttu-id="35414-105">Однако если в провинции применяется местный налог с продаж (PST, Provincial Sales Tax), покупатель должен рассчитывать PST-налог и уплачивать его непосредственно в провинции.</span><span class="sxs-lookup"><span data-stu-id="35414-105">However, if the province has a Provincial Sales Tax (PST), then the purchaser must still calculate the PST and pay it directly to the province.</span></span> <span data-ttu-id="35414-106">Если выбран провинциальный код налоговой области, [!INCLUDE[d365fin](includes/d365fin_md.md)] использует его для вычисления PST-налога и учета его таким образом, чтобы налоговые обязательства отражались как в главной книге, так и в записях налоговой операции.</span><span class="sxs-lookup"><span data-stu-id="35414-106">When a Provincial Tax Area Code is selected, [!INCLUDE[d365fin](includes/d365fin_md.md)] uses it to calculate the PST and post it so that there is a tax liability in both the general ledger and the tax entry records.</span></span> <span data-ttu-id="35414-107">Поэтому выбранный здесь код налоговой области должен соответствовать коду области, где применяется PST-налог, а не GST-налог.</span><span class="sxs-lookup"><span data-stu-id="35414-107">Therefore, the tax area code selected here should be one where only the PST is included, not the GST.</span></span>  

<span data-ttu-id="35414-108">Дополнительные сведения о налоге с продаж см в разделе [Налог с продаж и налоговые группы в США и Канаде](us-finance-sales-tax.md).</span><span class="sxs-lookup"><span data-stu-id="35414-108">For more information about sales tax, see [Sales Tax and Tax Groups in the US and Canada](us-finance-sales-tax.md).</span></span>  

## <a name="submitting-the-gsthst-file"></a><span data-ttu-id="35414-109">Отправка GST/HST-файла</span><span class="sxs-lookup"><span data-stu-id="35414-109">Submitting the GST/HST File</span></span>
<span data-ttu-id="35414-110">Сведения о налоге в документах покупки используются для формирования GST/HST-файлов для подачи по Интернету в налоговые органы.</span><span class="sxs-lookup"><span data-stu-id="35414-110">The tax information in purchase documents is used to generate a GST/HST online file transfer that you must provide to the tax authorities.</span></span> <span data-ttu-id="35414-111">Этот файл включает GST-налог и HST-налог.</span><span class="sxs-lookup"><span data-stu-id="35414-111">This file includes goods and services tax (GST) and harmonized sales tax (HST).</span></span> <span data-ttu-id="35414-112">Файл создается в формате TAX, который можно передавать через Интернет.</span><span class="sxs-lookup"><span data-stu-id="35414-112">The file is created in a .tax file format, which can be transferred online.</span></span>  

## <a name="see-also"></a><span data-ttu-id="35414-113">См. также</span><span class="sxs-lookup"><span data-stu-id="35414-113">See Also</span></span>
[<span data-ttu-id="35414-114">Финансы</span><span class="sxs-lookup"><span data-stu-id="35414-114">Finance</span></span>](finance.md)  
[<span data-ttu-id="35414-115">Настройка финансов</span><span class="sxs-lookup"><span data-stu-id="35414-115">Setting Up Finance</span></span>](finance-setup-finance.md)  
[<span data-ttu-id="35414-116">Налог с продаж и налоговые группы в США и Канаде</span><span class="sxs-lookup"><span data-stu-id="35414-116">Sales Tax and Tax Groups in the US and Canada</span></span>](us-finance-sales-tax.md)  
<span data-ttu-id="35414-117">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="35414-117">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

