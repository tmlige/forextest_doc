iBarShift_索引
=============================================


获取一个bar的索引





**Delphi**

.. code:: delphi

	function iBarShift(
	Symbol: string; 
	TimeFrame: integer; 
	time: TDateTime; 
	Exact: boolean
	): integer;



	
	
**C++** 

.. code:: cpp

	int iBarShift(
	PChar Symbol, 
	int TimeFrame, 
	TDateTime time, 
	bool Exact
	);



*参数说明*


- Symbol

   标的名


- TimeFrame

   时间框架

- time

   K线的时间

- Exact

   如何查看时间。如果Exact = true，则BAR的时间= time，如果Exact = false，则BAR的时间<= time < 下一个BAR的时间。





------------


*代码示例*


**Delphi**

.. code:: delphi

	
	index := iBarShift('GBPUSD', 60, time, false);




**C++**

.. code:: cpp

	int index = iBarShift('GBPUSD', 60, time, false);




