---
title: "Назначение уровня приоритета поставщику | Microsoft Docs"
description: "Вы можете назначать номера поставщика для их приоритизации и поддержки функции предложений платежей в Business Central."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier, payment priority
ms.date: 03/29/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: f7834f0f99b775125425eb7209c3c648de4ccd1f
ms.contentlocale: ru-ru
ms.lasthandoff: 03/22/2018

---
# <a name="prioritize-vendors"></a>Назначение приоритетов поставщикам
В [!INCLUDE[d365fin](includes/d365fin_md.md)] предлагаются различные виды оплат поставщикам, например оплаты, которые должны быть произведены быстро, или оплаты, для которых возможны скидки. Дополнительные сведения см. в разделе [Предложение оплаты поставщикам](payables-how-suggest-vendor-payments.md).

Во-первых, следует назначить приоритеты поставщикам путем назначения им номеров.

## <a name="to-prioritize-vendors"></a>Назначение приоритета поставщикам
1. Выберите значок ![Поиск страницы или отчета](media/ui-search/search_small.png "Значок поиска страницы или отчета"), введите **Поставщики**, а затем выберите связанную ссылку.
2. Выберите соответствующего поставщика, а затем выберите **Правка**.
3. В поле **Приоритет** введите номер.

В [!INCLUDE[d365fin](includes/d365fin_md.md)] самый нижний номер (за исключением 0) рассматривается как номер с наивысшим приоритетом. Так, например, если используются 1, 2 и 3, то 1 будет иметь наивысший приоритет.

Если назначать приоритет для поставщика не требуется, оставьте поле **Приоритет** пустым. В случае же использования средства предложения с учетом приоритетов, поставщик, с пустым полем "Приоритет", будет числиться после всех поставщиков, которые имеют номер приоритета. В случае необходимости можно вводить столько уровней приоритета, сколько требуется.

## <a name="see-also"></a>См. также
[Настройка покупки](purchasing-setup-purchasing.md)  
[Управление кредиторской задолженностью](payables-manage-payables.md)  
[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)
