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


В ходе решения задачи:
1. Построена логическая и физическая модель данных Primary Data Layer, Core Data Layer, Data Mart Layer в нотации 3 NF.
Инструменты: draw.io (блок фигур «Сущность-связь»)

![10](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/ba7756c9-7aa9-4f86-91f4-50099088a8a4)

Фрагмент. Core Data Layer
![02](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/a9aaaef3-6e8d-4319-9aa5-5c26631db06a) 

Фрагмент. Логическая модель данных Data Mart Layer составлена в нотации “Снежинка”.
![03](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/4cd65eac-245e-42c8-b957-321c24181cdd)

![11](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/e48f7e9b-d57b-41bb-bbd5-10c77b1d6dfe)

Фрагмент. Core Data Layer
![05](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/1852560e-b514-4858-9dae-09362de3f9d9)


2. Сформирована техническая спецификация Primary Data Layer, Core Data Layer, Data Mart Layer,
где описаны все системы-источники, таблицы с их атрибутами и их свойства.

3. Построена схема ETL процесса на базе технических спецификаций Raw Data Layer, Core Data Layer и Data Mart Layer.
   
![07](https://github.com/ElenaTratsevskaya/Planning-DWH-components-in-drawio/assets/110056199/9681fce0-d74c-4672-8ee3-11064478265f)



