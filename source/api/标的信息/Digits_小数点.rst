Digits_小数位
=============================================


返回小数位

 




**Delphi**

.. code:: delphi

	function Digits: integer;
	
**C++** >

.. code:: cpp

	int Digits();


------------


*代码示例*


**Delphi**

.. code:: delphi

	Print('number of digits after point ' + IntToStr(Digits));





**C++**

.. code:: cpp

	sprintf(buff, "number of digits after point %d", Digits);
	Print(buff);



------------




*在GetSingleTick 中返回买入价。*

*调用SetCurrencyAndTimeframe 后，则返回所选货币的买入价。*




