---
title: Импорт транзакций по зарплате | Документация Майкрософт
description: Для управления зарплатой необходимо импортировать финансовые транзакции от поставщика заработной платы непосредственно в главную книгу, используя расширение для зарплаты, например Ceridian или Quickbooks.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Ceridian, Quickbooks, salary
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: b2bd2408152cac52be5e2b22e6568600ceeb96f6
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "5781585"
---
# <a name="import-payroll-transactions"></a><span data-ttu-id="ae59a-103">Импорт транзакций зарплаты</span><span class="sxs-lookup"><span data-stu-id="ae59a-103">Import Payroll Transactions</span></span>
<span data-ttu-id="ae59a-104">Для учета выплаты зарплаты и связанных транзакций необходимо импортировать и учесть финансовые транзакции, сделанные поставщиком системы зарплаты, в главную книгу.</span><span class="sxs-lookup"><span data-stu-id="ae59a-104">To account for salary payments and related transactions, you must import and post financial transactions made by your payroll provider to the general ledger.</span></span> <span data-ttu-id="ae59a-105">Чтобы это сделать, следует сначала импортировать файл, полученный от поставщика системы зарплаты, на страницу **Финансовый журнал**.</span><span class="sxs-lookup"><span data-stu-id="ae59a-105">To do this, you first import a file that you receive from the payroll provider into the **General Journal** page.</span></span> <span data-ttu-id="ae59a-106">Затем следует сопоставить внешние счета в файле зарплаты с соответствующими счетами ГК.</span><span class="sxs-lookup"><span data-stu-id="ae59a-106">Then you map the external accounts in the payroll file to the relevant G/L accounts.</span></span> <span data-ttu-id="ae59a-107">Наконец требуется учесть транзакции зарплаты в соответствии с сопоставлением счетов.</span><span class="sxs-lookup"><span data-stu-id="ae59a-107">Lastly, you post the payroll transactions according to the account mapping.</span></span>

> [!NOTE]  
>   <span data-ttu-id="ae59a-108">Чтобы воспользоваться этой функцией, расширение для импорта зарплаты необходимо установить и включить.</span><span class="sxs-lookup"><span data-stu-id="ae59a-108">To use this functionality, an extension for payroll import must be installed and enabled.</span></span> <span data-ttu-id="ae59a-109">Расширения "Зарплата Ceridian" и "Импорт файла зарплаты Quickbooks" предварительно установлены в [!INCLUDE[prod_short](includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="ae59a-109">The Ceridian Payroll and the Quickbooks Payroll File Import extensions are pre-installed in [!INCLUDE[prod_short](includes/prod_short.md)].</span></span> <span data-ttu-id="ae59a-110">Дополнительные сведения см. в разделе [Настройка [!INCLUDE[prod_short](includes/prod_short.md)] с помощью расширений](ui-extensions.md).</span><span class="sxs-lookup"><span data-stu-id="ae59a-110">For more information, see [Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md).</span></span>

## <a name="to-import-a-payroll-file"></a><span data-ttu-id="ae59a-111">Импорт файла зарплаты</span><span class="sxs-lookup"><span data-stu-id="ae59a-111">To import a payroll file</span></span>
1. <span data-ttu-id="ae59a-112">Выберите значок ![Лампочка, которая открывает функцию "Что вы хотите сделать"](media/ui-search/search_small.png "Что вы хотите сделать"), введите **Финансовые журналы**, затем выберите соответствующую ссылку.</span><span class="sxs-lookup"><span data-stu-id="ae59a-112">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **General Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="ae59a-113">В соответствующем разделе финансового журнала выберите действие **Импорт транзакций зарплаты**.</span><span class="sxs-lookup"><span data-stu-id="ae59a-113">In the relevant general journal batch, choose the **Import Payroll Transactions** action.</span></span> <span data-ttu-id="ae59a-114">Откроется руководство по сопровождаемой настройке.</span><span class="sxs-lookup"><span data-stu-id="ae59a-114">An assisted setup guide opens.</span></span>
3. <span data-ttu-id="ae59a-115">Выполните шаги на странице **Импорт транзакций зарплаты**.</span><span class="sxs-lookup"><span data-stu-id="ae59a-115">Follow the steps on the **Import Payroll Transactions** page.</span></span>

    > [!TIP]  
    >   <span data-ttu-id="ae59a-116">На шаге сопоставления внешних записей зарплаты со счетами ГК выполненные сопоставления будут отображаться при следующем импорте тех же записей.</span><span class="sxs-lookup"><span data-stu-id="ae59a-116">In the step about mapping the external payroll records to your G/L accounts, the mappings that you make will be remembered next time the same records are imported.</span></span> <span data-ttu-id="ae59a-117">Это экономит время, так как не требуется вручную заполнять поле **Номер счета** в финансовом журнале при каждом импорте повторяющихся транзакций зарплаты.</span><span class="sxs-lookup"><span data-stu-id="ae59a-117">This will save you time as you do not have to manually fill in the **Account No.** field in the general journal every time you have imported recurring payroll transactions.</span></span>   

    <span data-ttu-id="ae59a-118">При нажатии кнопки **ОК** в руководстве по сопровождаемой настройке страница **Финансовый журнал** будет заполнена строками, представляющими транзакции, содержащиеся в файле зарплаты, с соответствующими счетами, предварительно заполненными в полях **Счет ГК** в соответствии с сопоставлениями, выполненными в руководстве.</span><span class="sxs-lookup"><span data-stu-id="ae59a-118">When you choose the **OK** button in the assisted setup guide, the **General Journal** page is filled with lines representing the transactions that the payroll file contains and with the relevant accounts prefilled in the **G/L Account** fields according to mappings you made in the guide.</span></span>
4. <span data-ttu-id="ae59a-119">Отредактируйте или учтите строки журнала, как и для любых других транзакций главной книги.</span><span class="sxs-lookup"><span data-stu-id="ae59a-119">Edit or post the journal lines as for any other general ledger transactions.</span></span> <span data-ttu-id="ae59a-120">Дополнительные сведения см. в разделе [Учет транзакций непосредственно в главной книге](finance-how-post-transactions-directly.md).</span><span class="sxs-lookup"><span data-stu-id="ae59a-120">For more information, see [Post Transactions Directly to the General Ledger](finance-how-post-transactions-directly.md).</span></span>   

## <a name="see-also"></a><span data-ttu-id="ae59a-121">См. также</span><span class="sxs-lookup"><span data-stu-id="ae59a-121">See Also</span></span>
[<span data-ttu-id="ae59a-122">Финансы</span><span class="sxs-lookup"><span data-stu-id="ae59a-122">Finance</span></span>](finance.md)  
<span data-ttu-id="ae59a-123">[Настройка [!INCLUDE[prod_short](includes/prod_short.md)] с помощью расширений](ui-extensions.md)</span><span class="sxs-lookup"><span data-stu-id="ae59a-123">[Customizing [!INCLUDE[prod_short](includes/prod_short.md)] Using Extensions](ui-extensions.md)</span></span>  
[<span data-ttu-id="ae59a-124">Работа с финансовыми журналами</span><span class="sxs-lookup"><span data-stu-id="ae59a-124">Working with General Journals</span></span>](ui-work-general-journals.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]