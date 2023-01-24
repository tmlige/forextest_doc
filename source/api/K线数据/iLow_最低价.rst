iLow_最低价
=============================================


说明





**Delphi**

.. code:: delphi

	function iLow(
	Symbol: string;
	TimeFrame: integer;
	index: integer
	): double;


	
	
**C++** 

.. code:: cpp

	double iLow(
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

	o := iLow('USDJPY', 15, 10);





**C++**

.. code:: cpp

	double o = iLow("USDJPY", 15, 10);




