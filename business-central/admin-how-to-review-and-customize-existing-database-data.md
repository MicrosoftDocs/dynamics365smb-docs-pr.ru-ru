---
title: Просмотр и настройка существующих данных базы данных | Документация Майкрософт
description: По мере создания пакета конфигурации для решения можно просматривать и настраивать доступные данные в базе данных в соответствии с потребностями клиента. Таблица базы данных должна иметь соответствующую страницу.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
redirect_url: admin-how-to-create-custom-company-configuration-packages
ms.openlocfilehash: 295329bf7f665a9dd34194b211a5ef65a7a65d4c
ms.sourcegitcommit: 02e704bc3e01d62072144919774f1244c42827e4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2019
ms.locfileid: "2308022"
---
# <a name="review-and-customize-existing-database-data"></a><span data-ttu-id="22b9a-104">Просмотр или настройка существующих данных базы данных</span><span class="sxs-lookup"><span data-stu-id="22b9a-104">Review and Customize Existing Database Data</span></span>
<span data-ttu-id="22b9a-105">По мере создания пакета конфигурации для решения можно просматривать и настраивать доступные данные в базе данных в соответствии с потребностями клиента.</span><span class="sxs-lookup"><span data-stu-id="22b9a-105">As you create a configuration package for a solution, you can view and customize the available database data to suit your customer needs.</span></span> <span data-ttu-id="22b9a-106">Таблица базы данных должна иметь соответствующую страницу.</span><span class="sxs-lookup"><span data-stu-id="22b9a-106">The database table has to have an associated page.</span></span>  

### <a name="to-customize-data-in-the-database"></a><span data-ttu-id="22b9a-107">Настройка данных в базе данных</span><span class="sxs-lookup"><span data-stu-id="22b9a-107">To customize data in the database</span></span>  

1.  <span data-ttu-id="22b9a-108">В журнале конфигураций определите таблицы, данные которых необходимо просмотреть или изменить.</span><span class="sxs-lookup"><span data-stu-id="22b9a-108">In the configuration worksheet, identify the tables whose data that you want to view or customize.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="22b9a-109">Убедитесь, что каждая таблица имеет код страницы, присвоенный ей.</span><span class="sxs-lookup"><span data-stu-id="22b9a-109">Make sure that each table has a page ID assigned to it.</span></span> <span data-ttu-id="22b9a-110">Для стандартных таблиц [!INCLUDE[d365fin](includes/d365fin_md.md)] это значение заполняется автоматически.</span><span class="sxs-lookup"><span data-stu-id="22b9a-110">For standard [!INCLUDE[d365fin](includes/d365fin_md.md)] tables, this value is automatically filled in.</span></span> <span data-ttu-id="22b9a-111">В случае пользовательских таблиц вам следует указать код.</span><span class="sxs-lookup"><span data-stu-id="22b9a-111">For custom tables, you have to provide the ID.</span></span>  

2.  <span data-ttu-id="22b9a-112">На вкладке **Действия** в группе **Показать** выберите **Данные из базы данных**.</span><span class="sxs-lookup"><span data-stu-id="22b9a-112">On the **Actions** tab, in the **Show** group, choose **Database Data**.</span></span>  

     <span data-ttu-id="22b9a-113">Откроется страница [!INCLUDE[d365fin](includes/d365fin_md.md)] для этой страницы.</span><span class="sxs-lookup"><span data-stu-id="22b9a-113">The [!INCLUDE[d365fin](includes/d365fin_md.md)] page for the page opens.</span></span>  

3.  <span data-ttu-id="22b9a-114">Просмотрите имеющуюся информацию.</span><span class="sxs-lookup"><span data-stu-id="22b9a-114">Review the available information.</span></span> <span data-ttu-id="22b9a-115">Измените его по мере необходимости путем удаления ненужных записей или добавления новых.</span><span class="sxs-lookup"><span data-stu-id="22b9a-115">Modify it as necessary by deleting records that are not relevant or by adding new ones.</span></span>  

## <a name="see-also"></a><span data-ttu-id="22b9a-116">См. также</span><span class="sxs-lookup"><span data-stu-id="22b9a-116">See Also</span></span>  
 [<span data-ttu-id="22b9a-117">Управление конфигурацией организации в журнале</span><span class="sxs-lookup"><span data-stu-id="22b9a-117">Manage Company Configuration in a Worksheet</span></span>](admin-how-to-manage-company-configuration-in-a-worksheet.md)
