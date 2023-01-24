OrderCloseTime_获取订单关闭日期
=============================================


返回订单平仓时间



**Delphi**

.. code:: delphi

	function OrderCloseTime: TDateTime;
	
**C++** >

.. code:: cpp

	TDateTime OrderCloseTime();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	if HourOf(OrderCloseTime) < 10 then ...





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	{
	  if (HourOf(OrderCloseTime) < 10) { ... }


------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





