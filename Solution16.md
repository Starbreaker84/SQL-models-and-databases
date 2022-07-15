**Решение на задачи занятия 16:**</br>
Добавляем некластеризованный индекс (поскольку PK-ключ уже создал кластеризованное поле) в таблице Territories:</br>
**CREATE INDEX** idxTerritoryDescription **ON** Territories (TerritoryDescription);</br>
Аналогично создаём индекс для таблицы Region:</br>
**CREATE INDEX** idxRegionDescription **ON** Region (RegionDescription);
