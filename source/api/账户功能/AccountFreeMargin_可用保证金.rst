AccountFreeMargin_可用保证金
=============================================


获取以美元为单位的活期账户可用保证金。





**Delphi**

.. code:: delphi

	function AccountFreeMargin: double;

	
	
**C++** 

.. code:: cpp

	double AccountFreeMargin();





------------


*代码示例*


**Delphi**

.. code:: delphi

	var
	LotSize: double;	 

	LotSize := RoundTo(AccountFreeMargin/10, -1);
	if LotSize < 0.1 then
	LotSize := 0.1;






**C++**

.. code:: cpp

	double LotSize; 

	LotSize = RoundTo(AccountFreeMargin()/10, -1);
	if (LotSize < 0.1) LotSize = 0.1;







