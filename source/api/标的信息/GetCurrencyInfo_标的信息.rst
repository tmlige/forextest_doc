GetCurrencyInfo_标的信息
=============================================


在TCurrencyInfo列表中获取标的信息,如果标的在列表中,则将信息返回到info中,同时返回值为true

否则返回false




**Delphi**

.. code:: delphi

	function GetSymbolInfo(
	Symbol: string;
	var info: PCurrencyInfo
	): boolean;

	
**C++** >

.. code:: cpp

	bool GetSymbolInfo(
	PChar Symbol,
	PCurrencyInfo& info
	);
	

*参数说明*


- Symbol

   标的名


- info

   返回的变量名





------------


*代码示例*


**Delphi**

.. code:: delphi

	var
	info: PCurrencyInfo;	 

	if GetCurrencyInfo('USDJPY', info) then
	begin
	  Print(format('%s %d %d %.4f', [info.Symbol, info.Digits, info.Spread, info.Point]));
	end;






**C++**

.. code:: cpp

	PCurrencyInfo info;
	char buff[1000]; 

	if (GetCurrencyInfo("USDJPY", info) == true)
	{
	  sprintf(buff, "%s %d %d %.4f", info.Symbol, info.Digits, info.Spread, info.Point);
	  Print(buff);
	}




