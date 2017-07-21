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
ms.lasthandoff: 07/07/2017


---
# <a name="reporting-sales-tax-and-goodsservices-tax-in-canada"></a>Отчетность по налогу с продаж и налогу на товары и услуги в Канаде
В Канаде, если поставщик не имеет представительства в провинции, в которой будет совершаться покупка, поставщик будет начислять GST-налог (Goods and Services Tax) или только HST-налог (Harmonized Sales Tax). Однако если в провинции применяется местный налог с продаж (PST, Provincial Sales Tax), покупатель должен рассчитывать PST-налог и уплачивать его непосредственно в провинции. Если выбран провинциальный код налоговой области, [!INCLUDE[d365fin](includes/d365fin_md.md)] использует его для вычисления PST-налога и учета его таким образом, чтобы налоговые обязательства отражались как в главной книге, так и в записях налоговой операции. Поэтому выбранный здесь код налоговой области должен соответствовать коду области, где применяется PST-налог, а не GST-налог.  

Дополнительные сведения о налоге с продаж см в разделе [Налог с продаж и налоговые группы в США и Канаде](us-finance-sales-tax.md).  

## <a name="submitting-the-gsthst-file"></a>Отправка GST/HST-файла
Сведения о налоге в документах покупки используются для формирования GST/HST-файлов для подачи по Интернету в налоговые органы. Этот файл включает GST-налог и HST-налог. Файл создается в формате TAX, который можно передавать через Интернет.  

## <a name="see-also"></a>См. также
[Финансы](finance.md)  
[Настройка финансов](finance-setup-finance.md)  
[Налог с продаж и налоговые группы в США и Канаде](us-finance-sales-tax.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

