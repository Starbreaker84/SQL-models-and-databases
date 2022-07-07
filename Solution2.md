**Рефлексия на задачу из занятия 1**</br>
В целом все совпало с эталонным решением. Не обратил внимания что таблица *Territories* это не просто территории, а территориальные единицы регионов, а также что в таблице *EmployeeTerritories* не место расположения сотрудника, а все-таки его "зона ответственности".

**Решение на задачу занятия 2**</br>
Взаимосвязи между таблицами northwind и их описание (один-к-одному, один-ко-многим и многие-ко-многим):</br>
*Categories* один-ко-многим c *Products*</br>
*Contacts* - нет связей</br>
*Customers* один-ко-многим c *Orders*</br>
*Employees* один-ко-многим c *EmployeeTerritories* и *Orders*</br>
*EmployeeTerritories* многие-ко-многим с *Employees* и *Territories*</br>
*Order Details* многие-ко-многим с *Orders* и *Products*</br>
*Orders* один-ко-многим с *Order Details, Customers, Employees* и *Shippers*</br>
*Products* один-ко-многим c *Order Details, Suppliers* и *Categories*</br>
*Region* один-ко-многим c *Territories*</br>
*Shippers* один-ко-многим *Orders*</br>
*Suppliers* один-ко-многим *Products*</br>
*Territories* один-ко-многим *EmployeeTerritories*</br>
