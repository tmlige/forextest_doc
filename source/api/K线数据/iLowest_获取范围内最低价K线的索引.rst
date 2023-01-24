iLowest_获取范围内最低价K线的索引
=============================================


在范围内(索引index和数量count)和商品(symbox)及时间框架中(TimeFrame)定位最低价K线的索引值.

如果找到K线，则函数返回其索引值，否则函数返回 -1。








**Delphi**

.. code:: delphi

	function iLowest(
	Symbol: string; 
	TimeFrame: integer; 
	_type: integer;
	count: integer; 
	index: integer
	): integer;


	
	
**C++** 

.. code:: cpp

	int iLowest(
	PChar Symbol, 
	int TimeFrame, 
	int _type, 
	int count, 
	int index
	);



*参数说明*


- Symbol

   标的名


- TimeFrame

   时间框架

- count

   数量

- index

   索引





------------


*代码示例*


**Delphi**

.. code:: delphi


	//查找GBPUSD收盘最低价的索引(100, 101, 102 .. 149)
	index := iLowest('GBPUSD', 15, MODE_CLOSE, 50, 100);





**C++**

.. code:: cpp	

	int index = iLowest("GBPUSD", 15, MODE_CLOSE, 50, 100);






