OrderTakeProfit_获取止赢价
=============================================


返回订单止赢信息



**Delphi**

.. code:: delphi

	function OrderTakeProfit: double;

 

	
**C++** >

.. code:: cpp

	double OrderTakeProfit();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	tp := OrderTakeProfit;





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	tp = OrderTakeProfit();

------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





