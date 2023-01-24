AccountLeverage_账户杠杆
=============================================


获取当前账户杠杆。 如果当前杠杆为 1:100，则该函数将返回 100。





**Delphi**

.. code:: delphi

	function AccountLeverage: integer;

	
	
**C++** 

.. code:: cpp

	double AccountLeverage();





------------


*代码示例*


**Delphi**

.. code:: delphi

	Print('Account leverage: ' + IntToStr(AccountLeverage));





**C++**

.. code:: cpp

	char buff[100];	 

	sprintf(buff, "Account leverage: %d', AccountLeverage());
	Print(buff);





