---
title: "Административные задачи в Finance and Operations, Business edition | Microsoft Docs"
description: "Некоторые задачи в Finance and Operations, Business edition требуют централизованного администрирования и настройки. Познакомьтесь с этими задачами и узнайте, что делать."
author: edupont04
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/01/2017
ms.author: edupont
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: c64bc883031be28aa6634bdcf48f00c7ca77567d
ms.contentlocale: ru-ru
ms.lasthandoff: 02/02/2018

---
# <a name="setup-and-administration-in-finance-and-operations-business-edition"></a><span data-ttu-id="4d041-104">Настройка и администрирование в Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="4d041-104">Setup and Administration in Finance and Operations, Business edition</span></span>
<span data-ttu-id="4d041-105">Основные задачи администрирования обычно выполняются в организации исполнителем какой-либо одной роли.</span><span class="sxs-lookup"><span data-stu-id="4d041-105">Central administration tasks are usually performed by one role in the company.</span></span> <span data-ttu-id="4d041-106">Объем этих задач может зависеть от размера организации и должностных обязанностей администратора.</span><span class="sxs-lookup"><span data-stu-id="4d041-106">The scope of these tasks can depend on the company's size and the administrator's job responsibilities.</span></span> <span data-ttu-id="4d041-107">Среди подобных задач могут быть следующие: управление синхронизацией с базой данных работ и очередей электронной почты, задание пользователей, настройка пользовательского интерфейса и управление ключами шифрования.</span><span class="sxs-lookup"><span data-stu-id="4d041-107">These tasks can include managing database synchronization of job and email queues, setting up users, customizing the user interface, and managing encryption keys.</span></span>  

<span data-ttu-id="4d041-108">Ввод правильных значений настройки с самого начала важен для успешной работы любого нового программного обеспечения для бизнеса.</span><span class="sxs-lookup"><span data-stu-id="4d041-108">Entering the correct setup values from the start is important to the success of any new business software.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="4d041-109"> включает ряд руководство по настройке, помогающих настроить ключевые данные.</span><span class="sxs-lookup"><span data-stu-id="4d041-109"> includes a number of setup guides that help you set up core data.</span></span> <span data-ttu-id="4d041-110">Дополнительные сведения см. в разделе [Настройка Finance and Operations, Business edition](setup.md).</span><span class="sxs-lookup"><span data-stu-id="4d041-110">For more information, see [Setting Up Finance and Operations, Business edition](setup.md).</span></span>

<!--Whether you use [!INCLUDE[rim](../../includes/rim_md.md)] to implement setup values or you manually enter them in the new company, you can support your setup decisions with some general recommendations for selected setup fields that are known to potentially cause the solution to be inefficient if defined incorrectly.-->  

<span data-ttu-id="4d041-111">Администратор или привилегированный пользователь может настроить платформу обмена данными, чтобы разрешить пользователям экспорт и импорт данные в банковских файлах и файлах зарплаты, например, для различных процессов управления денежными средствами.</span><span class="sxs-lookup"><span data-stu-id="4d041-111">A super user or an administrator can set up the Data Exchange Framework to enable users to export and import data in bank and payroll files, for example for various cash management processes.</span></span>  

