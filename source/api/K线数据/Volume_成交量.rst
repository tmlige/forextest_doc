Volume_成交量
=============================================



**Delphi**

.. code:: delphi

	function Volume(
	  index: integer
	): double;



	
	
**C++** 

.. code:: cpp

	double Volume(
	int index
	);



*参数说明*


- index

   Bar索引





------------


*代码示例*


**Delphi**

.. code:: delphi

	if Volume(1) < Volume(0) then …





**C++**

.. code:: cpp

	if (Volume(1) < Volume(0)) { … }
