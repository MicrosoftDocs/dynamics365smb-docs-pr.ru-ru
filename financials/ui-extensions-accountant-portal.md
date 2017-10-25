---
title: "Использование портала бухгалтера | Документы Майкрософт"
description: "Предоставляется информация о расширении портала бухгалтера."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms. search.keywords: app, add-in, manifest, customize, accountant
ms.date: 09/05/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 84b2331f14b8c7e8d73921189e2df33fa709626e
ms.contentlocale: ru-ru
ms.lasthandoff: 09/22/2017

---
# <a name="accountant-portal-for-dynamics-365-for-financials"></a><span data-ttu-id="3d5ef-103">Портал бухгалтера для Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="3d5ef-103">Accountant Portal for Dynamics 365 for Financials</span></span>
<span data-ttu-id="3d5ef-104">Это приложение обеспечивает панель мониторинга со сводкой данных по каждому клиенту бухгалтера.</span><span class="sxs-lookup"><span data-stu-id="3d5ef-104">This application provides a dashboard with summary data for each client of an accountant.</span></span> <span data-ttu-id="3d5ef-105">На портале отображаются финансовые КПЭ, а также прямая ссылка на финансовое приложение клиента.</span><span class="sxs-lookup"><span data-stu-id="3d5ef-105">The portal displays financial KPIs as well as a direct link to the client’s financial application.</span></span>  

<span data-ttu-id="3d5ef-106">Панель мониторинга представляет собой специализированный ролевой центр для лучшего обзора клиентов.</span><span class="sxs-lookup"><span data-stu-id="3d5ef-106">The dashboard is a highly specialized Role Center for a better overview of your clients.</span></span>  
<span data-ttu-id="3d5ef-107">[![Портал бухгалтера](./media/ui-extensions-accportal/accountant-portal.png)](https://go.microsoft.com/fwlink/?linkid=851257)</span><span class="sxs-lookup"><span data-stu-id="3d5ef-107">[![Accountant Portal](./media/ui-extensions-accportal/accountant-portal.png)](https://go.microsoft.com/fwlink/?linkid=851257)</span></span>

<span data-ttu-id="3d5ef-108">При первой установке расширения пример организации помогает начать работать.</span><span class="sxs-lookup"><span data-stu-id="3d5ef-108">When you first install the extension, a sample company helps you get started.</span></span> <span data-ttu-id="3d5ef-109">Вы можете удалить пример организации в любой момент.</span><span class="sxs-lookup"><span data-stu-id="3d5ef-109">You can delete the sample company at any time.</span></span>  

## <a name="installing-the-extension"></a><span data-ttu-id="3d5ef-110">Установка расширения</span><span class="sxs-lookup"><span data-stu-id="3d5ef-110">Installing the Extension</span></span>
<span data-ttu-id="3d5ef-111">При установке расширения в ваш экземпляр [!INCLUDE[d365fin](includes/d365fin_md.md)] выводится запрос, требуется ли использовать его сейчас.</span><span class="sxs-lookup"><span data-stu-id="3d5ef-111">When you install the extension in your [!INCLUDE[d365fin](includes/d365fin_md.md)], you will be asked if you want to use it now.</span></span> <span data-ttu-id="3d5ef-112">Если требуется, необходимо выйти и снова войти, так как расширение заменяет ваш текущий ролевой центр и добавляет расширения в ваш профиль пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d5ef-112">If you do, then you must sign out and sign in again, because the extension replaces your current Role Center and adds permissions to your user profile.</span></span>  

<span data-ttu-id="3d5ef-113">Дополнительные сведения см. в разделе [Работа бухгалтера в Dynamics 365 for Financials](finance-accounting.md).</span><span class="sxs-lookup"><span data-stu-id="3d5ef-113">For more information, see [Accountant Experiences in Dynamics 365 for Financials](finance-accounting.md).</span></span>  

> [!NOTE]  
>  <span data-ttu-id="3d5ef-114">Текущая версия расширения требует, чтобы ваши клиенты использовали [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="3d5ef-114">The current version of the extension requires that your clients use [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

## <a name="using-the-extension"></a><span data-ttu-id="3d5ef-115">Использование расширения</span><span class="sxs-lookup"><span data-stu-id="3d5ef-115">Using the extension</span></span>
<span data-ttu-id="3d5ef-116">Это расширение используется при подписке на [Financials для бухгалтеров на Microsoft.com](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants). При установке расширения в [!INCLUDE[d365fin](includes/d365fin_md.md)] оно заменяет текущий ролевой центр.</span><span class="sxs-lookup"><span data-stu-id="3d5ef-116">This extension is used when you sign up at [Financials for Accountants on Microsoft.com](https://www.microsoft.com/en-us/dynamics365/financial-insights-for-accountants). If you install the extension in your [!INCLUDE[d365fin](includes/d365fin_md.md)], it will replace your current Role Center.</span></span> <span data-ttu-id="3d5ef-117">Если затем нужно вернуться к другому ролевому центру, это можно сделать в пункте "Мои настройки".</span><span class="sxs-lookup"><span data-stu-id="3d5ef-117">If you then want to return to the other Role Center, then you can do that in My Settings.</span></span> <span data-ttu-id="3d5ef-118">Дополнительные сведения см. в разделе [Практическое руководство. Изменение ролевого центра](change-role.md).</span><span class="sxs-lookup"><span data-stu-id="3d5ef-118">For more information, see [How to: Change the Role Center](change-role.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="3d5ef-119">См. также</span><span class="sxs-lookup"><span data-stu-id="3d5ef-119">See Also</span></span>
[<span data-ttu-id="3d5ef-120">Работа бухгалтера в Dynamics 365 for Financials</span><span class="sxs-lookup"><span data-stu-id="3d5ef-120">Accountant Experiences in Dynamics 365 for Financials</span></span>](finance-accounting.md)  
[<span data-ttu-id="3d5ef-121">Финансы</span><span class="sxs-lookup"><span data-stu-id="3d5ef-121">Finance</span></span>](finance.md)  

