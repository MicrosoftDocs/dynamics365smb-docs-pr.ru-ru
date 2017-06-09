---
title: "Налог с продаж и налог на товары и услуги в Канаде | Документы Майкрософт"
description: "Информация о налогах GST и HST."
services: project-madeira
documentationcenter: 
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales tax, local
ms.date: 03/23/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: a31be0f9d07e2abb591e26f6bae34c6f6e4dcda6
ms.openlocfilehash: e1866f5047a826f3d527267d901eb30279d5b4e4
ms.contentlocale: ru-ru
ms.lasthandoff: 05/04/2017


---
# <a name="sales-tax-and-goods-and-services-tax-in-canada"></a>Налог с продаж и налог на товары и услуги в Канаде
В Канаде, если поставщик не имеет представительства в провинции, в которой будет совершаться покупка, поставщик будет начислять GST-налог (Goods and Services Tax) или только HST-налог (Harmonized Sales Tax). Однако если в провинции применяется местный налог с продаж (PST, Provincial Sales Tax), покупатель должен рассчитывать PST-налог и уплачивать его непосредственно в провинции. Если выбран провинциальный код налоговой области, [!INCLUDE[d365fin](includes/d365fin_md.md)] использует его для вычисления PST-налога и учета его таким образом, чтобы налоговые обязательства отражались как в главной книге, так и в записях налоговой операции. Поэтому выбранный здесь код налоговой области должен соответствовать коду области, где применяется PST-налог, а не GST-налог.  

Дополнительные сведения о налоге с продаж см в разделе [Налог с продаж и налоговые группы в США и Канаде](us-finance-sales-tax.md).  

## <a name="submitting-the-gsthst-file"></a>Отправка GST/HST-файла
Сведения о налоге в документах покупки используются для формирования GST/HST-файлов для подачи по Интернету в налоговые органы. Этот файл включает GST-налог и HST-налог. Файл создается в формате TAX, который можно передавать через Интернет.  

## <a name="see-also"></a>См. также
[Финансы](finance.md)  
[Настройка финансов](finance-setup-finance.md)  
[Налог с продаж и налоговые группы в США и Канаде](us-finance-sales-tax.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)

