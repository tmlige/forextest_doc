OrderClosePrice_获取平仓价
=============================================


返回订单平仓价



**Delphi**

.. code:: delphi

	function OrderClosePrice: double;
	
**C++** >

.. code:: cpp

	double OrderClosePrice();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	price := OrderClosePrice;





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	price = OrderClosePrice();


------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





