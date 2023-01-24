iBars_K线数据
=============================================


获取总K线数量





**Delphi**

.. code:: delphi

	function iBars(
	Symbol: string;
	TimeFrame: integer
	): integer;

	 


	
	
**C++** 

.. code:: cpp

	int iBars(
	PChar Symbol,
	int TimeFrame
	);


*参数说明*


- Symbol

   标的名


- TimeFrame

   时间框架





------------


*代码示例*


**Delphi**

.. code:: delphi

	for i:=0 to iBars('GBPUSD', 60) – 1 do
	begin
	  …
	end;





**C++**

.. code:: cpp

	for (int i=0; i < iBars("GBPUSD", 60); i++)
	{
	…
	}





