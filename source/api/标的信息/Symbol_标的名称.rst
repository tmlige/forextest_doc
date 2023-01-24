Symbol_标的名称
=============================================

返回标的名



**Delphi**

.. code:: delphi

	function Symbol: string;
	
**C++** >

.. code:: cpp

	PChar Symbol();


------------


*代码示例*


**Delphi**

.. code:: delphi

	if Symbol = 'USDJPY' then …





**C++**

.. code:: cpp

	if (strcmp(Symbol(), "USDJPY") == 0) { ... }


------------



*在GetSingleTick 中返回买入价。*

*调用SetCurrencyAndTimeframe 后，则返回所选货币的买入价。*





