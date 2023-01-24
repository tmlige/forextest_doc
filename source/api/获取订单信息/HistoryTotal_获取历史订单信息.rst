HistoryTotal_获取历史订单信息
=============================================


该函数为整数类型



**Delphi**

.. code:: delphi

	function HistoryTotal: integer;
	
	
	
**C++** >

.. code:: cpp

	int HistoryTotal();



------------


*代码示例*


**Delphi**

.. code:: delphi

	var
	i: integer;
	for i:=0 to HistoryTotal - 1 do
	begin
	  // returns number of records in Account History
	  if OrderSelect(i, SELECT_BY_POS, MODE_HISTORY) then
	  ...
	end;




**C++**

.. code:: cpp

	for (int i=0; i < HistoryTotal(); i++)
	{
	  // returns number of records in Account History
	  if (OrderSelect(i, SELECT_BY_POS, MODE_HISTORY) == true) { ... }
	}




