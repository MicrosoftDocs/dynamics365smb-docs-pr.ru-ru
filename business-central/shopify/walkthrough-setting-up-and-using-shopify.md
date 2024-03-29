---
title: Настройка и использование соединителя Shopify
description: Различные сценарии интеграции для демонстрации рабочего процесса между Shopify и Business Central
ms.date: 06/21/2022
ms.topic: article
ms.service: dynamics-365-business-central
ms.search.form: '30101, 30102, 30106, 30107, 30113, 30115, 30126, 30156, 30157'
ms.reviewer: solsen
author: brentholtorf
ms.author: bholtorf
---

# <a name="walkthrough-set-up-and-use-the-shopify-connector"></a>Пошаговое руководство. Настройка и использование соединителя Shopify

В этом разделе демонстрируются некоторые типичные сценарии и проводятся шаги по тестированию или обучению пользователей рабочему процессу интегрированного [!INCLUDE[prod_short](../includes/prod_short.md)] и магазина Shopify.

## <a name="prerequisites"></a>Предварительные требования

### <a name="shopify"></a>Shopify

У вас должны быть:

- учетная запись Shopify
- интернет-магазин Shopify

Дополнительные сведения о создании пробных версий Shopify и рекомендуемых параметрах см. в статье [Создание и настройка учетной записи Shopify](shopify-account.md).

### <a name="business-central"></a>Business Central

Необходимо иметь учетную запись [!INCLUDE[prod_short](../includes/prod_short.md)]. 

Например, вы можете создать демонстрационную учетную запись или начать пробный период. Узнайте больше в разделах [Подготовка демонстрационных сред для Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/administration/demo-environment) и [Регистрация в пробной версии](../trial-signup.md). 

## <a name="connect-business-central-to-the-shopify-shop"></a>Подключение Business Central к магазину Shopify

В [!INCLUDE[prod_short](../includes/prod_short.md)] выполните следующие действия:

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Магазины Shopify**, а затем выберите соответствующую ссылку.
2. Выберите действие **Создать**.
3. В поле **Код** введите `DEMO1`.
4. В поле **URL-адрес Shopify** введите URL-адрес интернет-магазина, к которому вы хотите подключиться.
5. Активируйте переключатель **Включено**, а затем просмотрите и примите условия использования.

Чтобы настроить магазин Shopify, выполните следующие действия:

1. Выключите переключатель **Разрешить фоновые синхронизации**.
2. Выберите *В Shopify* в поле **Синхронизировать товар**.
3. Выберите *В Shopify* в поле **Синхронизировать изображения товара**.
4. Включите переключатель **Синхронизировать атрибуты товара**.
5. Включите переключатель **Отслеживание запасов**.
6. Выберите *Отклонить* в поле **Политика запасов по умолчанию** .
7. Включите переключатель **Автоматическое создание неизвестных клиентов**.
8. Заполните поле **Код шаблона клиента/организации** соответствующим шаблоном.
9. Заполните **Счет стоимости доставки**, **Счет чаевых** счетом доходов. Например, в США используйте `40210`.
10. Включите переключатель **Автоматическое создание заказов**.
11. Отключите переключатель **Автоматически выпускать заказы на продажу**.

Настройка сопоставлений складов:

1. Выберите действие **Склады**, чтобы открыть **Склады магазинов Shopify**.
2. Выберите действие **Получить склады Shopify** для импорта всех складов, определенных в Shopify. Выберите запись с включенным переключателем **Является основным**.
3. В **Фильтре по складу** введите `''|EAST|MAIN`.
4. Выберите *Прогнозируемый доступный остаток на сегодня* в поле **Расчет запасов**, чтобы включить синхронизацию запасов для выбранного склада Shopify.

## <a name="walkthrough-start-selling-products-online"></a>Пошаговое руководство. Начало продаж товаров в Интернете

### <a name="scenario"></a>Сценарий

