GetOrderInfo_获取订单信息
=============================================


以TTradePosition记录的形式获取有关未平仓或待处理订单的信息

如果找到订单，则函数返回"true"，“并且"info”中填充订单信息，否则返回"false"



**Delphi**

.. code:: delphi

	function GetOrderInfo(
	OrderHandle: integer;
	var info: TTradePosition
	): boolean;
	
	
	
**C++** >

.. code:: cpp

	bool GetOrderInfo(
	int OrderHandle,
	TTradePosition& info
	);	


*参数说明*


- Symbol

   标的名

- info

	填充信息
	


------------


*代码示例*


**Delphi**

.. code:: delphi

	var
	info: TTradePosition;	 

	if GetOrderInfo(OrderHandle, info) then ...




**C++**

.. code:: cpp

	TTradePosition info;

	(GetOrderInfo(OrderHandle, info) == true) { ... }




