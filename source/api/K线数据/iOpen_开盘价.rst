iOpen_开盘价
=============================================

说明:

获取K线的“开盘”值，其中"Symbol "为标的名称

TimeFrame为选定的时间范围

"index" – 从0开始索引



**Delphi**

.. code:: delphi

	function iOpen(
	Symbol: string;
	TimeFrame: integer;
	index: integer
	): double;


	
	
**C++** 

.. code:: cpp

	double iOpen(
	PChar Symbol,
	int TimeFrame,
	int index
	);


*参数说明*


- Symbol

   标的名


- TimeFrame

   时间框架

- index

   索引





------------


*代码示例*


**Delphi**

.. code:: delphi

	var
	o: double;	 

	o := iOpen('USDJPY', 15, 10);





**C++**

.. code:: cpp

	double o = iOpen("USDJPY", 15, 10);




