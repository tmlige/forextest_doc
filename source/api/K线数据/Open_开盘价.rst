Open_开盘价
=============================================


按索引返回开盘价 (最后一根为0,前一根为1)





**Delphi**

.. code:: delphi

	function Open(
	  index: integer
	): double;



	
	
**C++** 

.. code:: cpp

	double Open(
	int index
	);



*参数说明*


- index

   Bar索引





------------


*代码示例*


**Delphi**

.. code:: delphi

	if Open(1) < Open(0) then …





**C++**

.. code:: cpp

	if (Open(1) < Open(0)) { … }




