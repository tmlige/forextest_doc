GetIndicatorValue_指标值
=============================================


获取指标的值




**Delphi**

.. code:: delphi

	function GetIndicatorValue(
	IndicatorHandle: integer;
	index: integer;
	BufferIndex: integer
	): double;


	
	
**C++** 

.. code:: cpp

	double GetIndicatorValue(
	int IndicatorHandle,
	int index,
	int BufferIndex
	);




*参数说明*


- Symbol

   要应用指标的标的

- index

   索引
   
- BufferIndex

   指标内部的索引
   





------------


*代码示例*


**Delphi**

.. code:: delphi

	var
	IndMACD: integer;
	MacdCurrent: double;
	MacdPrevious: double;

	MacdCurrent := GetIndicatorValue(IndMACD, 0, 2);
	MacdPrevious := GetIndicatorValue(IndMACD, 1, 2);






**C++**

.. code:: cpp

	int IndMACD, MacdCurrent, MacdPrevious; 

	MacdCurrent = GetIndicatorValue(IndMACD, 0, 2);
	MacdPrevious = GetIndicatorValue(IndMACD, 1, 2);

 
