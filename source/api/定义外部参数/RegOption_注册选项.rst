RegOption_注册选项
==============================

注册一个外部参数,该参数将通过forextester策略设置具体参数。


**Delphi**

.. code:: delphi

	RegOption(OptionName: string;	OptionType:TOptionType;	var option);



**C++** >

.. code:: cpp

	void RegOption(PChar OptionName,TOptionType OptionType,void\*option);



*参数说明*


-  OptionName:参数名称将显示在对话框中，也用于定义参数的其他选项。

-  OptionType:参数类型

-  Option:选项,存放参数的变量，变量的类型要与参数声明的类型-OptionType相对应

------------

*代码示例*


**Delphi**

.. code:: delphi

   var
   SMAPeriod: integer;
   SomeText: PChar = nil;
   
   RegOption('SMA period', ot_Integer, SMAPeriod);
   RegOption('Description', ot_String, SomeText);

**C++**

.. code:: cpp

   int  SMAPeriod;
   PChar SomeText = NULL;

   RegOption("SMA period", ot_Integer, &SMAPeriod);
   RegOption("Description", ot_String, &SomeText);