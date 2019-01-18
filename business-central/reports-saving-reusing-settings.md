---
title: "Применение и изменение сохраненных параметров в отчетах | Документы Майкрософт"
description: "Описывается использование заранее определенных параметров и фильтров для настройки отчета и формирования правильных данных."
author: jswymer
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customization, personalization
ms.date: 10/01/2018
ms.author: jswymer
ms.translationtype: HT
ms.sourcegitcommit: caf7cf5afe370af0c4294c794c0ff9bc8ff4c31c
ms.openlocfilehash: 9fd086831c0d145570d87c33c62a003c166aca87
ms.contentlocale: ru-ru
ms.lasthandoff: 11/22/2018

---
# <a name="managing-saved-settings-on-reports"></a><span data-ttu-id="88fc3-103">Управление сохраненными настройками в отчетах</span><span class="sxs-lookup"><span data-stu-id="88fc3-103">Managing Saved Settings on Reports</span></span>
<span data-ttu-id="88fc3-104">Во время выполнения отчетов пользователи видят страницу, которая позволяет задать некоторые параметры и фильтры для изменения данных, которые будут включены в отчет.</span><span class="sxs-lookup"><span data-stu-id="88fc3-104">When running a reports, users are typically presented with a page that lets them set certain options and filters for changing the data that is included in the generated report.</span></span> <span data-ttu-id="88fc3-105">Эта страница называется страницей запроса отчета.</span><span class="sxs-lookup"><span data-stu-id="88fc3-105">This page is called the report request page.</span></span> <span data-ttu-id="88fc3-106">Отчет может содержать одну или несколько *сохраненных настроек*, которые можно применять к отчету со страницы запроса отчета.</span><span class="sxs-lookup"><span data-stu-id="88fc3-106">A report can include one or more *saved settings* that users can apply to the report from the request page.</span></span> <span data-ttu-id="88fc3-107">*Сохраненные настройки* в целом являются заранее заданными параметрами и фильтрами.</span><span class="sxs-lookup"><span data-stu-id="88fc3-107">*Saved settings* are basically predefined options and filters.</span></span> <span data-ttu-id="88fc3-108">Сохраненные настройки обеспечивают быстрый и удобный способ последовательного создания отчетов, содержащих правильные данные.</span><span class="sxs-lookup"><span data-stu-id="88fc3-108">Using saved settings is a fast and reliable way to consistently generate reports that contain the correct data.</span></span> <span data-ttu-id="88fc3-109">Дополнительные сведения о том, как используются сохраненные настройки, см. в разделе [Использование сохраненных параметров](ui-work-report.md#SavedSettings).</span><span class="sxs-lookup"><span data-stu-id="88fc3-109">For more information about how saved settings are used, see [Using Saved Settings](ui-work-report.md#SavedSettings).</span></span>

<span data-ttu-id="88fc3-110">При наличии соответствующих прав доступа можно просматривать, создавать и изменять сохраненные настройки для всех отчетов для всех пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="88fc3-110">If you have the proper permissions, you can view, create, and modify the saved settings for all reports for all users in company.</span></span> <span data-ttu-id="88fc3-111">Можно назначить сохраненные настройки отчета индивидуальным пользователям или всем пользователям в организации.</span><span class="sxs-lookup"><span data-stu-id="88fc3-111">You can assign saved settings for a report to individual users or all users in the company.</span></span>

<!-- 
## Apply saved settings to a report
1. Open the report.

   The report request page appears.    
2. In the **Saved Settings** section of the page, set the **Name** field  to the saved settings that you want to use.

   The **Saved Settings** section only appears if the report has been run before or if there are existing saved settings entries. The saved settings entry called **Last used options and filters** is always available. These settings are the option and filter values that were used the last time you ran the report.

-->

## <a name="create-and-modify-saved-settings-for-all-users"></a><span data-ttu-id="88fc3-112">Создайте и измените сохраненные настройки для всех пользователей</span><span class="sxs-lookup"><span data-stu-id="88fc3-112">Create and modify saved settings for all users</span></span>
<span data-ttu-id="88fc3-113">Для управления сохраненными настройками используется страница **1560 Настройки отчетов**.</span><span class="sxs-lookup"><span data-stu-id="88fc3-113">You manage saved settings from page **1560 Reports Settings**.</span></span> <span data-ttu-id="88fc3-114">Существует два способа открыть эту страницу:</span><span class="sxs-lookup"><span data-stu-id="88fc3-114">There are two ways to open this page:</span></span>
-   <span data-ttu-id="88fc3-115">Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Параметры отчета**, затем выберите связанную ссылку.</span><span class="sxs-lookup"><span data-stu-id="88fc3-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Report Settings**, and then choose the related link.</span></span>
-   <span data-ttu-id="88fc3-116">Откройте отчет, нажмите кнопку выбора рядом с полем **Использовать значения по умолчанию из:** и выберите **Выбор из полного списка**.</span><span class="sxs-lookup"><span data-stu-id="88fc3-116">Open a report, choose the lookup next to the **Used default values from:** box, choose **Select from full list**.</span></span>

<span data-ttu-id="88fc3-117">На странице отобразятся все существующие операции сохраненных настроек для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="88fc3-117">The page displays all the existing save settings entries for all users.</span></span> <span data-ttu-id="88fc3-118">Если в столбце **Кому назначено** есть имя пользователя, то только этот пользователь может использовать сохраненные настройки для связанного отчета.</span><span class="sxs-lookup"><span data-stu-id="88fc3-118">If there is a user name in the **Assigned to** column, only that user can use the saved settings for the associated report.</span></span> <span data-ttu-id="88fc3-119">Если в столбце **Общий доступ для всех пользователей** стоит флажок, все пользователи могут использовать сохраненные настройки для отчета.</span><span class="sxs-lookup"><span data-stu-id="88fc3-119">If there is a check mark in the **Share with all users** column, all users can use the saved settings for the report.</span></span>

<span data-ttu-id="88fc3-120">На странице **Параметры отчета** можно:</span><span class="sxs-lookup"><span data-stu-id="88fc3-120">From the **Report Settings** page, you can:</span></span>
-   <span data-ttu-id="88fc3-121">Выбрать команду **Создать** для создания новой операции сохраненных настроек с нуля.</span><span class="sxs-lookup"><span data-stu-id="88fc3-121">Choose **New** to create a new saved settings entry from scratch.</span></span>
-   <span data-ttu-id="88fc3-122">Выбрать операцию сохраненных настроек из списка и нажать **Копировать** для создания копии.</span><span class="sxs-lookup"><span data-stu-id="88fc3-122">Select a saved settings entry from the list, and choose **Copy** to create a copy.</span></span>
-   <span data-ttu-id="88fc3-123">Выбрать операцию сохраненных настроек из списка и нажать **Правка**, чтобы изменить операцию сохраненных настроек.</span><span class="sxs-lookup"><span data-stu-id="88fc3-123">Select a saved settings entry from the list, and choose **Edit** to modify a saved settings entry.</span></span>


> [!Important]
> <span data-ttu-id="88fc3-124">Обратите внимание на имя, которое вы присваиваете операции сохраненных настроек.</span><span class="sxs-lookup"><span data-stu-id="88fc3-124">Consider the name that you give a saved settings entry.</span></span> <span data-ttu-id="88fc3-125">Если вы создаете операцию сохраненных настроек для всех пользователей и присваиваете ей то же имя, что и у существующей операции сохраненных настроек, назначенной только определенному пользователю, то этот пользователь не сможет использовать операцию сохраненных настроек, которая назначена всем.</span><span class="sxs-lookup"><span data-stu-id="88fc3-125">If you create a saved settings entry for all users, and you give it the same name as an existing saved settings entry that is assigned to a specific user only, then that user will not be able to use the saved settings entry that is assigned to everyone.</span></span>  <span data-ttu-id="88fc3-126">В поле **Сохраненные настройки** на странице запроса отчета пользователь сможет просмотреть две операции сохраненных настроек с одинаковым именем.</span><span class="sxs-lookup"><span data-stu-id="88fc3-126">Under **Saved Settings** on the report request page, the user will see two saved settings entries with the same name.</span></span> <span data-ttu-id="88fc3-127">Однако независимо от выбранного параметра будет использоваться операция сохраненных настроек для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="88fc3-127">However, no matter which option he chooses, the user-specific saved settings entry will be used.</span></span>

> [!NOTE]
> <span data-ttu-id="88fc3-128">Функция сохраненных настроек доступна только в отчетах, в которых для [свойства SaveValues](https://docs.microsoft.com/en-us/dynamics-nav/savevalues-property) страницы запроса отчета задано значение `Yes`.</span><span class="sxs-lookup"><span data-stu-id="88fc3-128">The saved settings feature is available only on reports where the [SaveValues property](https://docs.microsoft.com/en-us/dynamics-nav/savevalues-property) of the report's request page is set to `Yes`.</span></span> <span data-ttu-id="88fc3-129">Свойство **SaveValues** задается в среде разработки.</span><span class="sxs-lookup"><span data-stu-id="88fc3-129">The **SaveValues** property is set in the development environment.</span></span>  

## <a name="see-also"></a><span data-ttu-id="88fc3-130">См. также</span><span class="sxs-lookup"><span data-stu-id="88fc3-130">See Also</span></span>
[<span data-ttu-id="88fc3-131">Работа с отчетами</span><span class="sxs-lookup"><span data-stu-id="88fc3-131">Working with Reports</span></span>](ui-work-report.md)  

