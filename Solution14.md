**Рефлексия на задачи из занятия 13:**</br>
В задании 13.3.1. интересное решение с обращением к стоку из таблицы Products. Взял на заметку.</br>
В задании 13.3.2. использовал AND вместо OR, хотя, наверное в рамках конкретно этой таблицы это не страшно, но все может зависеть от контекста.</br>
В задании 13.3.3. так и думал что надо удаление делать по PK-ключу, подтвердились мои предположения.

**Решение на задачи занятия 14:**</br>
14.1. В представлении отсутсвуют поля EmloyeeID и ShipVia, однако присутсвует дополнительная информация из полей CompanyName, Address, City, Region, PostalCode и Country таблицы заказчиков Customer, добавлена информация из полей ProductID, UnitPrice, Quantity и Discount таблицы детализации заказов Order Details, добавлено поле с названием компании доставки, поле наименования продукта, имя и фамилия сотрудника ведущего заказ и добавлена итоговая цена по заказу. В целом, представление содержит агрегированную информацию аж из шести таблиц.</br> 

14.2. Показывает общий объем продаж по категориям товаров за 1997 год. Делает это вычисляя сумму ProductSales из представления Product Sales for 1997 и отображает как поле CategorySales, сортировка порисходит по полю CategoryName.</br>

14.3. Показывает общую стоимость заказа по заказчику и дату его отправки из таблиц Customers, Orders и представления Order Subtotals. При этом, сумма заказа всегда больше 2500$ и все отправки только за 1997 год.</br>

14.4. Выводит список товаров из таблицы Products с ценой выше средней среди всех товаров.</br>

14.3. Выводит данные из таблицы Orders и представления Order Subtotals при этом поле ShippedDate не должно быть пустым. По сути список топравленнных заказов с общими суммами. Наверное, должно еще быть ограничение по датам отправки, "квартал" или "год", судя из названия. Но в дизайне такого условия нет. Возможно представление не доработано.
