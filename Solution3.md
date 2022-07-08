**Рефлексия на задачу из занятия 2**</br>
В моём решении есть несколько лишних связей, а в остальном все позиции из эталонного решения совпали, только у меня связь таблиц многие-ко-многим немного подругому описана, но смысл тот же. Указал лишней таблицу *Contacts*, которая без связей. Также добавил две лишие связи по таблицам *Orders* и *Products*, из-за того, что ориентировался на названия полей в самой таблице.


**Решение на задачу занятия 3**</br>
3.9.1. **SELECT** ProductName, UnitsInStock **FROM** Products;</br>
3.9.2. **SELECT** ProductName, UnitPrice **FROM** Products **WHERE** UnitPrice < 20;</br>
3.9.3. **SELECT** * **FROM** Orders **WHERE** (Freight > 11.7) **AND** (Freight < 98.1);</br>
3.9.4. **SELECT** * **FROM** Employees **WHERE** (TitleOfCourtesy = 'Mr.') **OR** (TitleOfCourtesy = 'Dr.');</br>
3.9.5. **SELECT** * **FROM** Suppliers **WHERE** Country = 'Japan';</br>
3.9.6. **SELECT** * **FROM** Orders **WHERE** (EmployeeID = 2) **OR** (EmployeeID = 4) **OR** (EmployeeID = 8);</br>
3.9.7. **SELECT** OrderID, ProductID **FROM** \[Order Details\] **WHERE** (UnitPrice > 40) **AND** (Quantity < 10);</br>
