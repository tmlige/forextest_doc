SetIndicatorBuffStyle_指标样式
=============================================


为使用CreateIndicator 创建的指标设置样式（线条样式、粗细、颜色）。



**Delphi**

.. code:: delphi

	procedure SetIndicatorBuffStyle(
	IndicatorHandle: integer;
	BuffIndex: integer; 
	_style: TPenStyle;
	width: integer; 
	color: TColor
	);



	
	
**C++** 

.. code:: cpp

	void SetIndicatorBuffStyle(
	int IndicatorHandle,
	int BuffIndex,
	TPenStyle _style,
	int width,
	TColor color
	);





*参数说明*


- IndicatorHandle

   指标句柄

- BufferIndex

   索引
   
- _style

   样式
   
- width

   宽度  
   
- color

   颜色
   





------------


*代码示例*


**Delphi**

.. code:: delphi

	var
	IndMACD: integer; 

	SetIndicatorBuffStyle(IndMACD, 0, psSolid, 1, clYellow);
	SetIndicatorBuffStyle(IndMACD, 1, psDot, 1, clBlue);



**C++**

.. code:: cpp

	int IndMACD;	 

	SetIndicatorBuffStyle(IndMACD, 0, psSolid, 1, clYellow);
	SetIndicatorBuffStyle(IndMACD, 1, psDot, 1, clBlue);


 
