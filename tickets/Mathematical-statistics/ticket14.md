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



