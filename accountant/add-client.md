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
ms.date: 10/23/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: ba26b354d235981bd7291f9ac6402779f554ac7a
ms.openlocfilehash: 6543eb4210a64802660189e5060975a327d71099
ms.contentlocale: ru-ru
ms.lasthandoff: 12/14/2017

---
# <a name="add-clients-to-your-dashboard-in-included365acclongincludesd365acclongmdmd"></a><span data-ttu-id="cc9e2-103">Добавление клиентов на панель мониторинга в [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)]</span><span class="sxs-lookup"><span data-stu-id="cc9e2-103">Add Clients to Your Dashboard in [!INCLUDE[d365acc_long](includes/d365acc_long_md.md)]</span></span>
[!INCLUDE[d365fin_early_release](includes/d365fin_early_release.md.md)]

<span data-ttu-id="cc9e2-104">Клиентов можно добавить с помощью окна **Клиенты**, которое можно открыть, выбрав в ленте **Управление клиентами**.</span><span class="sxs-lookup"><span data-stu-id="cc9e2-104">You can add a client by using the **Clients** window, which you can open by choosing the **Manage Clients** action in the ribbon.</span></span> <span data-ttu-id="cc9e2-105">Просто нажмите **Создать**, а затем заполните соответствующие поля.</span><span class="sxs-lookup"><span data-stu-id="cc9e2-105">Simply choose **New** and then fill in the fields.</span></span>  

![Добавление клиента](./media/accountant-add-client/manage-client.png)

<span data-ttu-id="cc9e2-107">Данные в карточке для каждого контакта задаются вами, и вы можете изменять их при необходимости.</span><span class="sxs-lookup"><span data-stu-id="cc9e2-107">The data in the card for each client is specified by you, and you can change it as needed.</span></span> <span data-ttu-id="cc9e2-108">Однако поле **URL-адрес клиента** является критическим. С его помощью вы получаете доступ к [!INCLUDE[d365fin](includes/d365fin_md.md)] каждого клиента.</span><span class="sxs-lookup"><span data-stu-id="cc9e2-108">However, the **Client URL** field is critical - this is how you can access each client's [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="cc9e2-109">Воспользуйтесь действием **Проверить URL-адрес клиента** на ленте, чтобы убедиться, что вы указали правильную ссылку.</span><span class="sxs-lookup"><span data-stu-id="cc9e2-109">Use the **Test Client URL** action in the ribbon to test that you entered the right link.</span></span> <span data-ttu-id="cc9e2-110">URL-адрес, который необходимо ввести, указывает на [!INCLUDE[d365fin](includes/d365fin_md.md)] клиента, например *https://mybusiness.financials.dynamics.com*. Этот URL-адрес затем используется при выборе пункта меню **Перейти к компании** на панели мониторинга [!INCLUDE[d365acc](includes/d365acc_md.md)].</span><span class="sxs-lookup"><span data-stu-id="cc9e2-110">The URL that you must enter points at the client's [!INCLUDE[d365fin](includes/d365fin_md.md)], such as *https://mybusiness.financials.dynamics.com*. This URL is then used when you choose the **Go To Company** menu item in the [!INCLUDE[d365acc](includes/d365acc_md.md)] dashboard.</span></span>  