<span data-ttu-id="4d041-112">В следующей таблице приводится последовательность задач со ссылками на разделы, в которых они описываются.</span><span class="sxs-lookup"><span data-stu-id="4d041-112">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="4d041-113">**Задача**</span><span class="sxs-lookup"><span data-stu-id="4d041-113">**To**</span></span>|<span data-ttu-id="4d041-114">**Ссылка**</span><span class="sxs-lookup"><span data-stu-id="4d041-114">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="4d041-115">Добавьте пользователей, управляйте разрешениями и доступом к данным, назначьте роли.</span><span class="sxs-lookup"><span data-stu-id="4d041-115">Add users, manage permissions and access to data, assign roles.</span></span>|[<span data-ttu-id="4d041-116">Пользователи, профили и ролевые центры в Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="4d041-116">Users, Profiles, and Role Centers in Finance and Operations, Business edition</span></span>](admin-users-profiles-roles.md)|  
|<span data-ttu-id="4d041-117">Отслеживание всех непосредственных изменений, вносимых пользователями в данные базы данных, для определения источника ошибок и изменений в данных.</span><span class="sxs-lookup"><span data-stu-id="4d041-117">Track all direct modifications that users make to data in the database to identify the origin of errors and data changes.</span></span>|[<span data-ttu-id="4d041-118">Регистрация изменений в Finance and Operations, Business edition</span><span class="sxs-lookup"><span data-stu-id="4d041-118">Logging Changes in Finance and Operations, Business edition</span></span>](across-log-changes.md)|  
|<span data-ttu-id="4d041-119">Поддержка ваших решений по настройке за счет рекомендаций для выбранных полей, которые могут стать причиной неэффективной работы решения в случае неправильной настройки.</span><span class="sxs-lookup"><span data-stu-id="4d041-119">Support your setup decisions with recommendations for selected fields that are known to potentially cause the solution to be inefficient if set up incorrectly</span></span>|[<span data-ttu-id="4d041-120">Настройка сложных областей приложения с помощью рекомендаций</span><span class="sxs-lookup"><span data-stu-id="4d041-120">Set Up Complex Application Areas Using Best Practices</span></span>](set-up-complex-application-areas-using-best-practices.md)|  
|<span data-ttu-id="4d041-121">Можно отображать страницы, модули codeunit и запросы как веб-службы.</span><span class="sxs-lookup"><span data-stu-id="4d041-121">Expose pages, codeunits, and queries as web services.</span></span>|[<span data-ttu-id="4d041-122">Публикация веб-службы</span><span class="sxs-lookup"><span data-stu-id="4d041-122">Publish a Web Service</span></span>](across-how-publish-web-service.md)|  
|<span data-ttu-id="4d041-123">Настройте SMTP-сервер для включения передачи сообщений электронной почты в приложении Finance and Operations, Business edition и из него.</span><span class="sxs-lookup"><span data-stu-id="4d041-123">Set up an SMTP server to enable e-mail communication in and out of Finance and Operations, Business edition</span></span>| [<span data-ttu-id="4d041-124">Настройка электронной почты вручную или с помощью сопровождаемой настройки</span><span class="sxs-lookup"><span data-stu-id="4d041-124">Set Up Email Manually or Using the Assisted Setup</span></span>](madeira-how-setup-email.md)|  
|<span data-ttu-id="4d041-125">Ввод одиночных или повторяющихся запросов для создания отчетов или запуска модулей Codeunit.</span><span class="sxs-lookup"><span data-stu-id="4d041-125">Enter single or recurring requests to run reports or codeunits.</span></span>|[<span data-ttu-id="4d041-126">Использование очередей работ для планирования задач</span><span class="sxs-lookup"><span data-stu-id="4d041-126">Use Job Queues to Schedule Tasks</span></span>](admin-job-queues-schedule-tasks.md)|  
|<span data-ttu-id="4d041-127">Управление документами, удаление или сжатие документов</span><span class="sxs-lookup"><span data-stu-id="4d041-127">Manage, delete, or compress documents</span></span>|[<span data-ttu-id="4d041-128">Управление документами</span><span class="sxs-lookup"><span data-stu-id="4d041-128">Manage Documents</span></span>](admin-manage-documents.md)|  
|<span data-ttu-id="4d041-129">Настройка нового филиала с помощью шаблонов</span><span class="sxs-lookup"><span data-stu-id="4d041-129">Set up a new business unit using templates</span></span>|<span data-ttu-id="4d041-130">[Создание новых организаций в [!INCLUDE[d365fin](includes/d365fin_md.md)]](about-new-company.md)</span><span class="sxs-lookup"><span data-stu-id="4d041-130">[Creating New Companies in [!INCLUDE[d365fin](includes/d365fin_md.md)]](about-new-company.md)</span></span>|  

## <a name="see-also"></a><span data-ttu-id="4d041-131">См. также</span><span class="sxs-lookup"><span data-stu-id="4d041-131">See Also</span></span>
[<span data-ttu-id="4d041-132">Функциональные бизнес-возможности</span><span class="sxs-lookup"><span data-stu-id="4d041-132">Business Functionality</span></span>](madeira-business-functionality.md)  
[<span data-ttu-id="4d041-133">Общие бизнес-функции</span><span class="sxs-lookup"><span data-stu-id="4d041-133">General Business Functionality</span></span>](ui-across-business-areas.md)  
<span data-ttu-id="4d041-134">[Работа с [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="4d041-134">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="4d041-135">[Добро пожаловать в [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span><span class="sxs-lookup"><span data-stu-id="4d041-135">[Welcome to [!INCLUDE[d365fin](includes/d365fin_md.md)]](index.md)</span></span>  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  
## [!INCLUDE[d365fin](includes/training_link_md.md)]