Предположим, что вы хотите попробовать Shopify в качестве интернет-магазина, не тратя много времени на настройку, особенно поскольку вы уже ведете учет своих товаров в [!INCLUDE[prod_short](../includes/prod_short.md)]. После того как вы запустите свой интернет-магазин Shopify, вы сразу же получите новых клиентов, которые довольны вашим магазином и обслуживанием. Поэтому они решают оставить чаевые на кассе.

### <a name="steps"></a>Шаги

В [!INCLUDE[prod_short](../includes/prod_short.md)] выполните следующие действия:

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Продукты Shopify**, а затем выберите соответствующую ссылку.
2. Выберите **Добавить товары**.
3. В поле **Код магазина**введите `DEMO1`.
4. Установите фильтр `CHAIR` по полю **Код категории товара**.
5. Включите переключатель **Синхронизировать изображения продуктов**.
6. Включите переключатель **Синхронизировать запасы**.
7. Выберите **ОК** и дождитесь завершения начальной синхронизации товаров, цен, изображений и запасов.

В **интернет-магазине Shopify**:
> [!Tip]  
> Откройте **портал администрирования Shopify**, перейдя по URL-адресу, указанному в поле **URL-адрес** страницы **Карточка магазина Shopify**. Выберите значок глаза рядом с каналом продаж **Online Store**, расположенным на боковой панели **портале администрирования Shopify**. 

Откройте каталог продуктов. Примечание.

* Названия продуктов, их изображения и цены.
* Индикатор наличия (распродано для товаров, которых нет в наличии).

Выберите любой товар, который можно продать, например `BERLIN Swivel Chair, yellow`. Обратите внимание, что описание содержит атрибуты товара.

Выберите **Buy it now** и переходите к оформлению заказа.

1. В поле **Email or mobile phone number** введите `cl@contoso.com` (или адрес электронной почты, на который вы хотите получать подтверждения заказа и доставки).
2. В полях **First name** и **Last name** введите `Claudia Lawson`.
3. Введите местный адрес.
4. Установите флажок **Save this information for next time**.
6. Оставьте *Standard* в качестве способа доставки.
8. В поле **Credit Card number** введите `1`, если вы используете *(for testing) Bogus Gateway*, либо введите `5555 5555 5555 4444`, если вы используете *Shopify Payments* в тестовом режиме.
9. Заполните поле **Name on card**.
10. В поле **Expiration date** введите текущие месяц/год.
11. В поле **Security code** введите `111`.
7. (Необязательно) Выберите чаевые в размере `10%`.
8. 12. Выберите **Pay now**.

В [!INCLUDE[prod_short](../includes/prod_short.md)] выполните следующие шаги:

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы Shopify**, а затем выберите соответствующую ссылку.
2. Выберите действие **Синхронизировать заказы из Shopify**.
3. Нажмите **ОК**.

Импортированный заказ готов к обработке.

1. Выберите импортированный заказ, чтобы открыть окно **Заказ Shopify**.
2. Будут созданы новый клиент и заказы на продажу.
3. Ознакомьтесь с действиями **Риск** и **Стоимость доставки**.
4. Выберите **Заказ на продажу**, чтобы открыть окно **Заказ на продажу**. Заказ на продажу — это потребность, которая при необходимости может быть покрыта сборкой, производством или закупкой с помощью механизма планирования. Он также поддерживает различные процессы складской обработки с полным разделением обязанностей.
6. В поле **Агент** введите `DHL`. При необходимости повторно откройте заказ, выбрав действие **Открыть**.
7. В поле **Номер трасс. посылки** введите `123456789`.
8. Выберите действие **Учет**, оставьте выбранным вариант **Отгрузить и выставить счет** и выберите **ОК**.

Теперь физические и финансовые данные регистрируются в [!INCLUDE[prod_short](../includes/prod_short.md)]. Пришло время сообщить Shopify об изменениях.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Синхронизировать отгрузки в Shopify**, а затем выберите соответствующую ссылку.
2. Нажмите **ОК**.

