---
title: Устранение неполадок в вашем разделе организации
description: Узнайте, как обойти любые проблемы, когда вы работаете в узле компании в Dynamics 365 Business Central для управления работой в нескольких компаниях.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, troubleshoot
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: d75c6ceb27c7e1ee101b23bbc18f3eac0db4ced7
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5389128"
---
# <a name="troubleshooting-your-company-hub"></a><span data-ttu-id="a4c06-103">Устранение неполадок в вашем разделе организации</span><span class="sxs-lookup"><span data-stu-id="a4c06-103">Troubleshooting Your Company Hub</span></span>

<span data-ttu-id="a4c06-104">Добавлять компании в раздел организации также очень просто, однако в этой статье рассматриваются проблемы, которые могут при этом возникнуть.</span><span class="sxs-lookup"><span data-stu-id="a4c06-104">Adding companies to the company hub dashboard is easy enough, but this article addresses issues that you may have on the way.</span></span>  

## <a name="check-errors"></a><span data-ttu-id="a4c06-105">Проверка ошибок</span><span class="sxs-lookup"><span data-stu-id="a4c06-105">Check errors</span></span>

<span data-ttu-id="a4c06-106">Используйте действие **Проверить ошибки**, чтобы просмотреть список последних ошибок.</span><span class="sxs-lookup"><span data-stu-id="a4c06-106">Use the **Check Errors** action to view a list of recent errors.</span></span> <span data-ttu-id="a4c06-107">Вы можете просмотреть дополнительные сведения о каждой ошибке и очистить журнал, удалив старые записи.</span><span class="sxs-lookup"><span data-stu-id="a4c06-107">You can see additional details for each error, and you can clean up the log by deleting older entries.</span></span>  

## <a name="connection-failed"></a><span data-ttu-id="a4c06-108">Ошибка подключения</span><span class="sxs-lookup"><span data-stu-id="a4c06-108">Connection failed</span></span>

<span data-ttu-id="a4c06-109">Может быть несколько причин, по которым вы не можете подключиться к компании, в том числе следующие:</span><span class="sxs-lookup"><span data-stu-id="a4c06-109">There can be a couple of reasons why you cannot connect to a company, including the following:</span></span>

- <span data-ttu-id="a4c06-110">URL-адрес в поле **Ссылка на среду** не является действительным</span><span class="sxs-lookup"><span data-stu-id="a4c06-110">The URL in the **Environment Link** field is not valid</span></span>  

  <span data-ttu-id="a4c06-111">Перейдите на страницу **Ссылки на среды**, откройте среду, к которой вы не можете подключиться, а затем выберите действие **Проверить подключение**.</span><span class="sxs-lookup"><span data-stu-id="a4c06-111">Go to the **Environment Links** page, open the environment that you cannot connect to, and then choose the **Test the connection** action.</span></span>  
- <span data-ttu-id="a4c06-112">Компания клиента в настоящее время не подключена в сети, например из-за обновления</span><span class="sxs-lookup"><span data-stu-id="a4c06-112">The client's company is currently offline, for example if it being upgraded</span></span>

  <span data-ttu-id="a4c06-113">На панели мониторинга выберите пункт меню **Инструменты** и выберите **Проверить ошибки**.</span><span class="sxs-lookup"><span data-stu-id="a4c06-113">In your dashboard, choose the **Tools** menu item, and then choose **Check Errors**.</span></span> <span data-ttu-id="a4c06-114">Откроется список с техническими подробностями; если вы видите ошибки, возможно, имеет смысл связаться с администратором.</span><span class="sxs-lookup"><span data-stu-id="a4c06-114">This opens a list with technical details, so you might want to contact your administrator if you're seeing errors.</span></span> <span data-ttu-id="a4c06-115">Например, сообщение об ошибке "*Сервер отклонил учетные данные клиента*" может говорить о том, что у вас нет доступа.</span><span class="sxs-lookup"><span data-stu-id="a4c06-115">For example, the error message "*The server has rejected the client credentials*" suggests that you do not have access.</span></span>  
- <span data-ttu-id="a4c06-116">У вас нет доступа ко всем компаниям в среде, к которой вы пытаетесь подключиться.</span><span class="sxs-lookup"><span data-stu-id="a4c06-116">You do not have access to all companies in the environment that you are trying to connect to</span></span>

  <span data-ttu-id="a4c06-117">В [!INCLUDE [prod_short](includes/prod_short.md)] у организации может быть несколько бизнес-единиц, называемых компаниями, и у вас может не быть доступа ко всем компаниям.</span><span class="sxs-lookup"><span data-stu-id="a4c06-117">In [!INCLUDE [prod_short](includes/prod_short.md)], an organization can have multiple business units called companies, and you might not have access to all companies.</span></span> <span data-ttu-id="a4c06-118">Поговорите со своим администратором или клиентом, чтобы убедиться, что у вас есть доступ ко всем компаниям, с которыми вы должны работать.</span><span class="sxs-lookup"><span data-stu-id="a4c06-118">Work with your administrator or client to make sure that you have access to the companies that you have to work in.</span></span>  

## <a name="data-does-not-refresh"></a><span data-ttu-id="a4c06-119">Данные не обновляются</span><span class="sxs-lookup"><span data-stu-id="a4c06-119">Data does not refresh</span></span>

<span data-ttu-id="a4c06-120">Когда вы добавляете компанию или запрашиваете обновление данных, [!INCLUDE [prod_short](includes/prod_short.md)] извлекает данные.</span><span class="sxs-lookup"><span data-stu-id="a4c06-120">When you add a company or request a refresh of the data, [!INCLUDE [prod_short](includes/prod_short.md)] fetches the data.</span></span> <span data-ttu-id="a4c06-121">Однако вы должны сами обновить страницу: например, выбрать действие **Перезагрузить все компании**, обновить страницу браузера, перейти с панели мониторинга на другую страницу и затем вернуться и т. п.</span><span class="sxs-lookup"><span data-stu-id="a4c06-121">But you must refresh the page yourself, such as choosing the **Reload all companies** action, refresh the browser page, navigate away from the dashboard and then back again, or similar.</span></span>  

<span data-ttu-id="a4c06-122">Если вы добавили компанию, но она не отображается в списке, вы также можете использовать действие **Перезагрузить все компании** для обновления списка.</span><span class="sxs-lookup"><span data-stu-id="a4c06-122">If you've added a company but it is not displaying in the list, you can also use the **Reload all companies** action to update the list.</span></span>

## <a name="see-also"></a><span data-ttu-id="a4c06-123">См. также</span><span class="sxs-lookup"><span data-stu-id="a4c06-123">See also</span></span>

[<span data-ttu-id="a4c06-124">Управление работой нескольких компаний в разделе организаций</span><span class="sxs-lookup"><span data-stu-id="a4c06-124">Manage Work across Multiple Companies in the Company Hub</span></span>](company-hub.md)  
[<span data-ttu-id="a4c06-125">Добавьте компании в свой раздел организации</span><span class="sxs-lookup"><span data-stu-id="a4c06-125">Add companies to your company hub</span></span>](company-hub-add-company.md)  
[<span data-ttu-id="a4c06-126">Работа бухгалтера в Business Central</span><span class="sxs-lookup"><span data-stu-id="a4c06-126">Accountant Experiences in Business Central</span></span>](finance-accounting.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]