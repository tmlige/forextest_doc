AccountBalance_账户余额 
=============================================


说明





**Delphi**

.. code:: delphi

	function AccountBalance: double;

	
	
**C++** 

.. code:: cpp

	double AccountBalance();





------------


*代码示例*


**Delphi**

.. code:: delphi

	Print(format('Account profit: %.2f', [AccountProfit]));





**C++**

.. code:: cpp

	char buff[100];	 

	sprintf(buff, "Account profit: %.2f", AccountProfit());
	Print(buff);





