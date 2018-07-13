---
title: "Добавление клиентов в интерфейс для бухгалтера в Dynamics 365 | Microsoft Docs"
description: "Узнайте, как добавлять существующих клиентов в Accountant Hub для Dynamics 365."
author: edupont04
ms.service: dynamics365-accountant
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, financial report
ms.date: 05/15/2018
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 4bc9199b879c23115082b07a81d6da5a0b46e60d
ms.openlocfilehash: 00e0d0a131b586d3aee39b3d08064defff81814a
ms.contentlocale: ru-ru
ms.lasthandoff: 05/31/2018

---
# <a name="add-clients-to-your-dashboard-in-include-d365acclongincludesd365acclongmdmd"></a>Добавление клиентов на панель мониторинга в [!INCLUDE [d365acc_long](includes/d365acc_long_md.md)]
[!INCLUDE [d365fin_early_release](includes/d365fin_early_release.md.md)]

Клиентов можно добавить с помощью окна **Клиенты**, которое можно открыть, выбрав в ленте **Управление клиентами**. Просто нажмите **Создать**, а затем заполните соответствующие поля.  

![Добавление клиента](./media/accountant-add-client/manage-client.png)

Данные в карточке для каждого контакта задаются вами, и вы можете изменять их при необходимости. Однако поле **URL-адрес клиента** является критическим. С его помощью вы получаете доступ к [!INCLUDE [d365fin](includes/d365fin_md.md)] каждого клиента. Воспользуйтесь действием **Проверить URL-адрес клиента** на ленте, чтобы убедиться, что вы указали правильную ссылку. Вводимый URL-адрес должен указывать на [!INCLUDE [d365fin](includes/d365fin_md.md)] клиента и включать адрес домена. Например, если клиент указал домен MyBusiness.com, то ссылка на их [!INCLUDE [d365fin](includes/d365fin_md.md)] будет иметь вид *https://businesscentral.dynamics.com/mybusiness.com?redirectedfromsignup=1*.  

> [!NOTE]
>  До обновления от мая 2018 года указываемый URL-адрес имел другой формат и начинался с адреса компании клиента. После мая 2018 года он имеет формат ```https://businesscentral.dynamics.com/clientdomain?redirectedfromsignup=1```, где ```clientdomain``` — домен клиента.  

URL-адрес клиента затем используется при выборе пункта меню **Перейти к компании** на панели мониторинга [!INCLUDE [d365acc](includes/d365acc_md.md)].  

### <a name="get-invited-to-a-clients-include-d365finlongincludesd365finlongmdmd"></a>Получение приглашения в [!INCLUDE [d365fin_long](includes/d365fin_long_md.md)] клиента
Компания, которая использует [!INCLUDE [d365fin](includes/d365fin_md.md)], может пригласить вас [!INCLUDE [d365fin](includes/d365fin_md.md)] как внешнего бухгалтера. Для получения приглашения необходимо предоставить адрес электронной почты для [!INCLUDE [d365acc](includes/d365acc_md.md)], например <em>me@accountant.com</em>. Администратор клиента может добавить вас в свою систему с помощью мастера **Пригласить внешнего бухгалтера**.  

После этого получите от компании-клиента сообщение электронной почты со ссылками на ее [!INCLUDE [d365fin](includes/d365fin_md.md)] Первая ссылка представляет собой приглашение для получения доступа к компании. Перейдите по этой ссылке и согласитесь с действиями, в результате которых вы будете добавлены в [!INCLUDE [d365fin](includes/d365fin_md.md)] своего клиента. Вторая ссылка предназначена для добавления этого клиента на вашу панель мониторинга в [!INCLUDE [d365acc](includes/d365acc_md.md)], как описано выше.  

После принятия приглашения вы автоматически войдете в систему и сможете обращаться к финансовым данным клиента из ролевого центра **Бухгалтер**. Дополнительные сведения см. в разделе [Работа бухгалтера в [!INCLUDE[d365fin](includes/d365fin_md.md)]](/dynamics365/business-central/finance-accounting?toc=/dynamics365/accountants/toc.json).  

## <a name="see-also"></a>См. также
[Начало работы с [!INCLUDE[d365acc](includes/d365acc_md.md)]](get-started.md)  
[Устранение неполадок в [!INCLUDE[d365acc](includes/d365acc_md.md)]](troubleshooting.md)  

