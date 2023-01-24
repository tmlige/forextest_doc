MarketInfo_市场信息
=============================================


查询市场信息



**Delphi**

.. code:: delphi

	function MarketInfo(
	Symbol: string;
	_type: TMarketInfo
	): double;

	 



	
**C++** >

.. code:: cpp

	double MarketInfo(PChar Symbol,
	TMarketInfo _type
	);
	
	

*参数说明*


- Symbol

   标的名


- _type

   请求信息的类型（MODE_ASK、MODE_BID）




------------


*代码示例*


**Delphi**

.. code:: delphi

	if MarketInfo('USDJPY', MODE_BID) < 102.18 then ...





**C++**

.. code:: cpp

	if (MarketInfo("USDJPY", MODE_BID) < 102.18) { ... }







