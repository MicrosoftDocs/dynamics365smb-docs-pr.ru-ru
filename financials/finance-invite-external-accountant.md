---
title: "Добавление внешнего бухгалтера в Financials | Документы Майкрософт"
description: "Узнайте, как можно пригласить внешнего бухгалтера в Dynamics 365 for Financials."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting
ms.date: 06/23/2017
ms.author: edupont
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 1b9f88f02b198ae8da0f3359a3ce7799b9535739
ms.contentlocale: ru-ru
ms.lasthandoff: 07/07/2017


---
# <a name="invite-your-external-accountant-to-your-included365finincludesd365finmdmd"></a>Приглашение внешнего бухгалтера в ваш экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)]
Если вы используете внешнего бухгалтера для управления вашим учетом и финансовой отчетностью, вы можете пригласить его в свой экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)], чтобы он работал в вашими данными.

Как только бухгалтер получит доступ к вашему экземпляру [!INCLUDE[d365fin](includes/d365fin_md.md)], он сможет использовать ролевой центр **Бухгалтер**, который предоставляет простой доступ к наиболее важным для его работы окнам.  

> [!NOTE]  
>  Эта функция требует, чтобы было задано значение **Пакет**. Дополнительные сведения см. в разделе [Настройка взаимодействия Financials](ui-experiences.md).  

## <a name="invite-your-accountant-to-your-included365finincludesd365finmdmd"></a>Приглашение бухгалтера в ваш экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)]
В текущей версии [!INCLUDE[d365fin](includes/d365fin_md.md)] для приглашения внешнего бухгалтера администратор должен добавить его к вашему арендатору Active Directory. Соответствующие шаги зависят от типа учетной записи, которую вы использовали при регистрации в [!INCLUDE[d365fin](includes/d365fin_md.md)]. В этом разделе описано использование учетной записи Office 365, которая использует Microsoft Azure Active Directory.  

> [!TIP]  
>  Рекомендуется обратиться за помощью к вашему партнеру [!INCLUDE[d365fin](includes/d365fin_md.md)].  

Если вы активировали свою подписку [!INCLUDE[d365fin](includes/d365fin_md.md)] и больше не используете ознакомительную организацию, у вас есть арендатор Active Directory. Ваш администратор или партнер [!INCLUDE[d365fin](includes/d365fin_md.md)] управляет этим арендатором на [портале Azure](https://portal.azure.com). Там вы можете добавлять новых пользователей и выдавать и отзывать лицензии. Дополнительные сведения см. в разделе [Обзор портала Microsoft Azure](https://docs.microsoft.com/en-us/azure/azure-portal-overview).  

### <a name="separate-license"></a>Отдельная лицензия
Одним из типов лицензий для [!INCLUDE[d365fin](includes/d365fin_md.md)] является лицензия *Внешний бухгалтер*. Этот тип лицензии предназначен для использования такими пользователями, как внешние бухгалтеры. Это означает, что вам не нужно покупать дополнительное место в текущей подписке Active Directory или использовать одну из имеющихся учетных записей пользователя [!INCLUDE[d365fin](includes/d365fin_md.md)] для внешнего бухгалтера. Например, если ваша текущая подписка Office 365 включает 10 пользователей [!INCLUDE[d365fin](includes/d365fin_md.md)] и вы уже используете 10 лицензий *Полный пользователь*, ваш администратор может просто добавить внешнего бухгалтера в качестве гостя на портал Azure и без дополнительной платы назначить этому пользователю лицензию *Внешний бухгалтер*. Однако у вам может быть только один пользователь с лицензией *Внешний бухгалтер*. Если требуется добавить больше пользователей, следует соответствующим образом обновить. подписку Office 365.  

## <a name="see-also"></a>См. также
[Финансы](finance.md)  
[Работа бухгалтера в Dynamics 365 for Financials](finance-accounting.md)  
[Financials для бухгалтеров на Microsoft.com](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants)  