На **портале администрирования Shopify** обратите внимание, что заказ теперь помечен как *выполненный*. Вы также можете просмотреть сведения о доставке и увидеть там URL-адрес отслеживания. Если вы снова запустите **Синхронизировать заказы из Shopify**, заказ будет заархивирован в обеих системах.

## <a name="walkthrough-add-your-customers-to-your-new-online-store"></a>Пошаговое руководство. Добавление клиентов в новый интернет-магазин

### <a name="scenario-1"></a>Сценарий

После успешного быстрого запуска нового интернет-магазина вам нужно, чтобы ваши текущие клиенты посетили его и начали делать заказы. В зависимости от вашего плана Shopify и специфики работы вы можете попробовать процессы B2B и D2C.

### <a name="d2c-steps"></a>Процесс D2C

В [!INCLUDE[prod_short](../includes/prod_short.md)] выполните следующие действия:

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиенты Shopify**, а затем выберите соответствующую ссылку.
2. Выберите **Добавить клиентов**.
3. В поле **Код магазина**введите `DEMO1`.
4. Установите фильтр `20000` по полю **№**. .
5. Выберите **ОК** и дождитесь завершения начальной синхронизации клиентов.

На **портале администрирования Shopify** обратите внимание, что клиент был импортирован. Откройте клиентов и обратите внимание, что имя и фамилия клиента взяты из поля **Имя контакта** в **Карточке клиента**. Название компании можно найти в адресе по умолчанию, связанном с клиентом. Если вы используете классические учетные записи клиентов (*Classic customer accounts*), вы можете выбрать **Send account invite**, чтобы пригласить клиента. Если вы используете новые учетные записи клиентов (*New customer accounts*), клиентам не нужен пароль для входа; вместо этого Shopify предоставляет вашим клиентам входить в систему с использованием одноразового 6-значного проверочного кода, отправляемого по электронной почте. 

### <a name="b2b-steps"></a>Процесс B2B

[!INCLUDE [shopify-preview](../includes/shopify-preview.md)]

В [!INCLUDE[prod_short](../includes/prod_short.md)] выполните следующие действия:

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Организации Shopify**, а затем выберите соответствующую ссылку.
2. Выберите **Добавить организацию**.
3. В поле **Код магазина**введите `DEMO1`.
4. Установите фильтр `30000` по полю **№**. .
5. Выберите **ОК** и дождитесь завершения начальной синхронизации клиентов.

На **портале администрирования Shopify** обратите внимание, чтобы были импортированы и организация, и клиент. Откройте клиентов и обратите внимание на информационную панель «Организация» со ссылкой на организацией, местоположением и назначенными разрешениями. Выберите **[...]** на информационной панели **Организация**, затем выберите **Отправить сообщение электронной почты с данными для доступа B2B**, чтобы пригласить клиента.

## <a name="walkthrough-fine-tuning-of-item-management"></a>Пошаговое руководство. Тонкая настройка управления товарами

### <a name="scenario-2"></a>Сценарий

Вы хотели бы добавить больше гибкости и контроля в свои процессы, связанные с управлением товарами. Вам нужно улучшить описания продуктов, и вы хотели бы добавить дополнительные этапы проверки, прежде чем продукты станут доступными всем клиентам.

### <a name="steps-1"></a>Шаги

В [!INCLUDE[prod_short](../includes/prod_short.md)] выполните следующие действия:

Подготовка данных.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Ценовая группа клиента**, а затем выберите соответствующую ссылку.
2. Добавьте новую ценовую группу. В поле **Код** введите `SHOPIFY`.
3. Закройте окно **Ценовая группа клиентов**.
4. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, а затем выберите соответствующую ссылку.
5. Выберите товар *1896-S, Athens Desk* и выполните следующие действия:

