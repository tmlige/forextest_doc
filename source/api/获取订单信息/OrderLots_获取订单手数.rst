OrderLots_获取订单手数
=============================================


返回订单手数



**Delphi**

.. code:: delphi

	function OrderLots: double;
	
**C++** >

.. code:: cpp

	double OrderLots();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	if OrderLots < 0.5 then ...





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	{
	  if (OrderLots() < 0.5) { ... }


------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





