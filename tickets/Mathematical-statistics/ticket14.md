# Точечные и интервальные оценки. Доверительные интервалы.

Оценки, которые задаются одним числом называтся точечными. Если объем выборки n большой, то оценки дают достаточно хорошие результаты. 


Если n маленькое, то надежность этих оценок ![](https://latex.codecogs.com/svg.latex?\gamma) является маленькой.

Увеличить надежность можно только увеличив объем выборки. Но существует множество задач, в которых новые измерения дорогостоящие. В этом случае вместо точечных оценок строят интервальные оценки.

Вместо одного числа предлагают целый интервал.
параметр ![](https://latex.codecogs.com/svg.latex?a\rightarrow&space;\tilde{a}) точечная оценка

![](https://latex.codecogs.com/svg.latex?\gamma&space;=&space;p(\left&space;|&space;\tilde{a}&space;-&space;a\right&space;|<\varepsilon&space;)), где ![](https://latex.codecogs.com/svg.latex?\varepsilon) - точечная оценка

Если ![](https://latex.codecogs.com/svg.latex?\varepsilon&space;\rightarrow&space;0,&space;\gamma&space;\rightarrow&space;1) - это хорошо.

![](https://latex.codecogs.com/svg.latex?\tilde{a}-\varepsilon&space;<&space;a&space;<&space;\tilde{a}&plus;\varepsilon&space;;&space;\tilde{a}-\varepsilon&space;=\tilde{a_{1}};\tilde{a}&plus;\varepsilon&space;=\tilde{a_{2}}) (1)

![](https://latex.codecogs.com/svg.latex?(\tilde{a_{1}},\tilde{a_{2}})) - доверительный интервал, который покрывает неизвестный параметр а с данной надежностью ![](https://latex.codecogs.com/svg.latex?\gamma)

Увеличиваем надежность, тогда теряем точность (интервал)

Доверительный интервал - интервальная оценка.

Заметим, из (1) полученный интервал всегда является симметричным относительно оценки.

Задача сводится к нахождению ![](https://latex.codecogs.com/svg.latex?\varepsilon)

![](https://latex.codecogs.com/svg.latex?\gamma) - Дано. То есть мы подгоняем интервал под надежность

#### Построение доверительных интервалов для неизвестного параметра а нормального распределения при известном параметре ![](https://latex.codecogs.com/svg.latex?\sigma)

![](https://latex.codecogs.com/svg.latex?f_{\varepsilon&space;}(x)=\frac{1}{\sqrt{2\pi&space;}\sigma&space;}&space;\cdot&space;e^{\frac{-(x-a)^2}{\sigma&space;^{2}}})

![](https://latex.codecogs.com/svg.latex?\sigma) - известная

требуется построить доверительный интервал ![](https://latex.codecogs.com/svg.latex?(\tilde{a_{1}},\tilde{a_{2}})), покрывающий неизвестный параметр a с заданной надежностью ![](https://latex.codecogs.com/svg.latex?\gamma) по выборочным значениям ![](https://latex.codecogs.com/svg.latex?x_{1},x_{2},...,x_{n})

Имеем:

![](https://latex.codecogs.com/svg.latex?a=M_{\xi&space;})

![](https://latex.codecogs.com/svg.latex?\tilde{a}=\tilde{M_{\xi&space;}}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})

ТОгда ![](https://latex.codecogs.com/svg.latex?\gamma&space;=&space;p(\left&space;|&space;\tilde{a}-a&space;\right&space;|<\varepsilon&space;)=p(\left&space;|&space;\tilde{M_{\xi&space;}}&space;-&space;M_{\xi}\right&space;|<\varepsilon&space;)=...=\Phi&space;(\frac{\varepsilon&space;\sqrt{n}}{\sqrt{D_{\xi&space;}}})=\Phi&space;(\frac{\varepsilon&space;\sqrt{n}}{\sigma&space;}))

![](https://latex.codecogs.com/svg.latex?\gamma&space;=&space;\Phi&space;(\frac{\varepsilon&space;\sqrt{n}}{\sigma&space;})&space;\rightarrow&space;\varepsilon&space;-&space;?)

По функции Лапласа по ![](https://latex.codecogs.com/svg.latex?\phi&space;(x)) получаем x ( по ![](https://latex.codecogs.com/svg.latex?\gamma) получаем ![](https://latex.codecogs.com/svg.latex?t_{\gamma&space;}))

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon&space;\sqrt{n}}{\sigma&space;}&space;=&space;t_{\gamma&space;}\Rightarrow&space;\varepsilon&space;=&space;\frac{t_{\gamma&space;}\cdot&space;\sigma&space;}{\sqrt{n}})

Раскрываем модуль:

![](https://latex.codecogs.com/svg.latex?\tilde{a}-\varepsilon&space;<&space;a&space;<&space;\tilde{a}&plus;\varepsilon&space;;&space;\tilde{a}-\varepsilon&space;=\tilde{a_{1}};\tilde{a}&plus;\varepsilon&space;=\tilde{a_{2}})

Подставляем:

![](https://latex.codecogs.com/svg.latex?\frac{1}{n}\sum_{i=1}^{n}\xi_{i}-&space;\frac{t_{\gamma&space;}\cdot&space;\sigma&space;}{\sqrt{n}}<a<\frac{1}{n}\sum_{i=1}^{n}\xi_{i}&plus;&space;\frac{t_{\gamma&space;}\cdot&space;\sigma&space;}{\sqrt{n}})

Пусть задана выборка (конкретные числа)

![](https://latex.codecogs.com/svg.latex?x_{1},x_{2},..,x_{n})

Нужно посчитать их среднее арифмитическое 

![](https://latex.codecogs.com/svg.latex?\bar{x}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})

И подставим так:

![](https://latex.codecogs.com/svg.latex?\bar{x}-&space;\frac{t_{\gamma&space;}\cdot&space;\sigma&space;}{\sqrt{n}}<a<\bar{x}&plus;&space;\frac{t_{\gamma&space;}\cdot&space;\sigma&space;}{\sqrt{n}})

Замечание: полученную формулу для доверительного интервала можно использовать для любого параметра

