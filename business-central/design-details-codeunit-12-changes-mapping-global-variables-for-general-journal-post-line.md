---
title: Сведения о проектировании — изменения модуля codeunit 12 в сопоставлении глобальных переменных для строки учета финансового журнала | Документация Майкрософт
description: В этом выпуске Business Central реализованы следующие изменения.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 513518f7e76fcdbb43563d225c683a8bd97e5e4e
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "3917455"
---
# <a name="codeunit-12-changes-mapping-global-variables-for-general-journal-post-line"></a>Изменения модуля codeunit 12: сопоставление глобальных переменных для строки учета финансового журнала
В этом выпуске [!INCLUDE[d365fin](includes/d365fin_md.md)] реализованы следующие изменения.  

|**Microsoft Dynamics NAV 2009 R2**|**Microsoft Dynamics NAV 2013 R2**|**Комментарий**|  
|----------------------------------------|----------------------------------------|-----------------|  
|GLSetup@1009 : Record 98;|GLSetup@1009 : Record 98;|Не изменено|  
|SalesSetup@1010 : Record 311;||Изменено на локальное|  
|PurchSetup@1011 : Record 312;||Изменено на локальное|  
|AccountingPeriod@1012 : Record 50;||Изменено на локальное|  
|GLAcc@1013 : Record 15;||Изменено на локальное|  
|GLEntry@1014 : Record 17;|GlobalGLEntry@1014 : Record 17;|Переименовано|  
|GLEntryTmp@1015 : TEMPORARY Record 17;|TempGLEntryBuf@1010 : TEMPORARY Record 17;|Переименовано|  
|TempGLEntryVAT@1016 : TEMPORARY Record 17;|TempGLEntryVAT@1016 : TEMPORARY Record 17;|Не изменено|  
|OrigGLEntry@1017 : Record 17;||Удалено|  
|VATPostingSetup@1019 : Record 325;||Изменено на локальное|  
|Cust@1020 : Record 18;||Изменено на локальное|  
|Vend@1021 : Record 23;||Изменено на локальное|  
|GenJnlLine@1022 : Record 81;||Изменено на локальное|  
|GLReg@1029 : Record 45;|GLReg@1029 : Record 45;|Не изменено|  
|CustPostingGr@1030 : Record 92;||Изменено на локальное|  
|VendPostingGr@1031 : Record 93;||Изменено на локальное|  
|Currency@1032 : Record 4;||Изменено на локальное|  
|AddCurrency@1033 : Record 4;|AddCurrency@1033 : Record 4;|Не изменено|  
|ApplnCurrency@1034 : Record 4;||Изменено на локальное|  
|CurrExchRate@1035 : Record 330;|CurrExchRate@1035 : Record 330;|Не изменено|  
|VATEntry@1038 : Record 254;|VATEntry@1038 : Record 254;|Не изменено|  
|BankAcc@1039 : Record 270;||Изменено на локальное|  
|BankAccLedgEntry@1040 : Record 271;||Изменено на локальное|  
|CheckLedgEntry@1041 : Record 272;||Изменено на локальное|  
|CheckLedgEntry2@1042 : Record 272;||Изменено на локальное|  
|BankAccPostingGr@1043 : Record 277;||Изменено на локальное|  
|GenJnlTemplate@1044 : Record 80;||Изменено на локальное|  
|TaxJurisdiction@1045 : Record 320;||Изменено на локальное|  
|TaxDetail@1046 : Record 322;|TaxDetail@1046 : Record 322;|Не изменено|  
|FAGLPostBuf@1047 : TEMPORARY Record 5637;||Изменено на локальное|  
|UnrealizedCustLedgEntry@1084 : Record 21;|UnrealizedCustLedgEntry@1084 : Record 21;|Не изменено|  
|UnrealizedVendLedgEntry@1085 : Record 25;|UnrealizedVendLedgEntry@1085 : Record 25;|Не изменено|  
|GLEntryVATEntryLink@1087 : Record 253;|GLEntryVATEntryLink@1087 : Record 253;|Не изменено|  
|TempVATEntry@1088 : TEMPORARY Record 254;|TempVATEntry@1088 : TEMPORARY Record 254;|Не изменено|  
|ReversedGLEntryTemp@1089 : TEMPORARY Record 17;||Перемещено в модуль Codeunit 17|  
|CostAccSetup@1092 : Record 1108;||Изменено на локальное|  
|GenJnlCheckLine@1048 : Codeunit 11;|GenJnlCheckLine@1001 : Codeunit 11;|Не изменено|  
|ExchAccGLJnlLine@1049 : Codeunit 366;||Изменено на локальное|  
|FAJnlPostLine@1050 : Codeunit 5632;||Изменено на локальное|  
|SalesTaxCalculate@1051 : Codeunit 398;||Изменено на локальное|  
|GenJnlApply@1052 : Codeunit 225;||Изменено на локальное|  
|DimMgt@1053 : Codeunit 408;||Изменено на локальное|  
|JobPostLine@1028 : Codeunit 1001;||Изменено на локальное|  
|TransferGlEntriesToCA@1091 : Codeunit 1105;||Изменено на локальное|  
||PaymentToleranceMgt@1002 : Codeunit 426;|Добавление|  
||AddCurrencyCode@1117 : Code[10];|Добавление|  
|FiscalYearStartDate@1054 : Date;|FiscalYearStartDate@1011 : Date;|Не изменено|  
|NextEntryNo@1055 : Integer;|NextEntryNo@1022 : Integer;|Не изменено|  
|BalanceCheckAmount@1056 : Decimal;|BalanceCheckAmount@1056 : Decimal;|Не изменено|  
|BalanceCheckAmount2@1057 : Decimal;|BalanceCheckAmount2@1057 : Decimal;|Не изменено|  
|BalanceCheckAddCurrAmount@1058 : Decimal;|BalanceCheckAddCurrAmount@1058 : Decimal;|Не изменено|  
|BalanceCheckAddCurrAmount2@1059 : Decimal;|BalanceCheckAddCurrAmount2@1059 : Decimal;|Не изменено|  
|CurrentBalance@1060 : Decimal;|CurrentBalance@1060 : Decimal;|Не изменено|  
|SalesTaxBaseAmount@1061 : Decimal;||Изменено на локальное|  
|TotalAddCurrAmount@1062 : Decimal;|TotalAddCurrAmount@1062 : Decimal;|Не изменено|  
|TotalAmount@1063 : Decimal;|TotalAmount@1063 : Decimal;|Не изменено|  
|UnrealizedRemainingAmountCust@1086 : Decimal;|UnrealizedRemainingAmountCust@1086 : Decimal;|Не изменено|  
|UnrealizedRemainingAmountVend@1074 : Decimal;|UnrealizedRemainingAmountVend@1074 : Decimal;|Не изменено|  
|NextVATEntryNo@1064 : Integer;|NextVATEntryNo@1064 : Integer;|Не изменено|  
|FirstNewVATEntryNo@1065 : Integer;|FirstNewVATEntryNo@1065 : Integer;|Не изменено|  
|NextTransactionNo@1066 : Integer;|NextTransactionNo@1066 : Integer;|Не изменено|  
|NextConnectionNo@1067 : Integer;|NextConnectionNo@1067 : Integer;|Не изменено|  
|InsertedTempGLEntryVAT@1068 : Integer;|InsertedTempGLEntryVAT@1027 : Integer;|Не изменено|  
|LastDocNo@1069 : Code[20];|LastDocNo@1023 : Code[20];|Не изменено|  
|LastLineNo@1070 : Integer;||Удалено|  
|LastDate@1071 : Date;|LastDate@1021 : Date;|Не изменено|  
|LastDocType@1072 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';|LastDocType@1025 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';|Не изменено|  
|NextCheckEntryNo@1073 : Integer;|NextCheckEntryNo@1028 : Integer;|Не изменено|  
|AddCurrGLEntryVATAmt@1075 : Decimal;|AddCurrGLEntryVATAmt@1017 : Decimal;|Не изменено|  
|CurrencyDate@1076 : Date;|CurrencyDate@1020 : Date;|Не изменено|  
|CurrencyFactor@1077 : Decimal;|CurrencyFactor@1019 : Decimal;|Не изменено|  
|UseCurrFactorOnly@1078 : Boolean;|UseCurrFactorOnly@1078 : Boolean;|Не изменено|  
|NonAddCurrCodeOccured@1079 : Boolean;|NonAddCurrCodeOccured@1079 : Boolean;|Не изменено|  
|FADimAlreadyChecked@1080 : Boolean;|FADimAlreadyChecked@1080 : Boolean;|Не изменено|  
|AllApplied@1081 : Boolean;||Изменено на локальное|  
|OverrideDimErr@1018 : Boolean;|OverrideDimErr@1018 : Boolean;|Не изменено|  
|JobLine@1036 : Boolean;|JobLine@1036 : Boolean;|Не изменено|  
|Prepayment@1037 : Boolean;||Удалено|  
|CheckUnrealizedCust@1082 : Boolean;|CheckUnrealizedCust@1082 : Boolean;|Не изменено|  
|CheckUnrealizedVend@1083 : Boolean;|CheckUnrealizedVend@1083 : Boolean;|Не изменено|  
|GLEntryNo@1090 : Integer;|GLEntryNo@1026 : Integer;|Не изменено|  
||GLSetupRead@1015 : Boolean;|Добавление|  
||AmountRoundingPrecision@1012 : Decimal;|Добавление|  
||CrCardTransactionEntryNo@1013 : Integer;|Добавление|  

## <a name="see-also"></a>См. также  
 [Сведения о проектировании. Изменения модуля codeunit 12: изменения в процедурах учета финансовых журналов](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)