6. Выберите действие **Варианты**, а затем добавьте два варианта: `PREMIUM, Athens Desk, Premium edition` и `ESSENTIAL, Athens Desk, Essential edition`.
7. Выберите действие **Маркетинговый текст** и используйте вариант **Создать черновик с помощью Copilot**, чтобы получить креативный и увлекательный текст. Если предлагаемые маркетинговые тексты не включены, просто введите: «**Простой стильный дизайн** сочетается с любым ансамблем. *Доступно в двух вариантах.*». 
8. Выберите действие **Цены продажи** и добавьте новые цены, как показано в следующей таблице:

   |График|Тип продажи|Код продажи|Тип|Код|Код варианта<br>(добавление поля через персонализацию)|Цена единицы|
   |------|------------|------------|------------|----------------|------------|------------|
   |1|Ценовая группа клиентов|SHOPIFY|Пункт меню|1896-S|ESSENTIAL|700|
   |2|Ценовая группа клиентов|SHOPIFY|Пункт меню|1896-S|PREMIUM|1000|

9. Выберите действие **Торговые скидки** и добавьте новую скидку:

   * **Тип продажи** *Скидочная группа клиента*
   * **Код продажи** *РОЗНИЦА*
   * **Тип** *Товар*
   * **Код** *1896-S*
   * **Код единицы измерения** *ШТ.*
   * **Скидка строки %** *10*

10. Выберите действие **Ссылки на товары** и добавьте следующие строки:

   |График|Тип ссылки|Номер ссылки|Код варианта|
   |------|------------|------------|------------|
   |1|Штрихкод|77777777|ESSENTIAL|
   |2|Штрихкод|11111111|PREMIUM|

11. Выберите товар *1920-S, ANTWERP Conference Table* и выполните следующие действия:
12. Выберите **Корректировать запасы** и в поле **Новые запасы** введите `100` для складов *EAST* и *WEST*. 
13. Нажмите **ОК**.

Настройка параметров синхронизации.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Магазины Shopify** и выберите соответствующую ссылку.
2. Выберите магазин `DEMO1`, для которого вы хотите синхронизировать товары, чтобы открыть страницу **Карточка магазина Shopify**.
3. Включите поле **Синхронизировать маркетинговый текст**.
4. Выберите *Номер товара + Код варианта* в поле **Сопоставление SKU**.
5. Выберите *Продолжить* в поле **Политика запасов по умолчанию**.
6. Выберите *Черновик* в поле **Статус созданных продуктов**.
7. Выберите *Статус в архиве* в поле **Действие для удаленного продукта**.
8. Выберите *SHOPIFY* в поле **Ценовая группа клиента**.
9. Выберите *РОЗНИЦА* в поле **Скидочная группа клиента**.
 
Выполните синхронизацию.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Магазины Shopify** и выберите соответствующую ссылку.
2. Выберите магазин `DEMO1`, для которого вы хотите синхронизировать товары, чтобы открыть страницу **Карточка магазина Shopify**.
3. Выберите **Продукты**, чтобы открыть окно **Продукты Shopify**.
4. Выберите действие **Добавить товары**.
5. Установите фильтр *СТОЛ|ПАРТА* в поле **Код категории товара**.
6. Включите переключатель **Синхронизировать изображения продуктов**.
7. Включите переключатель **Синхронизировать запасы**.
8. Выберите **ОК** и дождитесь завершения начальной синхронизации товаров, цен, изображений и запасов.

Будут добавлены продукты. Обратите внимание, что для статуса установлено *Черновик*, поэтому товары не отображаются в интернет-магазине Shopify.

1. Выберите строку с товаром *1920-S, ANTWERP Conference Table*. В **Название для SEO** введите `Rectangular meeting table Antwerp, 10 seats, black`.
2. Выберите *Активно* в поле **Статус**.
3. Выберите строку с товаром *1906-S, ATHENS, Mobile Pedestal*, а затем выберите действие **Удалить**.

