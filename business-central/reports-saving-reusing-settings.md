---
title: Применение и изменение сохраненных параметров в отчетах | Документация Майкрософт
description: Описывается использование заранее определенных параметров и фильтров для настройки отчета и формирования правильных данных.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customization, personalization
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 70b3f391c141aa53dcef258a131d6395782a4488
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/15/2021
ms.locfileid: "5392553"
---
# <a name="manage-saved-settings-for-reports-and-batch-jobs"></a><span data-ttu-id="9ac46-103">Управление сохраненными настройками отчетов и пакетных заданий</span><span class="sxs-lookup"><span data-stu-id="9ac46-103">Manage Saved Settings for Reports and Batch jobs</span></span>
<span data-ttu-id="9ac46-104">Во время выполнения отчетов пользователи обычно видят страницу, которая позволяет задать параметры и установить фильтры для изменения данных, которые будут включены в отчет.</span><span class="sxs-lookup"><span data-stu-id="9ac46-104">When running reports, users are typically presented with a page that lets them select options and set filters to change the data that is included in the generated report.</span></span> <span data-ttu-id="9ac46-105">Эта страница называется страницей запроса.</span><span class="sxs-lookup"><span data-stu-id="9ac46-105">This page is called the request page.</span></span> <span data-ttu-id="9ac46-106">Отчет может содержать одну или несколько *сохраненных настроек*, которые можно применять к отчету со страницы запроса отчета.</span><span class="sxs-lookup"><span data-stu-id="9ac46-106">A report can include one or more *saved settings* that users can apply to the report from the request page.</span></span> <span data-ttu-id="9ac46-107">*Сохраненные настройки* в целом являются заранее заданными параметрами и фильтрами.</span><span class="sxs-lookup"><span data-stu-id="9ac46-107">*Saved settings* are basically predefined options and filters.</span></span> <span data-ttu-id="9ac46-108">Сохраненные настройки обеспечивают быстрый и удобный способ единообразного создания отчетов, содержащих правильные данные.</span><span class="sxs-lookup"><span data-stu-id="9ac46-108">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span></span> <span data-ttu-id="9ac46-109">Дополнительные сведения см. в разделе [Использование сохраненных параметров](ui-work-report.md#SavedSettings).</span><span class="sxs-lookup"><span data-stu-id="9ac46-109">For more information, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span></span>

> [!NOTE]
> <span data-ttu-id="9ac46-110">В этом разделе в основном упоминается "отчет", но аналогичная информация относится к пакетным заданиям.</span><span class="sxs-lookup"><span data-stu-id="9ac46-110">This topic refers mainly to "report", but similar information applies to batch jobs.</span></span>

<span data-ttu-id="9ac46-111">При наличии соответствующих прав доступа можно просматривать, создавать и изменять сохраненные настройки для всех отчетов для всех пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="9ac46-111">If you have the proper permissions, you can view, create, and modify the saved settings for all reports for all users in a company.</span></span> <span data-ttu-id="9ac46-112">Можно назначить сохраненные настройки отчета отдельным пользователям или всем пользователям в организации.</span><span class="sxs-lookup"><span data-stu-id="9ac46-112">You can assign saved settings for a report to individual users or to all users in the company.</span></span>

<!--
## Apply saved settings to a report
1. Open the report.

   The request page appears.    
2. In the **Saved Settings** section of the page, set the **Name** field  to the saved settings that you want to use.

   The **Saved Settings** section only appears if the report has been run before or if there are existing saved settings entries. The saved settings entry called **Last used options and filters** is always available. These settings are the option and filter values that were used the last time you ran the report.

-->

## <a name="to-create-and-modify-saved-settings-for-all-users"></a><span data-ttu-id="9ac46-113">Создание и изменение сохраненных настроек для всех пользователей</span><span class="sxs-lookup"><span data-stu-id="9ac46-113">To create and modify saved settings for all users</span></span>
<span data-ttu-id="9ac46-114">Для управления сохраненными настройками используется страница **Настройки отчетов**.</span><span class="sxs-lookup"><span data-stu-id="9ac46-114">You manage saved settings on the **Reports Settings** page.</span></span> <span data-ttu-id="9ac46-115">Существует два способа открыть эту страницу:</span><span class="sxs-lookup"><span data-stu-id="9ac46-115">There are two ways to open this page:</span></span>
-   <span data-ttu-id="9ac46-116">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Параметры отчета**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="9ac46-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Settings**, and then choose the related link.</span></span>
-   <span data-ttu-id="9ac46-117">Откройте отчет, нажмите кнопку выбора рядом с полем **Использовать значения по умолчанию из** и выберите действие **Выбрать из полного списка**.</span><span class="sxs-lookup"><span data-stu-id="9ac46-117">Open a report, choose the lookup in the **Use default values from** field, and then choose the **Select from full list** action.</span></span>

<span data-ttu-id="9ac46-118">На странице отобразятся все существующие операции сохраненных настроек для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="9ac46-118">The page displays all the existing saved settings entries for all users.</span></span> <span data-ttu-id="9ac46-119">Если в поле **Кому назначено** есть имя пользователя, то только этот пользователь может использовать сохраненные настройки для связанного отчета.</span><span class="sxs-lookup"><span data-stu-id="9ac46-119">If there is a user name in the **Assigned to** field, only that user can use the saved settings for the associated report.</span></span> <span data-ttu-id="9ac46-120">Если в поле **Общий доступ для всех пользователей** стоит флажок, все пользователи могут использовать сохраненные настройки для отчета.</span><span class="sxs-lookup"><span data-stu-id="9ac46-120">If there is a check mark in the **Share with all users** field, all users can use the saved settings for the report.</span></span>

<span data-ttu-id="9ac46-121">На странице **Параметры отчета** можно:</span><span class="sxs-lookup"><span data-stu-id="9ac46-121">From the **Report Settings** page, you can:</span></span>
-   <span data-ttu-id="9ac46-122">Выбрать действие **Создать** для создания новой операции сохраненных настроек с нуля.</span><span class="sxs-lookup"><span data-stu-id="9ac46-122">Choose the **New** action to create a new saved settings entry from scratch.</span></span>
-   <span data-ttu-id="9ac46-123">Выбрать операцию сохраненных настроек из списка и выбрать действие **Копировать** для создания копии.</span><span class="sxs-lookup"><span data-stu-id="9ac46-123">Select a saved settings entry from the list, and choose the **Copy** action to create a copy.</span></span>
-   <span data-ttu-id="9ac46-124">Выбрать операцию сохраненных настроек из списка и выбрать действие **Изменить**, чтобы изменить операцию сохраненных настроек.</span><span class="sxs-lookup"><span data-stu-id="9ac46-124">Select a saved settings entry from the list, and choose the **Edit** action to modify a saved settings entry.</span></span>

> [!Important]
> <span data-ttu-id="9ac46-125">Обратите внимание на имя, которое вы присваиваете операции сохраненных настроек.</span><span class="sxs-lookup"><span data-stu-id="9ac46-125">Consider the name that you give a saved settings entry.</span></span> <span data-ttu-id="9ac46-126">Если вы создаете операцию сохраненных настроек для всех пользователей и присваиваете ей то же имя, что и у существующей операции сохраненных настроек, назначенной только определенному пользователю, то этот пользователь не сможет использовать операцию сохраненных настроек, которая назначена всем.</span><span class="sxs-lookup"><span data-stu-id="9ac46-126">If you create a saved settings entry for all users, and you give it the same name as an existing saved settings entry that is assigned to a specific user only, then that user will not be able to use the saved settings entry that is assigned to everyone.</span></span>  <span data-ttu-id="9ac46-127">В разделе **Сохраненные настройки** на странице запроса отчета пользователь увидит две операции сохраненных настроек с одинаковым именем.</span><span class="sxs-lookup"><span data-stu-id="9ac46-127">In the **Saved Settings** section on the request page, the user will see two saved settings entries with the same name.</span></span> <span data-ttu-id="9ac46-128">Однако независимо от выбранного варианта будет использоваться операция сохраненных настроек для данного пользователя.</span><span class="sxs-lookup"><span data-stu-id="9ac46-128">However, no matter which option they choose, the user-specific saved settings entry will be used.</span></span>

> [!NOTE]
> <span data-ttu-id="9ac46-129">Функция сохраненных настроек доступна только в отчетах, в которых для [свойства SaveValues](/dynamics365/business-central/dev-itpro/developer/properties/devenv-savevalues-property) страницы запроса отчета задано значение **Да**.</span><span class="sxs-lookup"><span data-stu-id="9ac46-129">The Saved Settings feature is available only on reports where the [SaveValues property](/dynamics365/business-central/dev-itpro/developer/properties/devenv-savevalues-property) of the report's request page is set to **Yes**.</span></span> <span data-ttu-id="9ac46-130">Свойство **SaveValues** задается в среде разработки.</span><span class="sxs-lookup"><span data-stu-id="9ac46-130">The **SaveValues** property is set in the development environment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9ac46-131">См. также</span><span class="sxs-lookup"><span data-stu-id="9ac46-131">See Also</span></span>
[<span data-ttu-id="9ac46-132">Работа с отчетами, пакетными заданиями и XMLport</span><span class="sxs-lookup"><span data-stu-id="9ac46-132">Working with Reports, Batch Jobs, and XMLports</span></span>](ui-work-report.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]