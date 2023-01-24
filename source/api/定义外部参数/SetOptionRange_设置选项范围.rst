SetOptionRange_设置选项范围
==============================


定义外部参数的值范围（对于 ot_Longword、ot_Integer、ot_Double 类型）。

在参数对话框中输入数据后，将检查输入：LowValue <= x <= HighValue。



**Delphi**

.. code:: delphi

	procedure SetOptionRange(
	OptionName: string;
	LowValue: double;
	HighValue: double
	);




**C++** >

.. code:: cpp

	void SetOptionRange(
	PChar OptionName,
	double LowValue,
	double HighValue
	);




*参数说明*


- OptionName

   选项名称.

- LowValue

	范围最小值.

- HighValue

	范围最大值.


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
