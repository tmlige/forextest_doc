OrderProfit_以美元显示利润
=============================================


以美元形式返回订单利润



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
	if OrderProfit < 100 then ...





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	{
	  if (OrderProfit() < 100) { ... }


------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





