---
title: Устранение неполадок при интеграции с Microsoft Flow | Документы Майкрософт
description: Устраняйте неполадки, чтобы сделать данные Business Central доступными в качестве источника данных и указать URL-адрес OData ваших веб-служб для создания автоматического бизнес-процесса.
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: workflow, Odata, Power App, SOAP
ms.date: 10/01/2018
ms.author: solsen
ms.openlocfilehash: 0818550021bf17e5a269d3e11f8db54b9ff80dfa
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "804604"
---
# <a name="troubleshooting-integration-with-microsoft-flow---request-url-too-long"></a><span data-ttu-id="6bd58-103">Устранение неполадок при интеграции с Microsoft Flow — запрошенный URL-адрес слишком длинный</span><span class="sxs-lookup"><span data-stu-id="6bd58-103">Troubleshooting Integration with Microsoft Flow - Request URL Too Long</span></span>
<span data-ttu-id="6bd58-104">Можно использовать данные [!INCLUDE[d365fin](includes/d365fin_md.md)] как часть рабочего процесса в Microsoft Flow.</span><span class="sxs-lookup"><span data-stu-id="6bd58-104">You can use your [!INCLUDE[d365fin](includes/d365fin_md.md)] data as part of a workflow in Microsoft Flow.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="6bd58-105">Вы должны иметь допустимую учетную запись в [!INCLUDE[d365fin](includes/d365fin_md.md)] и в Flow.</span><span class="sxs-lookup"><span data-stu-id="6bd58-105">You must have a valid account with [!INCLUDE[d365fin](includes/d365fin_md.md)] and with Flow.</span></span>  

<span data-ttu-id="6bd58-106">При создании Microsoft Flow с помощью соединителя [!INCLUDE[d365fin](includes/d365fin_md.md)] вы можете получить сообщение об ошибке, указывающее, что запрошенный URL-адрес слишком длинный после создания потока, например: **RequestUriTooLong**.</span><span class="sxs-lookup"><span data-stu-id="6bd58-106">If you are creating a Microsoft Flow using the [!INCLUDE[d365fin](includes/d365fin_md.md)] connector, you may receive an error message stating that the requsted URL is too long after creating the flow, such as the following: **RequestUriTooLong**.</span></span>

## <a name="cause"></a><span data-ttu-id="6bd58-107">Причина</span><span class="sxs-lookup"><span data-stu-id="6bd58-107">Cause</span></span>
<span data-ttu-id="6bd58-108">Для активации потока выполняется поиск изменений в данных.</span><span class="sxs-lookup"><span data-stu-id="6bd58-108">For a flow to trigger, it looks for changes in your data.</span></span> <span data-ttu-id="6bd58-109">Если определяется, что данные были изменены, соединители сравнивают кэшированные данные с новыми данными, запрошенными из источника.</span><span class="sxs-lookup"><span data-stu-id="6bd58-109">When determining if your data has changed, the connectors compare the cached data to the new data requested from the source.</span></span>  

<span data-ttu-id="6bd58-110">Если запрос данных создается слишком длинный URL-адрес, возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="6bd58-110">If the data request creates a URL that is too long, it will fail.</span></span> <span data-ttu-id="6bd58-111">К распространенным причинам могут относиться следующие:</span><span class="sxs-lookup"><span data-stu-id="6bd58-111">Common causes may include:</span></span>
- <span data-ttu-id="6bd58-112">Обычно любая исходная таблица с более 250 строками.</span><span class="sxs-lookup"><span data-stu-id="6bd58-112">Generally, any source table with over 250 rows</span></span>
- <span data-ttu-id="6bd58-113">Исходные таблицы, содержащие несколько тысяч записей.</span><span class="sxs-lookup"><span data-stu-id="6bd58-113">Source tables containing multiple thousands of records</span></span>

## <a name="workaround"></a><span data-ttu-id="6bd58-114">Обходное решение</span><span class="sxs-lookup"><span data-stu-id="6bd58-114">Workaround</span></span>
<span data-ttu-id="6bd58-115">Выполните следующие шаги в качестве обходного решения.</span><span class="sxs-lookup"><span data-stu-id="6bd58-115">Follow these steps as a workaround.</span></span>
1. <span data-ttu-id="6bd58-116">Выберите изменение потока с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="6bd58-116">Choose to edit the flow that is failing.</span></span>
2. <span data-ttu-id="6bd58-117">Разверните **Показать дополнительные параметры** в триггере потока.</span><span class="sxs-lookup"><span data-stu-id="6bd58-117">Expand the **Show advanced options** on the flow trigger.</span></span>
3. <span data-ttu-id="6bd58-118">В поле **Пропустить подсчет** введите количество записей для пропуска.</span><span class="sxs-lookup"><span data-stu-id="6bd58-118">In the **Skip Count** field, enter the number of records to skip.</span></span>  
<span data-ttu-id="6bd58-119">Например, если для таблица, используемая как источник данных, имеет 4000 записей, введите 4000 как число записей для пропуска.</span><span class="sxs-lookup"><span data-stu-id="6bd58-119">For example, if the table that you are using as a data source has 4,000 records, enter 4,000 as the number of records to skip.</span></span>
4. <span data-ttu-id="6bd58-120">Обновите поток.</span><span class="sxs-lookup"><span data-stu-id="6bd58-120">Update your flow.</span></span>

> [!NOTE]  
> <span data-ttu-id="6bd58-121">Соединитель в данный момент находится в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="6bd58-121">The connector is currently in Beta.</span></span> <span data-ttu-id="6bd58-122">Обновления, связанные с изменением данных, будут добавлены в будущих выпусках.</span><span class="sxs-lookup"><span data-stu-id="6bd58-122">Updates to how data changes are targeted for a future release.</span></span>


## <a name="see-also"></a><span data-ttu-id="6bd58-123">См. также</span><span class="sxs-lookup"><span data-stu-id="6bd58-123">See Also</span></span>
<span data-ttu-id="6bd58-124">[Использование [!INCLUDE[d365fin](includes/d365fin_md.md)] в автоматическом бизнес-процессе](across-how-use-financials-data-source-flow.md)</span><span class="sxs-lookup"><span data-stu-id="6bd58-124">[Using [!INCLUDE[d365fin](includes/d365fin_md.md)] in an Automated Workflow](across-how-use-financials-data-source-flow.md)</span></span>  
[<span data-ttu-id="6bd58-125">Приступая к работе</span><span class="sxs-lookup"><span data-stu-id="6bd58-125">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="6bd58-126">Импорт бизнес-данных из других финансовых систем</span><span class="sxs-lookup"><span data-stu-id="6bd58-126">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="6bd58-127">[Управление пользователями и разрешениями](ui-how-users-permissions.md)  </span><span class="sxs-lookup"><span data-stu-id="6bd58-127">[Managing Users and Permissions](ui-how-users-permissions.md)  </span></span>  
<span data-ttu-id="6bd58-128">[Настройка [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="6bd58-128">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="6bd58-129">Финансы</span><span class="sxs-lookup"><span data-stu-id="6bd58-129">Finance</span></span>](finance.md)  
