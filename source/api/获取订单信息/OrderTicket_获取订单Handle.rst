OrderTicket_获取订单Handle
=============================================

返回订单的标识符(ticket)



**Delphi**

.. code:: delphi

	function OrderTicket: integer;

 

	
**C++** >

.. code:: cpp

	int OrderTicket();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	if OrderTicket <> SavedHandle then ...





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	{
	  if (OrderTicket() != SavedHandle) { ... }


------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





