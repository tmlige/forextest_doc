Time_时间
=============================================

按索引返回时间 (最后一根为0,前一根为1)


**Delphi**

.. code:: delphi

	function Time(
	  index: integer
	): TDateTime;



	
	
**C++** 

.. code:: cpp

	double Time(
	int index
	);



*参数说明*


- index

   Bar索引





------------


*代码示例*


**Delphi**

.. code:: delphi

	if Hour(Time(0)) <> 22 then …





**C++**

.. code:: cpp

	if (HourOf(Time(0)) != 22) { … }