На **портале администрирования Shopify** обратите внимание, что все продукты имеют разные статусы.

* *ANTWERP Conference Table* имеет статус *Active*, потому что мы изменили статус этого товара в окне **Продукт Shopify**.
* *ATHENS Desk* имеет статус *Draft*, потому что мы настроили в качестве статуса по умолчанию для всех добавленных продуктов *Черновик*.
* *ATHENS Mobile Pedestal* имеет статус *Archived*, потому что мы настроили магазин на автоматическое присвоение статуса *Archived* для удаленных продуктов.

Обратите внимание, что запасы товара ANTWERP Conference Table составляют 100, потому что мы настроили систему для использования запасов только с двух складов (MAIN и EAST). Запасы в третьем складе (WEST) игнорируются.

* Откройте *ANTWERP Conference Table* и обратите внимание на поля **Custom Type**, **Vendor**, **Weight** и **Cost per item**, а также на раздел **Search engine listing preview**.
* Откройте *Athens Desk*, прокрутите вниз до раздела **Variants** и обратите внимание, как заполнено поле **SKU**.
* Выберите **Edit**, чтобы просмотреть штрих-код и цены.
* Измените статус товара *Athens Desk* на *Active* и выберите действие **Preview**.

В **интернет-магазине Shopify** откройте каталог товаров и найдите товар *ATHENS Desk*. Обратите внимание, что доступны различные варианты. Для разных вариантов цены являются разными. Обратите внимание на информацию о скидках.

### <a name="additional-steps-for-b2b"></a>Дополнительные шаги для B2B

[!INCLUDE [shopify-preview](../includes/shopify-preview.md)]

Вы можете настроить соединитель для автоматического создания и назначения каталога экспортируемым организациям. Инструкции ниже будут полезны, если вы хотите в большей степени контролировать то, что доступно вашим B2B-клиентам.

На **портале администрирования Shopify** создайте и назначьте каталог.

1. Выберите **Products** и затем **Catalogs** на боковой панели **портала администрирования Shopify**.
2. Создайте каталог для конкретных продуктов. Назовите его «B2B». 
3. Выберите **Manage** и затем **Manage products and pricing**.
4. Выберите фильтр *Excluded* фильтр, найдите *ATHERN Desk* и выберите **Include in catalog**.
5. Выберите **Customers** и затем **Companies** на боковой панели **портала администрирования Shopify**.
6. Выберите *School of Fine Art*, выберите **[...]** и затем **Add catalogs**, после чего добавьте созданный ранее каталог *B2B*.

В [!INCLUDE[prod_short](../includes/prod_short.md)] выполните следующие действия:

Подготовка данных.

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товары**, а затем выберите соответствующую ссылку.

2. Выберите товар **1896-S, Athens Desk** и выполните следующие действия:

3. Выберите действие **Торговые скидки** и добавьте новую скидку:

   * **Тип продажи** *Скидочная группа клиента*
   * **Код продаж** *КРУПКЛИЕНТ*
   * **Тип** *Товар*
   * **Код** *1896-S*
   * **Код единицы измерения** *ШТ.*
   * **Скидка строки %** *25*

4. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Каталоги Shopify**, а затем выберите соответствующую ссылку.
5. Выберите **Получить каталоги**.
6. В поле **Код магазина**введите `DEMO1`.
7. Выберите запись каталога с именем *B2B*, для которого вы хотите синхронизировать цены.
8. Включите переключатель **Синхронизировать цены**.
9. Выберите *SHOPIFY* в поле **Ценовая группа клиента**.
10. Выберите *КРУПКЛИЕНТ* в поле **Скидочная группа клиента**.
11. Выберите **Синхронизировать цены** и дождитесь завершения синхронизации цен.

На **портале администрирования Shopify** проверьте цены на товары из каталога *B2B*.

В **интернет-магазине Shopify** откройте каталог товаров и найдите товар *ATHENS Desk*. Обратите внимание, что цены содержат информацию о скидках.

