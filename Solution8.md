**Рефлексия на задачи из занятия 7:**</br>
В задании 7.3.1. я полагал что в поле Discount изначально стоят центы, поэтому вычислял процент подругому, плюс покопался в документации чтобы понять, как можно округлять значения. Ну, подумал что только одно поле нужно вывести.

**Решение на задачи занятия 8:**</br>
8.3.1. **SELECT** Products.ProductName, Categories.CategoryName
       **FROM** Products, Categories
       **WHERE** Products.CategoryID = Categories.CategoryID;</br>
8.3.2. **SELECT** Products.ProductName, \[Order Details\].UnitPrice
       **FROM** Products, \[Order Details\]
       **WHERE** Products.ProductID = \[Order Details\].ProductID **AND** \[Order Details\].UnitPrice < 20;</br>
8.3.3. **SELECT** Products.ProductName, Categories.CategoryName, \[Order Details\].UnitPrice
       **FROM** Products, Categories, \[Order Details\]
       **WHERE** Products.ProductID = \[Order Details\].ProductID **AND** Products.CategoryID = Categories.CategoryID **AND** \[Order Details\].UnitPrice < 20;
