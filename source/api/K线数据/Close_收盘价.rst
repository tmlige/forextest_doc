Close_收盘价
=============================================


**Delphi**

.. code:: delphi

	function Close(
	  index: integer
	): double;



	
	
**C++** 

.. code:: cpp

	double Close(
	int index
	);



*参数说明*


- index

   Bar索引





------------


*代码示例*


**Delphi**

.. code:: delphi

	if Close(1) < Close(0) then …





**C++**

.. code:: cpp

	if (Close(1) < Close(0)) { … }
