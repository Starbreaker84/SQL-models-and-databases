**Решение на задачи занятия 9:**</br>
9.4.1.</br>
**SELECT** t1.CompanyName, t2.CompanyName, t1.Region</br>
**FROM** Customers t1, Customers t2</br>
**WHERE** t1.region *IS NULL* **AND** t2.Region *IS NULL* **AND** t1.CustomerID <> t2.CustomerID</br>
**ORDER BY** t1.CompanyName;</br>
9.4.2.</br>
**SELECT** * **FROM** Orders t1</br>
**WHERE** t1.CustomerID = *ANY*</br>
(**SELECT** t2.CustomerID **FROM** Customers t2 **WHERE** t2.Region *IS NOT NULL*);</br>
9.4.3.</br>
**SELECT** * **FROM** Orders t1</br>
**WHERE** t1.Freight > *ALL*</br>
(**SELECT** *MAX*(t2.UnitPrice) **FROM** Products t2);</br>
