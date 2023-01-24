OrderSymbol_获取订单标的物
=============================================


返回交易标的



**Delphi**

.. code:: delphi

	function OrderSymbol: string;
	
**C++** >

.. code:: cpp

	PChar OrderSymbol();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(0, SELECT_BY_POS, MODE_TRADES) then
	if OrderSymbol <> 'USDJPY' then ...





**C++**

.. code:: cpp

	if (OrderSelect(0, SELECT_BY_POS, MODE_TRADES) == true)
	{
      if (strcmp(OrderSymbol(), "USDJPY") != 0) { ... }
	}



------------


*提示:首先通过OrderSelect 函数选择订单才能使用。*





