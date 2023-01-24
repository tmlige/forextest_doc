OrderComment_获取订单注释
=============================================

返回订单注释



**Delphi**

.. code:: delphi

	function OrderComment: string;
	
**C++** >

.. code:: cpp

	PChar OrderComment();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	if OrderComment = '123' then ...





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	{
	  if (strcmp(OrderComment(), "123") == 0) { ... }
	  }


------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





