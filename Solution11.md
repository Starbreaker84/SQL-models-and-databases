**Решение на задачи занятия 11:**</br>
11.5.1.</br>
**SELECT** Customers.CompanyName, Orders.OrderID **FROM** Customers</br>
**LEFT JOIN** Orders</br>
**ON** Customers.CustomerID = Orders.CustomerID;</br>

11.5.2.</br>
**SELECT** 'Customer' *As Type*, ContactName, City, Country **FROM** Customers</br>
**UNION**</br>
**SELECT** 'Supplier' *As Type*, ContactName, City, Country **FROM** Suppliers;
