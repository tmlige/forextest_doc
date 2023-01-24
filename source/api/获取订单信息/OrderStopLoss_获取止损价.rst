OrderStopLoss_获取止损价
=============================================


返回订单止损信息



**Delphi**

.. code:: delphi

	function OrderProfit: double;
	
**C++** >

.. code:: cpp

	double OrderProfit();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	sl := OrderStopLoss;








**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	sl = OrderStopLoss();

------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





