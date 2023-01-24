Ask_卖价
=============================================


获取当前标的卖入价


**Delphi**

.. code:: delphi

	function Ask: double;
	
**C++** >

.. code:: cpp

	double Ask();


------------


*代码示例*


**Delphi**

.. code:: delphi

	StopLoss := Ask - 30*Point;




**C++**

.. code:: cpp

	StopLoss = Ask() - 30.0*Point();


------------


*在GetSingleTick 中返回买入价。*

*调用SetCurrencyAndTimeframe 后，则返回所选货币的买入价。*





