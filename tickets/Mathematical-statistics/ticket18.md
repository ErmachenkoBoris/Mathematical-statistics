# 18. Критерий согласия Пирсона для дискретных случайных величин.

### Проверка гипотезы о законе распределения при помощи критерия "Хи-квадрат" Пирсона (Согласия Пирсона)

Пусть гипотеза ![](https://latex.codecogs.com/svg.latex?H_{0}): случайная величина ![](https://latex.codecogs.com/svg.latex?\xi) имеет функция распределения ![](https://latex.codecogs.com/svg.latex?F_{\xi}(x)=) ______ - формула

Гипотеза ![](https://latex.codecogs.com/svg.latex?H_{1}): функция распределения - другая формула

Требуется проверить ![](https://latex.codecogs.com/svg.latex?H_{0}) с заданным уровнем значимости 
![](https://latex.codecogs.com/svg.latex?\alpha)

1) Рассмотрим случай, когда ![](https://latex.codecogs.com/svg.latex?\xi) - дискретная случайная величина. (второй случай в следующем билете)

Произведем n измерений этой случайной величины

|  ![](https://latex.codecogs.com/svg.latex?x_{i}) |  ![](https://latex.codecogs.com/svg.latex?x_{1}) |  ![](https://latex.codecogs.com/svg.latex?x_{2}) | ...  |  ![](https://latex.codecogs.com/svg.latex?x_{k}) |
|---|---|---|---|---|
| ![](https://latex.codecogs.com/svg.latex?n_{i})  | ![](https://latex.codecogs.com/svg.latex?n_{1})  | ![](https://latex.codecogs.com/svg.latex?n_{2})  | ...  |  ![](https://latex.codecogs.com/svg.latex?n_{k}) |
| ![](https://latex.codecogs.com/svg.latex?P^{*}_{i}=\frac{n_{i}}{n})  | ![](https://latex.codecogs.com/svg.latex?P^{*}_{1})   | ![](https://latex.codecogs.com/svg.latex?P^{*}_{2})   | ...  |  ![](https://latex.codecogs.com/svg.latex?P^{*}_{k})  |

Используя функцию распределения ![](https://latex.codecogs.com/svg.latex?H_{0}) посчитаем вероятности:

![](https://latex.codecogs.com/svg.latex?%5Cbegin%7Bmatrix%7D%20P_%7B1%7D%3DP%28%5Cxi%20%3D%20x_%7B1%7D%29%5C%5C%20P_%7B2%7D%3DP%28%5Cxi%20%3D%20x_%7B2%7D%29%20%5C%5C%20...%20%5C%5CP_%7Bk%7D%3DP%28%5Cxi%20%3D%20x_%7Bk%7D%29%20%5Cend%7Bmatrix%7D)

Мера расхождения между ними:

![](https://latex.codecogs.com/svg.latex?R=\sum_{i=1}^{k}C_{i}(p_{i}^{*}-p_{i})^2)

![](https://latex.codecogs.com/svg.latex?C_{i}) - веса, константы

Пирстон предложил в качестве ![](https://latex.codecogs.com/svg.latex?C_{i}) взять величину ![](https://latex.codecogs.com/svg.latex?\frac{n}{p_{i}})

![](https://latex.codecogs.com/svg.latex?R=\sum_{i=1}^{k}\frac{n}{p_{i}}\cdot&space;C_{i}(p_{i}^{*}-p_{i})^2&space;=&space;...&space;=\sum_{i=1}^{k}\frac{(n_{i}-np_{i})^2}{np_{i}})

В этой формуле ![](https://latex.codecogs.com/svg.latex?n_{1},&space;n_{2},&space;...,&space;n_{k}) есть случайные величины

Тогда R - это случайная величина

Пирсон доказал, что данная случайная величина при достаточно больших значений n не зависит
от функции ![](https://latex.codecogs.com/svg.latex?F_{\xi&space;}(x)) и имеет распределение Хи-квадрат

Пусть случайные величины ![](https://latex.codecogs.com/svg.latex?\xi_{1},&space;\xi_{2},&space;...,&space;\xi_{r}) являются независимыми и все они имеют стандартное нормальное распределение

![](https://latex.codecogs.com/svg.latex?\chi&space;=&space;\sum_{i=1}^{r}\xi&space;^{2}_{i})

(2 - это не квадрат, а обозначение)

Параметр r - называют число степеней свобод

Для нее составлено много разных таблиц, которыми мы можем пользоваться. Для использования этого критерия нужно найти число степеней свободы r

Если в гипотезе ![](https://latex.codecogs.com/svg.latex?H_{0}) указаны все параметры распределения точно, то число степеней свободы r вычисляется по формуле ![](https://latex.codecogs.com/svg.latex?r=k-1 ) 

Если в гипотезе ![](https://latex.codecogs.com/svg.latex?H_{0}) не все параметры указаны точно и S параметр приходится считать по выборке ![](https://latex.codecogs.com/svg.latex?r=k-1-S ) 

#### Правила применения критерия Хи-квадрат на практике

1. По полученным данным, где в таблице конкретные числа нужно вычислить R наблюдаемое

![](https://latex.codecogs.com/svg.latex?R=\sum_{i=1}^{k}\frac{(n_{i}-np_{i})^2}{np_{i}})

(это будет число, а не св)

2. Высчитываем r=k-1-S

3. Далее есть 2 пути (взависимости от таблиц)

I. Есть таблица критических точек

В ней ![](https://latex.codecogs.com/svg.latex?\alpha) - дано, а r мы высчитываем. По этим данным находим в ней ![](https://latex.codecogs.com/svg.latex?\chi_{cr}^{2})

Далее сравниваем:

Если R наблюдаемое  ![](https://latex.codecogs.com/svg.latex?\geq\chi_{cr}^{2}), то данные полученные не согласуются с гипотезой ![](https://latex.codecogs.com/svg.latex?H_{0}) и ее следует отвергнуть.

В противном случае(<) - данные согласуются и гипотезу следует принять

II Другие таблицы

сверху - r, слева - R наблюдаемое, на пересечении вероятности P

![](https://latex.codecogs.com/svg.latex?P_{0}=P(\chi&space;^{2}_{r}\geq&space;R))

Если ![](https://latex.codecogs.com/svg.latex?P_{0}\leq&space;\alpha) , то гипотезу ![](https://latex.codecogs.com/svg.latex?H_{0}) отвергаем, если ![](https://latex.codecogs.com/svg.latex?P_{0}>&space;\alpha), то гипотезу принимаем

 ![](https://latex.codecogs.com/svg.latex?\alpha) - берут больше нуля
