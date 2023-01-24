OrderOpenTime_获取订单创建日期
=============================================


返回订单开仓时间



**Delphi**

.. code:: delphi

	function OrderOpenTime: TDateTime;
	
	
	
**C++** >

.. code:: cpp

	TDateTime OrderOpenTime();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	if HourOf(OrderOpenTime) <> 12 then ...





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	{
	  if (HourOf(OrderOpenTime) <> 12) { ... }


------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





