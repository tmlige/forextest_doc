CreateIndicator_创建指标
=============================================


说明





**Delphi**

.. code:: delphi

	function CreateIndicator(
	Symbol: string;
	TimeFrame: integer;
	IndicatorName: string;
	Parameters: string
	): integer;



	
	
**C++** 

.. code:: cpp

	int CreateIndicator(
	PChar Symbol,
	int TimeFrame,
	PChar IndicatorName,
	PChar parameters
	);



*参数说明*


- Symbol

   要应用指标的标的

- TimeFrame

   时间框架

- IndicatorName

   指标名称
   
- Parameters

   指标参数字符串





------------


*代码示例*


**Delphi**

.. code:: delphi

	var
	IndMACD: integer;
	IndMA: integer;

	{-----Reset strategy---------------------------------------------------------}
	procedure ResetStrategy; stdcall;
	begin
	IndMACD := CreateIndicator('EURUSD', 15, 'MACD', '8;20;12;Close');
	IndMA := CreateIndicator('USDJPY', 60, 'MovingAverage',
	  format('%d;0;0;%s;Close', [MATrendPeriod, StrMAType(ma_EMA)]));
	end;






**C++**

.. code:: cpp

	int IndMACD;
	int IndMA;	 

	{-----Reset strategy---------------------------------------------------------}
	EXPORT void __stdcall  ResetStrategy()
	{
	IndMACD = CreateIndicator("EURUSD", 15, "MACD", "8;20;12;Close"); 

	char buff[1000];
	sprintf(buff, "%d;0;0;%s;Close", MATrendPeriod, StrMAType(ma_EMA));
	IndMA = CreateIndicator("USDJPY", 60, "MovingAverage", buff);
	}

*这个函数应该仅在ResetStrategy重启时被调用!!!*

*获取指标句柄后应该将其存储在全局变量中,与GetIndicatorValue函数一起使用来获取指标的值.* 

*此功能将指标置于选定货币时间范围的图表上。如果该指标已存在，则无需创建新指标即可使用。该策略将在执行期间锁定该指标，因此您将无法手动将其从图表中删除。但是断开连接后它会被解锁。*