## <a name="walkthrough-check-out-and-order-synchronization-for-individual-buyer-and-company-representative"></a>Пошаговое руководство. Оформление заказа и синхронизация заказа для индивидуального покупателя и представителя организации
Это продолжение [Пошагового руководства: начало продаж товаров в Интернете](walkthrough-setting-up-and-using-shopify.md#walkthrough-start-selling-products-online). Вы также можете попробовать использовать собственные данные — например, свой магазин Shopify или песочницу.

Индивидуальный покупатель

1. В **интернет-магазине Shopify**: Выберите значок **Account**. Введите адрес электронной почты, к которому у вас есть доступ.
2. Войдите в систему, используя одноразовый 6-значный проверочный код, отправленный на введенный вами адрес электронной почты.
3. Изучите каталог продукции; вы должны видеть все товары с розничными ценами.
4. Выберите вариант Essential, выберите **Buy it now** и переходите к оформлению заказа.
5. Заполните поле **First name** и **Last name**.
6. Введите местный адрес.
7. Оставьте *Standard* в качестве способа доставки.
8. В поле **Credit Card Number** введите `1`, если вы используете *(for testing) Bogus Gateway*, либо введите `5555 5555 5555 4444`, если вы используете *Shopify Payments* в тестовом режиме.
9. В поле **Expiration date** введите текущие месяц/год.
10. В поле **Security code** введите `111`.
11. Заполните поле **Name on card**.
12. Выберите **Pay now**.
 
Представитель организации

[!INCLUDE [shopify-preview](../includes/shopify-preview.md)]

1. На **портале администрирования Shopify**:
2. Выберите **Customers** и затем **Companies** на боковой панели **портала администрирования Shopify**.
3. Откройте запись *School of Fine Art*.
4. Выберите **[...]** на информационной панели **School of Fine Art**, выберите **Edit payment terms** и выберите *Due on fulfillment*.
5. Выберите **[...]** на информационной панели **Customers**, выберите **Add customer** и добавьте клиента с адресом электронной почты, который вы использовали для входа в магазин.
6. В **интернет-магазине Shopify**: Выберите значок **Account**. Введите адрес электронной почты, к которому у вас есть доступ.
7. Войдите в систему, используя одноразовый 6-значный проверочный код, отправленный на введенный вами адрес электронной почты.
8. Изучите каталог продукции. Вы должны видеть только товары, добавленные в каталог *B2B*, со специальными розничными ценами.
9. Выберите вариант Essential, выберите **Buy it now** и переходите к оформлению заказа.
10. Обратите внимание, что учетная запись, адрес доставки и способ оплаты заполнены.
11. В поле **PO Number** введите `PO-12345`.
12. Выберите **Submit order**.
 
В [!INCLUDE[prod_short](../includes/prod_short.md)] выполните следующие шаги:

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Заказы Shopify**, а затем выберите соответствующую ссылку.
2. Выберите действие **Синхронизировать заказы из Shopify**.
3. Нажмите **ОК**.

Импортированный заказ готов к обработке.

1. Выберите импортированный заказ, чтобы открыть окно **Заказ Shopify**.
2. Обратите внимание, что несмотря на то что оба заказа были отправлены одним и тем же человеком, они связаны с двумя разными клиентами. 
3. В заказе, отправленном от имени организации, вы видите значение в поле **Номер ЗнП**, которое также переносится в поле **№ внешнего документа** созданного документа продажи.
4. Потому что мы настроили организацию B2B для обработки платежей за пределами Shopify, в поле **Финансовый статус** установлено значение *Ожидание*. После получения оплаты выберите действие **Пометить как оплаченный**. Финансовый статус в Shopify будет обновлен. 

## <a name="walkthrough-import-items-customers-companies-from-shopify"></a>Пошаговое руководство. Импорт товаров, клиентов и организаций из Shopify

### <a name="scenario-3"></a>Сценарий

У вас уже есть успешный интернет-магазин, и вы хотели бы начать использовать [!INCLUDE[prod_short](../includes/prod_short.md)] в качестве программного обеспечения для управления бизнесом. Вам нужно импортировать как можно больше данных из Shopify. 

### <a name="steps-2"></a>Шаги

Это продолжение пошаговых руководств [Начало продаж товаров в Интернете](walkthrough-setting-up-and-using-shopify.md#walkthrough-start-selling-products-online) и [Добавление клиентов в новый интернет-магазин](walkthrough-setting-up-and-using-shopify.md#walkthrough-add-your-customers-to-your-new-online-store). Вы также можете попробовать использовать собственные данные — например, свой магазин Shopify или песочницу.

В [!INCLUDE[prod_short](../includes/prod_short.md)] выполните действия, перечисленные ниже.

#### <a name="prepare-data"></a>Подготовка данных

1. Перейдите на бесплатную 30-дневную пробную версию без примеров данных. Дополнительную информацию см. в разделе [Добавление собственных данных в пустую пробную версию](/dynamics365/business-central/dev-itpro/administration/trials-subscriptions#add-your-own-data-to-an-empty-trial-company).
2. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Магазины Shopify**, а затем выберите соответствующую ссылку.
3. Выберите **Создать**.
4. В поле **Код** введите `DEMO2`.
5. В поле **URL-адрес Shopify** введите URL-адрес интернет-магазина, к которому вы хотите подключиться.
6. Активируйте переключатель **Включено**, а затем просмотрите и примите условия использования.

Настройте магазин Shopify следующим образом:

1. Выключите переключатель **Разрешить фоновые синхронизации**.
2. Выберите *Из Shopify* в поле **Синхронизировать товар**.
3. Включите переключатель **Автоматически создавать неизвестные товары**.
4. Заполните поле **Код шаблона товара** соответствующим шаблоном.
5. Выберите *Из Shopify* в поле **Синхронизировать изображения товара**.
6. Выберите *Номер товара + Код варианта* в поле **Сопоставление SKU**.
7. Выберите *Все клиенты* в **Импорт клиентов из Shopify**
8. Включите переключатель **Автоматически создавать неизвестных клиентов**.
9. Заполните поле **Код шаблона клиента/организации** соответствующим шаблоном.
10. Выберите *Все клиенты* в **Импорт организаций из Shopify**
11. Включите переключатель **Автоматически создавать неизвестные организации**.

#### <a name="run-the-synchronization"></a>Выполните синхронизацию

1. Выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Магазины Shopify** и выберите соответствующую ссылку.
2. Выберите магазин *DEMO2*, для которого вы хотите синхронизировать данные, чтобы открыть страницу **Карточка магазина Shopify**.
3. Выберите **Синхронизировать продукты**.
4. Выберите **Синхронизировать изображения продуктов**.
5. Выберите **Синхронизировать клиентов**.
6. Выберите **Синхронизировать организации**

### <a name="results"></a>Результаты

* Продукты Shopify импортированы. Чтобы это проверить, выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Продукты Shopify**, а затем выберите соответствующую ссылку.
* Созданы товары с изображениями. Чтобы это проверить, выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Товар**, а затем выберите соответствующую ссылку.
* Клиенты Shopify импортированы. Чтобы это проверить, выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиенты Shopify**, а затем выберите соответствующую ссылку.
* Организации Shopify импортируются. Чтобы это проверить, выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Организации Shopify**, а затем выберите соответствующую ссылку.
* Клиенты созданы. Чтобы это проверить, выберите значок ![Лампочка, которая открывает функцию Что вы хотите сделать.](../media/ui-search/search_small.png "Что вы хотите сделать"), введите **Клиенты**, а затем выберите соответствующую ссылку.


## <a name="see-also"></a>См. также

[Начало работы с соединителем Shopify](get-started.md)  
