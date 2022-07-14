**Рефлексия на задачи из занятия 12:**</br>
В задании 12.3.3. не упоминул о том, что конечно, недобавление информации о заказе (значения NULL) в полях, или добавление некорретой информации в поля, может и не приведёт к ошибкам, но в целом, может нарушить логическую структуру.

**Решение на задачи занятия 13:**</br>
13.3.1.</br>
**UPDATE** \[Order Details\]</br>
**SET** Discount = 0.2</br>
**WHERE** Quantity > 50;</br>

13.3.2.</br>
**UPDATE** Contacts</br>
**SET** City = 'Piter', Country = 'Russia'</br>
**WHERE** City = 'Berlin' **AND** Country = 'Germany';</br>

13.3.3.</br>
**INSERT INTO** Shippers (CompanyName, Phone)</br>
**VALUES** ('FedEX', '(555) 555-5555');</br>
</br>
**INSERT INTO** Shippers (CompanyName, Phone)</br>
**VALUES** ('SuperPost', '(555) 577-5775');</br>
</br>
**DELETE FROM** Shippers</br>
**WHERE** ShipperID BETWEEN 4 AND 5;</br>
</br>
Удалял по PK-ключу, при этом предварительно убедившись, что данные значения ключей больше нигде не фигурируют.
