AccountProfit_账户利润
=============================================


当前总利润,这是当前余额和初始入金间存款之间的差额。





**Delphi**

.. code:: delphi

	function AccountProfit: double;

	
	
**C++** 

.. code:: cpp

	double AccountProfit();





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





