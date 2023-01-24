OrdersTotal_获取活动订单的数量
=============================================


返回未平仓和未完成订单的数量。



**Delphi**

.. code:: delphi

	function OrdersTotal: integer;new_file
	
	
	
**C++** >

.. code:: cpp

	int OrdersTotal();



------------


*代码示例*


**Delphi**

.. code:: delphi

	var
	i: integer;
	for i:=0 to OrdersTotal - 1 do
	begin
	   if OrderSelect(i, SELECT_BY_POS, MODE_HISTORY) then
	  ...
	end;




**C++**

.. code:: cpp

	for (int i=0; i < OrdersTotal(); i++)
	{
	    if (OrderSelect(i, SELECT_BY_POS, MODE_HISTORY) == true) { ... }
	}




