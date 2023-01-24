SetOptionDigits_设置参数位数
==============================


定义ot_Double(实数型类)的小数点位数,默认为两位.



**Delphi**

.. code:: delphi

	procedure SetOptionDigits(
	OptionName: string;
	digits: word
	);




**C++** >

.. code:: cpp

	void SetOptionDigits(
	PChar OptionName,
	Word digits
	);





*参数说明*


- OptionName

   参数名

- digits

	定义小数位数



------------

*代码示例*


**Delphi**

.. code:: delphi

	var
	Gamma: double; 

	RegOption('Gamma', ot_Double, Gamma);
	SetOptionDigits('Gamma', 4);


**C++**

.. code:: cpp

	double Gamma;	 

	RegOption("Gamma", ot_Double, &Gamma);
	SetOptionDigits("Gamma", 4);