### <a name="get-invited-to-a-clients-included365finlongincludesd365finlongmdmd"></a><span data-ttu-id="cc9e2-111">Получение приглашения в [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)] клиента</span><span class="sxs-lookup"><span data-stu-id="cc9e2-111">Get Invited to a Client's [!INCLUDE[d365fin_long](includes/d365fin_long_md.md)]</span></span>
<span data-ttu-id="cc9e2-112">Компания, которая использует [!INCLUDE[d365fin](includes/d365fin_md.md)], может пригласить вас [!INCLUDE[d365fin](includes/d365fin_md.md)] как внешнего бухгалтера.</span><span class="sxs-lookup"><span data-stu-id="cc9e2-112">A company who use [!INCLUDE[d365fin](includes/d365fin_md.md)] can invite you to [!INCLUDE[d365fin](includes/d365fin_md.md)] as their external accountant.</span></span> <span data-ttu-id="cc9e2-113">Чтобы получить приглашение, вы должны предоставить такой компании адрес электронной почты, который вы используете в [!INCLUDE[d365acc](includes/d365acc_md.md)], например *me@accountant.com*. После этого администратор компании-клиента может добавить вас в свою систему с помощью мастера **Пригласить внешнего бухгалтера**.</span><span class="sxs-lookup"><span data-stu-id="cc9e2-113">To get invited, you must give them the email that you use with [!INCLUDE[d365acc](includes/d365acc_md.md)], such as *me@accountant.com*. Your client's administrator can then add you to their system by running the **Invite External Accountant** wizard.</span></span>  

<span data-ttu-id="cc9e2-114">После этого получите от компании-клиента сообщение электронной почты со ссылками на ее [!INCLUDE[d365fin](includes/d365fin_md.md)]</span><span class="sxs-lookup"><span data-stu-id="cc9e2-114">As a result, you will receive email from your client with links to their [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="cc9e2-115">Первая ссылка представляет собой приглашение для получения доступа к компании. Перейдите по этой ссылке и согласитесь с действиями, в результате которых вы будете добавлены в [!INCLUDE[d365fin](includes/d365fin_md.md)] своего клиента.</span><span class="sxs-lookup"><span data-stu-id="cc9e2-115">The first link is an invitation to get access to their company - open the link and accept the steps that adds you to your client's [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span> <span data-ttu-id="cc9e2-116">Вторая ссылка предназначена для добавления этого клиента на вашу панель мониторинга в [!INCLUDE[d365acc](includes/d365acc_md.md)], как описано выше.</span><span class="sxs-lookup"><span data-stu-id="cc9e2-116">The second link is for adding this client to your dashboard in [!INCLUDE[d365acc](includes/d365acc_md.md)] as described above.</span></span>  

<span data-ttu-id="cc9e2-117">После принятия приглашения вы автоматически войдете в систему и сможете обращаться к финансовым данным клиента из ролевого центра **Бухгалтер**.</span><span class="sxs-lookup"><span data-stu-id="cc9e2-117">When you have accepted the invitation, you are logged in and can access the client's financial data from the **Accountant** Role Center.</span></span> <span data-ttu-id="cc9e2-118">Дополнительные сведения см. в разделе [Работа бухгалтера в [!INCLUDE[d365fin](includes/d365fin_md.md)]](/dynamics365/financials/finance-accounting?toc=/dynamics365/accountants/toc.json).</span><span class="sxs-lookup"><span data-stu-id="cc9e2-118">For more information, see [Accountant Experiences in [!INCLUDE[d365fin](includes/d365fin_md.md)]](/dynamics365/financials/finance-accounting?toc=/dynamics365/accountants/toc.json).</span></span>  

## <a name="see-also"></a><span data-ttu-id="cc9e2-119">См. также</span><span class="sxs-lookup"><span data-stu-id="cc9e2-119">See Also</span></span>
<span data-ttu-id="cc9e2-120">[Начало работы с [!INCLUDE[d365acc](includes/d365acc_md.md)]](get-started.md)</span><span class="sxs-lookup"><span data-stu-id="cc9e2-120">[Get Started with [!INCLUDE[d365acc](includes/d365acc_md.md)]](get-started.md)</span></span>  
<span data-ttu-id="cc9e2-121">[Устранение неполадок в [!INCLUDE[d365acc](includes/d365acc_md.md)]](troubleshooting.md)</span><span class="sxs-lookup"><span data-stu-id="cc9e2-121">[Troubleshooting [!INCLUDE[d365acc](includes/d365acc_md.md)]](troubleshooting.md)</span></span>  

