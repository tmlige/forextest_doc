OrderType_获取订单类型
=============================================


返回所选订单的类型



**Delphi**

.. code:: delphi

	function OrderType: TTradePositionType;
	
**C++** >

.. code:: cpp

	TTradePositionType OrderType();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	if (OrderType <> tp_Sell) and (OrderType <> tp_Buy) then ...





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	{
	  if ((OrderType() != tp_Sell) && (OrderType() != tp_Buy)) { ... }


------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





