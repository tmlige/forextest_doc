AccountMargin_账户保证金
=============================================


获取以美元为单位的活期账户可用保证金。





**Delphi**

.. code:: delphi

	function AccountMargin: double;

	
	
**C++** 

.. code:: cpp

	double AccountMargin();





------------


*代码示例*


**Delphi**

.. code:: delphi

	Print(format('Account margin: %.2f', [AccountMargin]);





**C++**

.. code:: cpp

	char buff[100];	 

	sprintf(buff, "Account margin: %.2f", AccountMargin());
	Print(buff);





