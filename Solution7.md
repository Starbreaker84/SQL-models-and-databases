**Рефлексия на задачи из занятия 6:**</br>
В задании 6.3.1. допустил ошибку и не добавил поле с количеством типа контакта, от этого моя выборка не имеет особого смысла. Еще раз повторяю тему агрегации таблиц.

**Решение на задачи занятия 7:**</br>
7.3.1. **SELECT ROUND**(Discount * 100 / UnitPrice, 2) **FROM** \[Order Details\];</br>
7.3.2. **SELECT** * **FROM** \[Order Details\] **WHERE** ProductID **IN** (**SELECT** ProductID **FROM** Products **WHERE** UnitsInStock > 40);</br>
7.3.3. **SELECT** * **FROM** \[Order Details\] **WHERE** ProductID **IN** (**SELECT** ProductID **FROM** Products **WHERE** UnitsInStock > 40) **AND** OrderID **IN** (**SELECT** OrderID **FROM** Orders **WHERE** Freight >= 50);
