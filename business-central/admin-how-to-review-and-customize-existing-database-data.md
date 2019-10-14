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
# <a name="review-and-customize-existing-database-data"></a>Просмотр или настройка существующих данных базы данных
По мере создания пакета конфигурации для решения можно просматривать и настраивать доступные данные в базе данных в соответствии с потребностями клиента. Таблица базы данных должна иметь соответствующую страницу.  

### <a name="to-customize-data-in-the-database"></a>Настройка данных в базе данных  

1.  В журнале конфигураций определите таблицы, данные которых необходимо просмотреть или изменить.  

    > [!NOTE]  
    >  Убедитесь, что каждая таблица имеет код страницы, присвоенный ей. Для стандартных таблиц [!INCLUDE[d365fin](includes/d365fin_md.md)] это значение заполняется автоматически. В случае пользовательских таблиц вам следует указать код.  

2.  На вкладке **Действия** в группе **Показать** выберите **Данные из базы данных**.  

     Откроется страница [!INCLUDE[d365fin](includes/d365fin_md.md)] для этой страницы.  

3.  Просмотрите имеющуюся информацию. Измените его по мере необходимости путем удаления ненужных записей или добавления новых.  

## <a name="see-also"></a>См. также  
 [Управление конфигурацией организации в журнале](admin-how-to-manage-company-configuration-in-a-worksheet.md)
