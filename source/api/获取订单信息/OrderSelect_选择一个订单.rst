OrderSelect 订单选择
=============================================


订单选择,执行此函数后以下功能才可用:
OrderProfit, OrderProfitPips, OrderOpenTime, OrderCloseTime, OrderLots, OrderTicket, OrderType, OrderStopLoss, OrderTakeProfit, OrderOpenPrice, OrderClosePrice, OrderSymbol. 

如果订单被选中，该函数返回“ture”，否则返回“false”。



**Delphi**

.. code:: delphi

	function OrderSelect(
	index: integer;
	flags: TOrderSelectMode = SELECT_BY_POS;
	pool: TSearchMode = MODE_TRADES
	): boolean;
	
	
**C++** >

.. code:: cpp

	bool OrderSelect(
	int index,
	TOrderSelectMode flags = SELECT_BY_POS,
	TSearchMode pool = MODE_TRADES
	);

*参数说明*


- index

   订单的索引

- flags

	选择订单的方式 SELECT_BY_POS, SELECT_BY_TICKET
	
- pool

	选择订单的模式 如 MODE_HISTORY 
	


------------


*代码示例*


**Delphi**

.. code:: delphi

	if OrderSelect(10, SELECT_BY_POS, MODE_TRADES) then ...




**C++**

.. code:: cpp

	if (OrderSelect(10, SELECT_BY_POS, MODE_TRADES) == true) { ... }





