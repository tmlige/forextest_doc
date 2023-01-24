OrderMagicNumber_获取订单MagicNumber
=============================================

返回订单自定义的"魔法号"



**Delphi**

.. code:: delphi

	function OrderMagicNumber: integer;
	
**C++** >

.. code:: cpp

	int OrderMagicNumber();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	if OrderMagicNumber = 777 then ...





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	{
	  if (OrderMagicNumber() == 777) { ... }
	  }


------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





