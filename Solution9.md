**Решение на задачи занятия 9:**</br>
9.4.1.
**SELECT** t1.CompanyName, t2.CompanyName, t1.Region
**FROM** Customers t1, Customers t2
**WHERE** t1.region *IS NULL* **AND** t2.Region *IS NULL* **AND** t1.CustomerID <> t2.CustomerID
**ORDER BY** t1.CompanyName;
9.4.2.
**SELECT** * **FROM** Orders t1
**WHERE** t1.CustomerID = *ANY*
(**SELECT** t2.CustomerID **FROM** Customers t2 **WHERE** t2.Region *IS NOT NULL*);
9.4.3.
**SELECT** * **FROM** Orders t1
**WHERE** t1.Freight > *ALL*
(**SELECT** *MAX*(t2.UnitPrice) **FROM** Products t2);
