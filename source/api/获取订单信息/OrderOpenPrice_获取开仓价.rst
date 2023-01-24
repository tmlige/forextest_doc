OrderOpenPrice_获取开仓价
=============================================


返回订单开仓价



**Delphi**

.. code:: delphi

	function OrderOpenPrice: double;
	
**C++** >

.. code:: cpp

	double OrderOpenPrice();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	price := OrderOpenPrice;





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	price = OrderOpenPrice();


------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





