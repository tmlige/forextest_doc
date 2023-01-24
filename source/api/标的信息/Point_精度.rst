Point_精度(最小变动值)
=============================================

返回最低变动的点数值(比如GBPUSD的0.0001)

 




**Delphi**

.. code:: delphi

	function Point: integer;
	
**C++** >

.. code:: cpp

	double Point();


------------


*代码示例*


**Delphi**

.. code:: delphi

	StopLoss := ask – 20*Point;





**C++**

.. code:: cpp

	StopLoss = Ask() – 20.0*Point();



------------




*在GetSingleTick 中返回买入价。*

*调用SetCurrencyAndTimeframe 后，则返回所选货币的买入价。*










