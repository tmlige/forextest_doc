OrderProfitPips_以点显示利润
=============================================


以点显示订单利润



**Delphi**

.. code:: delphi

	function OrderProfitPips: double;
	
**C++** >

.. code:: cpp

	double OrderProfitPips();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	if OrderProfitPips < 100 then ...






**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	{
	  if (OrderProfitPips() < 100) { ... }
	}



------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





