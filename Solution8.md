**Рефлексия на задачи из занятия 7:**</br>
В задании 7.3.1. я полагал что в поле Discount изначально стоят центы, поэтому вычислял процент по другому, плюс покопался в документации чтобы понять, как можно округлять значения. Ну и решил что только одно поле нужно вывести.

**Решение на задачи занятия 8:**</br>
8.3.1. </br>
**SELECT** Products.ProductName, Categories.CategoryName</br>
**FROM** Products, Categories</br>
**WHERE** Products.CategoryID = Categories.CategoryID;</br>
8.3.2. </br>
**SELECT** Products.ProductName, \[Order Details\].UnitPrice</br>
**FROM** Products, \[Order Details\]</br>
**WHERE** Products.ProductID = \[Order Details\].ProductID **AND** \[Order Details\].UnitPrice < 20;</br>
8.3.3. </br>
**SELECT** Products.ProductName, Categories.CategoryName, \[Order Details\].UnitPrice</br>
**FROM** Products, Categories, \[Order Details\]</br>
**WHERE** Products.ProductID = \[Order Details\].ProductID **AND** Products.CategoryID = Categories.CategoryID **AND** \[Order Details\].UnitPrice < 20;
