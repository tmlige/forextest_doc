OrderClosed_检查订单是否关闭
=============================================


检查订单是否已关闭/删除或尚未开仓。

如果订单被关闭/删除/未开仓，则函数返回“true”，否则返回“false”。



**Delphi**

.. code:: delphi

	function OrderClosed(
	OrderHandle: integer
	): boolean;
	
	
	
**C++** >

.. code:: cpp

	bool OrderClosed(int OrderHandle);



*参数说明*


- Symbol

   标的名



------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderClosed(OrderHandle) then ...




**C++**

.. code:: cpp

	if (OrderClosed(OrderHandle) == true) { ... }





