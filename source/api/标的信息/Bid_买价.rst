Bid_买价
=============================================


获取当前标的买入价


**Delphi**

.. code:: delphi

	function Bid: double;
	
**C++** >

.. code:: cpp

	double Bid();


------------


*代码示例*


**Delphi**

.. code:: delphi

	StopLoss := Bid + 30*Point;




**C++**

.. code:: cpp

	StopLoss = Bid() + 30.0*Point();


------------


*在GetSingleTick 中返回买入价。*

*调用SetCurrencyAndTimeframe 后，则返回所选货币的买入价。*





