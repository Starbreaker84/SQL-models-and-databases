**Рефлексия на задачи из занятия 14:**</br>
В задании 14.1. забыл упомянуть что на выходе получается инвойс/счёт.

**Решение на задачи занятия 15:**</br>
15.1.</br>
Создаём таблицу Territories:</br>
**CREATE TABLE** Territories (TerritoryID nchar(16) *NOT NULL*, TerritoryDescription nchar(50) *NOT NULL*, RegionID int *NOT NULL*);</br>
Задаём Primary Key в таблице Territories:</br>
**ALTER TABLE** Territories **ADD PRIMARY KEY** (TerritoryID);</br>
Задаём Primary Key в таблице Region:</br>
**ALTER TABLE** Region **ADD PRIMARY KEY** (RegionID);</br>
Добавляем поля в таблицу Region:</br>
**INSERT INTO** Region (RegionID, RegionDescription)</br>
**VALUES** (1, 'Eastern');</br>
**INSERT INTO** Region (RegionID, RegionDescription)</br>
**VALUES** (2, 'Western');</br>
**INSERT INTO** Region (RegionID, RegionDescription)</br>
**VALUES** (3, 'Northern');</br>
**INSERT INTO** Region (RegionID, RegionDescription)</br>
**VALUES** (4, 'Southern');</br>
Задаём FOREIGN KEY в таблице Territories:</br>
**ALTER TABLE** Territories **ADD FOREIGN KEY** (RegionID) **REFERENCES** Region (RegionID);</br>
Добавляем поля в таблицу Territories:</br>
**INSERT INTO** Territories (TerritoryID, TerritoryDescription, RegionID)</br>
**VALUES** (01581, 'Westboro', 1);</br>
**INSERT INTO** Territories (TerritoryID, TerritoryDescription, RegionID)</br>
**VALUES** (60601, 'Chicago', 2);</br>
**INSERT INTO** Territories (TerritoryID, TerritoryDescription, RegionID)</br>
**VALUES** (03049, 'Holis', 3);</br>
**INSERT INTO** Territories (TerritoryID, TerritoryDescription, RegionID)</br>
**VALUES** (31406, 'Columbia', 4);</br>
Попытка добавить запись с RegionID, которого нет в таблице Region выдаст ошибку:</br>
**INSERT INTO** Territories (TerritoryID, TerritoryDescription, RegionID)</br>
**VALUES** (51602, 'Hoffman', 5);</br>
Ошибка: The INSERT statement conflicted with the FOREIGN KEY constraint "FK_TerritoriRegio_15502E78".</br>
