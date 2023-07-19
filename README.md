# Planning-DWH-components-in-drawio
Creation of logical, physical data model, ETL process mapping and technical specification<br>

**Создание логической, физической модели данных, построение схемы ETL-процессов и создание технической спецификации**

**Контекст**

Интернет-магазин
1. Покупатель выбирает несколько продуктов из каталога. При оформлении заказа покупатель регистрируется на сайте интернет-магазина, указывая свой номер телефона, email и ФИО. 
При добавлении адреса доставки в заказ определяется конечная стоимость.
Покупатель также может сформировать возврат по заказу, указав причину. Возврат может быть оформлен только на весь заказ.

2. Отделу продаж необходимо знать, какая выручка по каждому продукту и по категории продуктов в месяц.
Данные о покупателях формируются в Auth системе (системе авторизации пользователей) в виде таблицы «Покупатели».
Данные о заказах и продуктах формируются в CRM системе в виде соответствующих таблиц «Заказы» и «Продукты».
Данные о возвратах находятся в CRM-системе в таблице «Возвраты»


**В ходе решения задачи:**<br>
**1**. Построена логическая и физическая модель данных Primary Data Layer, Core Data Layer, Data Mart Layer в нотации 3 NF.
Инструменты: draw.io (блок фигур «Сущность-связь»)

Логическая модель данных
![01_ЛМ_all](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/585560d2-964d-45ab-bbb0-f8264159d274)

Логическая модель данных. Фрагмент. Core Data Layer
![01_ЛМ_CDL](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/315f9eee-e7a8-45bb-9f55-8930d8967e79)

Фрагмент. Логическая модель данных Data Mart Layer составлена в нотации “Снежинка”.
![01_ЛМ_PDL](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/e7bce599-42bf-4968-bf45-d8605e4820f8)


Физическая модель данных
![01_ФМ_all](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/210b0766-7eb1-4e06-92a8-937544b82191)

Физическая модель данных. Фрагмент. Core Data Layer
![01_ФМ_CDL](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/bfaca12b-2b2c-40db-87fe-66b653ef356c)

Физическая модель данных. Фрагмент. Data Mart Layer
![01_ФМ_DML](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/aea7f95a-4686-4a31-80a5-e90f62128f47)


**2**. Сформирована техническая спецификация Primary Data Layer, Core Data Layer, Data Mart Layer,
где описаны все системы-источники, таблицы с их атрибутами и их свойства.<br>
[Техническая спецификация](https://docs.google.com/spreadsheets/d/1rmjF3JnWS4qaNOHGLw4pU8uCdbpPnQrhwlYntRFxiyw/edit#gid=381670597)
представлена в Гугл-таблицах, всё на отдельных листах, листы подписаны: Primary Data Layer, Core Data Layer, Data Mart Layer,
навигация по цвету и соотвествует контурам схемы и заливке под заголовком в моделях данных.

**3**. Построена схема ETL процесса на базе технических спецификаций Raw Data Layer, Core Data Layer и Data Mart Layer.
![02](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/6f0f0891-567b-4d94-8078-0a270daad4af)





