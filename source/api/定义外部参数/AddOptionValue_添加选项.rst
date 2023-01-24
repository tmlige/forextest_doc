AddOptionValue_添加选项
==============================

定义外部参数的值范围（对于 ot_Longword、ot_Integer、ot_Double 类型）。

在参数对话框中输入数据后，将检查输入：LowValue <= x <= HighValue。


**Delphi**

.. code:: delphi

	procedure SetOptionRange(OptionName: string;LowValue: double;HighValue: double);




**C++** >

.. code:: cpp

	void RegOption(PChar OptionName,TOptionType OptionType,void\*option);



*参数说明*


-  OptionName:参数名称将显示在对话框中，也用于定义参数的其他选项。

-  LowValue:最小值

-  HighValue:最大值

------------

*代码示例*


**Delphi**

.. code:: delphi

	var
	Period: integer;	 

	RegOption('Period', ot_Integer, Period);
	SetOptionRange('Period', 2, 16);


**C++**

.. code:: cpp

	int Period;	 

	RegOption("Period", ot_Integer, &Period);
	SetOptionRange("Period", 2, 16);
