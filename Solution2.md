**Рефлексия на задачу из занятия 1**
В целом все совпало с эталонным решением. Не обратил внимания что таблица Territories это не просто территории, а территориальные единицы регионов, а также что в таблице EmployeeTerritories не место расположения сотрудника, а все-таки его "зона ответственности".

**Решение га задачу занятия 2**
Взаимосвязи между таблицами northwind и их описание (один-к-одному, один-ко-многим и многие-ко-многим):
Categories один-ко-многим c Products
Contacts - нет связей
Customers один-ко-многим c Orders
Employees один-ко-многим c EmployeeTerritories и Orders
EmployeeTerritories многие-ко-многим с Employees и Territories
Order Details многие-ко-многим с Orders и Products
Orders один-ко-многим с Order Details, Customers, Employees и Shippers
Products один-ко-многим c Order Details, Suppliers и Categories
Region один-ко-многим c Territories
Shippers один-ко-многим Orders
Suppliers один-ко-многим Products
Territories один-ко-многим EmployeeTerritories
