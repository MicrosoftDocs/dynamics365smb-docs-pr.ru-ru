---
title: Назначение уровня приоритета поставщику | Документация Майкрософт
description: Вы можете назначать номера поставщика для их приоритизации и поддержки функции предложений платежей в Business Central.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: supplier, payment priority
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 1604113b255a585532677ccb47d7e68d1cc64059
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5772783"
---
# <a name="prioritize-vendors"></a>Назначение приоритетов поставщикам
В [!INCLUDE[prod_short](includes/prod_short.md)] предлагаются различные виды оплат поставщикам, например оплаты, которые должны быть произведены быстро, или оплаты, для которых возможны скидки. Дополнительные сведения см. в разделе [Предложение оплаты поставщикам](payables-how-suggest-vendor-payments.md).

Во-первых, следует назначить приоритеты поставщикам путем назначения им номеров.
<br><br>
> [!Video https://www.microsoft.com/videoplayer/embed/RE3PRGa?rel=0]

## <a name="to-prioritize-vendors"></a>Назначение приоритета поставщикам
1. Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Поставщики**, затем выберите соответствующую ссылку.
2. Выберите соответствующего поставщика, а затем выберите **Правка**.
3. В поле **Приоритет** введите номер.

В [!INCLUDE[prod_short](includes/prod_short.md)] самый нижний номер (за исключением 0) рассматривается как номер с наивысшим приоритетом. Так, например, если используются 1, 2 и 3, то 1 будет иметь наивысший приоритет.

Если назначать приоритет для поставщика не требуется, оставьте поле **Приоритет** пустым. В случае же использования средства предложения с учетом приоритетов, поставщик, с пустым полем "Приоритет", будет числиться после всех поставщиков, которые имеют номер приоритета. В случае необходимости можно вводить столько уровней приоритета, сколько требуется.

## <a name="see-also"></a>См. также
[Настройка покупки](purchasing-setup-purchasing.md)  
[Управление кредиторской задолженностью](payables-manage-payables.md)  
[Работа с [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]