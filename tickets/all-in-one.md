# **ДВУМЕРНЫЕ СЛУЧАЙНЫЕ ВЕЛИЧИНЫ**

# 1. Свойства матрицы распределения вероятностей для дискретной двумерной с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) и с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) по матрице распределения.

![](https://latex.codecogs.com/svg.latex?(\xi_{1},&space;\xi_{2})) - двумерная случайная величина.

Для того, чтобы задать двумерную дискретную случайную величину, нужно задать все ее пары, а также все вероятности ![](https://latex.codecogs.com/svg.latex?P_{ij}). Тогда говорят, что задан __Закон рапределения вероятностей двумерной с.в.__

Если с.в. имеет конечное число значений, то вероятности ![](https://latex.codecogs.com/svg.latex?P_{ij}) удобно располагать в виде матрицы (__таблица распределения вероятностей__)

| ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) \ ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1})  |      ![](https://latex.codecogs.com/svg.latex?x_{1})      |  ![](https://latex.codecogs.com/svg.latex?x_{2}) |   ![](https://latex.codecogs.com/svg.latex?\dots)  ![](https://latex.codecogs.com/svg.latex?x_{i})   |   ![](https://latex.codecogs.com/svg.latex?\dots)      | ![](https://latex.codecogs.com/svg.latex?x_{n})
|----------|:------:|------:|------:|------:|------:|
| ![](https://latex.codecogs.com/svg.latex?y_{1}) |  ![](https://latex.codecogs.com/svg.latex?P_{11}) | ![](https://latex.codecogs.com/svg.latex?P_{21}) |       |
| ![](https://latex.codecogs.com/svg.latex?y_{2}) |    ![](https://latex.codecogs.com/svg.latex?P_{12})   | ![](https://latex.codecogs.com/svg.latex?P_{22}) |       |
| ![](https://latex.codecogs.com/svg.latex?\dots) |
| ![](https://latex.codecogs.com/svg.latex?y_{j}) | | | ![](https://latex.codecogs.com/svg.latex?P_{ij}) |
| ![](https://latex.codecogs.com/svg.latex?\dots) |
| ![](https://latex.codecogs.com/svg.latex?y_{m}) | | | | | ![](https://latex.codecogs.com/svg.latex?P_{ij}) |

![](https://latex.codecogs.com/svg.latex?P_{ij}=P(\{\xi_{1}=x_{i}\}\cap&space;\{\xi_{2}=y_{j}\})=P(\xi_{1}=x_{i},&space;\xi_{2}=y_{j}))

Свойства матрицы:

- ![](https://latex.codecogs.com/svg.latex?P_{ij}\geqslant&space;0,&space;\forall&space;i=\overline{1,n},&space;\forall&space;j=\overline{1,m})
- ![](https://latex.codecogs.com/svg.latex?\sum^{n}_{i=1}\sum^{m}_{j=1}P_{ij}=1)

Матрица задает __совместный закон распределения__.

### Утверждение:
Зная совместный закон распределения, т.е. матрицу, можно всегда и однозначно найти законы распределения отдельно для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) и ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2})

Построим ряды распределения отдельно для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) и ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2})

| ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1})  |      ![](https://latex.codecogs.com/svg.latex?x_{i})      |  ![](https://latex.codecogs.com/svg.latex?x_{1}) |   ![](https://latex.codecogs.com/svg.latex?\dots)  ![](https://latex.codecogs.com/svg.latex?x_{i})   |   ![](https://latex.codecogs.com/svg.latex?\dots)      | ![](https://latex.codecogs.com/svg.latex?x_{n})
|----------|:------:|------:|------:|------:|------:|
| |![](https://latex.codecogs.com/svg.latex?P(\xi_{i}=x_{i})) |  ![](https://latex.codecogs.com/svg.latex?P_{1}) | ![](https://latex.codecogs.com/svg.latex?P_{i}) | |      ![](https://latex.codecogs.com/svg.latex?P_{n})|

![](https://latex.codecogs.com/svg.latex?P(\xi_{i}=x_{i})=\sum^{m}_{j}P(\xi_{2}=y_{j})P(\xi_{1}=x_{i}/\xi_{2}=y_{j})=P(\xi_{1}=x_{i};\xi_{2}=y_{j})=\sum^{m}_{j=1}P_{ij}) - истинна теорема умножения для зависимых событий

![](https://latex.codecogs.com/svg.latex?P(A)=\sum_{j}P(H_{i})P(A/H_{i})) - функция полной вероятности

![](https://latex.codecogs.com/svg.latex?H_{1}=\{\xi_{1}=y_{1}\},&space;H_{2}=\{\xi_{2}=y_{2}\},&space;\dots,H_{m}=\{\xi_{m}=y_{m}\})

Для нахождения величины ![](https://latex.codecogs.com/svg.latex?P_{1}) нужно сложить все элементы из первого __столбца__, для нахождения ![](https://latex.codecogs.com/svg.latex?P_{i}) нужно сложить все элементы из i-того __столбца__ и т.д.

Аналогично получается ряд распределения для ![](https://latex.codecogs.com/svg.latex?\xi_{2})

| ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2})  |      ![](https://latex.codecogs.com/svg.latex?y_{j})      |  ![](https://latex.codecogs.com/svg.latex?x_{1}) |   ![](https://latex.codecogs.com/svg.latex?\dots)  ![](https://latex.codecogs.com/svg.latex?y_{j})   |   ![](https://latex.codecogs.com/svg.latex?\dots)      | ![](https://latex.codecogs.com/svg.latex?y_{m})
|----------|:------:|------:|------:|------:|------:|
| |![](https://latex.codecogs.com/svg.latex?P(\xi_{i}=y_{j})) |  ![](https://latex.codecogs.com/svg.latex?q_{1}) | ![](https://latex.codecogs.com/svg.latex?q_{i}) | |      ![](https://latex.codecogs.com/svg.latex?q_{m})|

Для нахождения величины ![](https://latex.codecogs.com/svg.latex?q_{1}) нужно сложить все элементы из первой __строки__ и т.д.

### Замечание

Но если известны отдельно ряды распределения для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) и для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}), то матрицу восстановить __нельзя__, т.к. обратный переход очень сложный.
# 2. Определение двумерной совместной функции распределения F(x,y), ее свойства.

![](https://latex.codecogs.com/svg.latex?F(x,y)_{-\infty<x,y<&plus;\infty}=P(\{\xi_{1}<x&space;\}\cap&space;\{\xi_{2}<y&space;\})=P(\xi_{1}<x,\xi_{2}<y)) - **совместная функция распределения**

### **Свойства**:
- ![](https://latex.codecogs.com/svg.latex?0\leqslant&space;F(x,y)\leqslant1,&space;\forall&space;x,&space;\forall&space;y)
- Функция убывает по каждому своему аргументу
- Функция непрерывна слева по каждому своему аргументу
- *Предельные свойства*
  - ![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow&space;-\infty,&space;y\rightarrow&space;-\infty}F(x,y)=&space;F(-\infty,&space;-\infty)=P(\xi_{1}<-\infty,&space;\xi_{2}<-\infty)=P(\O&space;)=0)
  - ![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow&space;-\infty,&space;\forall&space;y-fixed}F(x,y)=&space;F(-\infty,&space;y)=P(\xi_{1}<-\infty,&space;\xi_{2}<y)=P(\O&space;)=0)
  - ![](https://latex.codecogs.com/svg.latex?\lim_{\forall&space;x-fixed,&space;y\rightarrow&space;-\infty}F(x,y)=&space;F(x,-\infty)=P(\xi_{1}<x,&space;\xi_{2}<-\infty)=P(\O&space;)=0)
  - ![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow&space;&plus;\infty,&space;\forall&space;y\rightarrow&space;&plus;\infty}F(x,y)=&space;F(&plus;\infty,&space;&plus;\infty)=P(\xi_{1}<&plus;\infty,&space;\xi_{2}<&plus;\infty)=P(\Omega&space;)=1)
  - ![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow&space;&plus;\infty,&space;\forall&space;y-fixed}F(x,y)=&space;F(&plus;\infty,&space;y)=P(\xi_{1}<&plus;\infty,&space;\xi_{2}<y)=P(\xi_{2}<y)=F_{\xi_{2}}(y))
  - ![](https://latex.codecogs.com/svg.latex?\lim_{\forall&space;x-fixed,&space;y\rightarrow&space;&plus;\infty}F(x,y)=&space;F(x,&plus;\infty)=P(\xi{1}<x,\xi_{2}<&plus;\infty)=P(\xi_{1}<x)=F_{\xi_{1}}(x))
- Вероятность попадания с.в. ![](https://latex.codecogs.com/svg.latex?(\xi_1,\xi_2)) в прямоугольник
  ![](../images/two-dimensional_random_variables/ticket2-1.png)
  ![](https://latex.codecogs.com/svg.latex?a&space;\leqslant&space;x<b,&space;c&space;\leqslant&space;y<d)
  ![](https://latex.codecogs.com/svg.latex?P(a&space;\leqslant&space;\xi_1<b,&space;c&space;\leqslant&space;\xi_2<d)=F(b,d)&plus;F(a,c)-F(b,c)-F(a,d))

### Замечание
Если ![](https://latex.codecogs.com/svg.latex?(\xi_1,\xi_2)) непрерывного типа, то:
- Функция F(x,y) также непрерывна справа по каждому своему аргументу, т.е. является просто непрерывной функцией и по x, и по y.
- Вероятность попадания в прямоугольник будет вычисляться независимо от того, как стоят знаки.


![](https://latex.codecogs.com/svg.latex?F_\xi_1(x)=F_{\xi_1\xi_2}(x,&plus;\infty))
![](https://latex.codecogs.com/svg.latex?F_\xi_2(y)=F_{\xi_1\xi_2}(&plus;\infty,y))

Зная совместную двумерную функцию распределения, можно всегда, и притом однозначно, получить фукнции распределения отдельно для ![](https://latex.codecogs.com/svg.latex?\xi_1) и для ![](https://latex.codecogs.com/svg.latex?\xi_2). Неверно в обратную сторону.
# 3. Способ нахождения F(x,y) из матрицы распределения для двумерной дискретной с.в.

Двумерная с.в. ![](https://latex.codecogs.com/svg.latex?(\xi_1,\xi_2)) имеет распределение, заданное матрицей.

| ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) \ ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) |  -1   |    0 |    1 |
| ------------------------------------------------------------------------------------------------------------------- | :---: | ---: | ---: |
| -1                                                                                                                  |  1/6  |  1/6 |  1/8 |
| 1                                                                                                                   |  1/4  |  1/8 |  1/6 |

| ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) |      ![](https://latex.codecogs.com/svg.latex?x_{i})       |           -1 |            0 |            1 |
| -------------------------------------------------------- | :--------------------------------------------------------: | -----------: | -----------: | -----------: |
|                                                          | ![](https://latex.codecogs.com/svg.latex?P(\xi_{1}=x_{i})) | 1/6+1/4=5/12 | 1/6+1/8=7/24 | 1/8+1/6=7/24 |

| ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) |      ![](https://latex.codecogs.com/svg.latex?y_{j})       |                -1 |                 1 |
| -------------------------------------------------------- | :--------------------------------------------------------: | ----------------: | ----------------: |
|                                                          | ![](https://latex.codecogs.com/svg.latex?P(\xi_{2}=y_{j})) | 1/6+1/6+1/8=11/24 | 1/4+1/8+1/6=13/24 |

F(x,y) удобно записывать в виде таблицы. Разобьем всю плоскость на прямоугольники следующего вида: ось OX разобьем значениями с.в. ![](https://latex.codecogs.com/svg.latex?\xi_1), ось OY - значениями ![](https://latex.codecogs.com/svg.latex?\xi_2).

| y \ x       | x <= 1 | -1 < x <= 0 | 0 < x <= 1 | x > 1 |
| ----------- | :----: | ----------: | ---------: | ----: |
| y <= -1     | 0 (1)  |           0 |          0 |     0 |
| -1 < y <= 1 |   0    |         1/6 |    1/3 (2) | 11/24 |
| y > 1       |   0    |        5/12 |      17/24 | 1 (3) |

1) Элементы первой строки и столба всегда равны 0.
2) Пусть x=1/2, y=0 (любые значения ихз подходящего интервала)
   ![](https://latex.codecogs.com/svg.latex?F(\frac{1}{2};0)=P(\xi_1&space;<&space;\frac{1}{2};\xi_2<0)=P(\xi_1=-1;\xi_2=1)&plus;P(\xi_1=0;\xi_2=1)=\frac{1}{6}&plus;\frac{1}{6}=\frac{1}{3})

   Значения 1/6 и 1/6 взяты из первой таблицы.
3) Значение правого нижнего элемента всегда равно 1.
4) Значения в строке и столбце возрастают.
# 4. Определение двумерной непрерывной с.в. Свойства двумерной плотности распределения f(x,y). Формулы, связывающие f(x,y) и F(x,y), и формулы, позволяющие находить плотности с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) и с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) через f(x,y).

При изучении двумерной непрерывной случайной с.в. ![](https://latex.codecogs.com/svg.latex?(\xi&space;_{1},\xi&space;_{2})) ее удобно интерпретировать как случайную точку на плоскости, при этом значение ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) по оси OX, а значение ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) - по оси OY.

__Непрерывная двумерная с.в.__ - двумерная с.в., значения которой сплошь покрывают некоторую область действительной плоскости или всю эту плоскость.

__f(x,y)__ - двумерная (совместная) плотность распределения вероятностей двумерной с.в. ![](https://latex.codecogs.com/svg.latex?(\xi&space;_{1},\xi&space;_{2})) 

### Свойства
- ![](https://latex.codecogs.com/svg.latex?f(x,y)&space;\geqslant&space;0,&space;\forall&space;x,&space;\forall&space;y)
- ![](https://latex.codecogs.com/svg.latex?P((\xi_1,\xi_2))&space;\in&space;D=\iint_{D}f(U,V)dUdV) - случайная точка попадет в некоторую область D

### Следствия
1. Возьмем в качестве D всю плоскость (![](https://latex.codecogs.com/svg.latex?R^2)) и найдем вероятность

![](https://latex.codecogs.com/svg.latex?1=P((\xi_1,\xi_2))&space;\in&space;R^2=\iint_{D}f(U,V)dUdV=&space;\int_{-\infty}^{&plus;\infty}\int_{-\infty}^{&plus;\infty}f(U,V)dUdV=\int_{-\infty}^{&plus;\infty}\int_{-\infty}^{&plus;\infty}f(x,y)dxdy=1)

2. Нарисуем на плоскости и рассмотрим прямоугольник D

![](../images/two-dimensional_random_variables/ticket4-1.png)

![](https://latex.codecogs.com/svg.latex?D%3D%5C%7B%28U%2CV%29%3AU%3Cx%2C%20V%3Cy%20%5C%7D)

![](https://latex.codecogs.com/svg.latex?P((\xi_1,\xi_2)&space;\in&space;D)=P(\xi_1<x,\xi_2<y)(==F_{\xi_1\xi_2}(x,y))=\int_{-\infty}^x\int_{-\infty}^yf(U,V)dUdV)

![](https://latex.codecogs.com/svg.latex?F_%7B%5Cxi_1%5Cxi_2%7D%28x%2Cy%29%3D%5Cint_%7B-%5Cinfty%7D%5Ex%5Cint_%7B-%5Cinfty%7D%5Eyf%28U%2CV%29dUdV%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%20%5Cint_%7B-%5Cinfty%7D%5ExdU%28%5Cint_%7B%5Cinfty%7D%5Eyf%28U%2CV%29dV%29%5C%5C%20%5Cint_%7B-%5Cinfty%7D%5EydV%28%5Cint_%7B%5Cinfty%7D%5Exf%28U%2CV%29dU%29%20%5Cend%7Bmatrix%7D%5Cright.)

  2.1. ![](https://latex.codecogs.com/svg.latex?f(x,y)&space;\rightarrow&space;F(x,y))
  2.2. ![](https://latex.codecogs.com/svg.latex?F(x,y),f(x,y)=\frac{\partial^2&space;F(x,y)}{\partial&space;x\partial&space;y})

Зная совсместную плотность, можно всегда и притом однозначно найти плотность отдельно для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) и для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2})

- ![](https://latex.codecogs.com/svg.latex?f_{\xi_1}(x)=\int_{-\infty}^{&plus;\infty}f(x,y)dy)
- ![](https://latex.codecogs.com/svg.latex?f_{\xi_2}(y)=\int_{-\infty}^{&plus;\infty}f(x,y)dx)

### Замечание

Но зная отдельно ![](https://latex.codecogs.com/svg.latex?f_{\xi_1}(x)) и ![](https://latex.codecogs.com/svg.latex?f_{\xi_2}(y)) в общем случае нельзя найти ![](https://latex.codecogs.com/svg.latex?f_{\xi_1\xi_2}(x,y))
# 5. Понятие независимости двух с.в. Критерии независимости для дискретных и непрерывных с.в.

Случайные величины называются независимыми, если:

![](https://latex.codecogs.com/svg.latex?\forall&space;x,&space;\forall&space;y&space;\Rightarrow&space;F_{\xi_1\xi_2}(x,y)=F_\xi_1(x)F_\xi_2(y))

![](https://latex.codecogs.com/svg.latex?F_\xi_1(x)=F_{\xi_1\xi_2}(x,&plus;\infty);&space;F_\xi_2(y)=F_{\xi_1\xi_2}(&plus;\infty,y))

### Следствия
1. Для двумерных дискретных с.в. (__Критерий независимоссти дискретных с.в.__)

   ![](https://latex.codecogs.com/svg.latex?\xi_1:x_1,x_2,&space;\dots,&space;x_i,&space;\dots)
   ![](https://latex.codecogs.com/svg.latex?\xi_2:y_1,y_2,&space;\dots,&space;y_j,&space;\dots)

   Если ![](https://latex.codecogs.com/svg.latex?\xi_1) и ![](https://latex.codecogs.com/svg.latex?\xi_2) дискретные с.в., то для того, чтобы они были независимы, необходимо и достаточно, чтобы ![](https://latex.codecogs.com/svg.latex?\forall&space;x_i&space;\in&space;\xi_1,\forall&space;y_j&space;\in&space;\xi_2) выполнялось условие:

   ![](https://latex.codecogs.com/svg.latex?%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%20P_%7Bij%7D%3DP%28%5Cxi_1%3Dx_i%2C%5Cxi_2%3Dy_j%29%3DP%28%5Cxi_1%3Dx_i%29P%28%5Cxi_2%3Dy_j%29%5C%5C%20%5Cforall%20x_i%2C%5Cforall%20y_j%20%5Cend%7Bmatrix%7D%5Cright.)
2. Для непрерывных с.в.

  Для того, чтобы непрерывные с.в. ![](https://latex.codecogs.com/svg.latex?\xi_1) и ![](https://latex.codecogs.com/svg.latex?\xi_2) были независимы, необходимо и достаточно:

  ![](https://latex.codecogs.com/svg.latex?\forall&space;x_i,\forall&space;y_j&space;\rightarrow&space;f_{\xi_1\xi_2}(x,y)=f_\xi_1(x)f_\xi_2(y))
# 6. Пример нахождения условных законов распределения для двух дискретных с.в.

Если ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) независимы, то ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) ведет себя так, будто ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) не существует, и наоборот.

Рассмотрим случай, когда ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) и ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) зависимы. Тогда распределение одной будет зависеть от того, какое значение приняла другая с.в.

Пусть ![](https://latex.codecogs.com/svg.latex?(\xi&space;_{1},\xi&space;_{2})) - дискретная с.в.

   ![](https://latex.codecogs.com/svg.latex?\xi_1:x_1,x_2,&space;\dots,&space;x_i,&space;\dots)
   ![](https://latex.codecogs.com/svg.latex?\xi_2:y_1,y_2,&space;\dots,&space;y_j,&space;\dots)

Пусть ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) приняла значение ![](https://latex.codecogs.com/svg.latex?y_j), т.е. ![](https://latex.codecogs.com/svg.latex?%5C%7B%5Cxi_2%3Dy_j%5C%7D). Найдем условный закон распределения ![](https://latex.codecogs.com/svg.latex?\xi&space;_1), при условии ![](https://latex.codecogs.com/svg.latex?\xi_2=y_j). Это будет набор из следующих условных вероятностей:

![](https://latex.codecogs.com/svg.latex?%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%20P%28%5Cxi_1%3Dx_1/%5Cxi_2%3Dy_j%29%5C%5C%20%5Cdots%20%5C%5C%20P%28%5Cxi_1%3Dx_i/%5Cxi_2%3Dy_j%29%5C%5C%20%5Cdots%20%5Cend%7Bmatrix%7D%5Cright.)

Набор этих условных вероятностей - __условный закон распределения__ для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}). Аналогично находится и для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}).

### Замечание

В любом условном законе сумма условных вероятностей равна 1.

### Способ нахождения условной вероятности для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1})

![](https://latex.codecogs.com/svg.latex?P(\xi_1=x_i/\xi_2=y_j)=\frac{P(\xi_1=x_1;\xi_2=y_j)}{P(\xi_2=y_j)}), где верхняя часть равна![](https://latex.codecogs.com/svg.latex?P_{ij}) в матрицы, а нижняя находится с помощью той же матрицы.

### Замечание

Для того, чтобы найти матрицу распределения для 2 дискретных с.в., нужно знать безусловный закон распределения для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) и все условные законы распределения для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}).

## Примеров нет, импровизируйте.
# 7. Способ задания условных законов распределения для двух непрерывных с.в., пример.

Пусть ![](https://latex.codecogs.com/svg.latex?(\xi&space;_{1},\xi&space;_{2})) - двумерная непрерывная с.в.

Условный закон распределения для с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}), при условии, что ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) приняла значение y, задается __условной плотностью распределения ![](https://latex.codecogs.com/svg.latex?f_{\xi_1/\xi_2}(x/y))__.

![](https://latex.codecogs.com/svg.latex?f_{\xi_1/\xi_2}(x/y)=\frac{f_{\xi_1,\xi_2}(x,y)}{f_{\xi_2}(y)}&space;\Rightarrow&space;f_{\xi_1,\xi_2}(x,y)=f_{\xi_1/\xi_2}(x/y)f_{\xi_2}(y)) - по __теореме умножения плотностей__.

Аналогично для y.

### Замечание

Для нахождения двумерной (совместной) плотности, нужно знать безусловную плотность одной с.в., и условную плотность другой.

## Теорема умножения для плотностей

Если ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1},\xi&space;_{2}) независимы, то как для дискретной с.в., так и для непрерывной с.в. по определению получим, что __все условные вероятности равны безусловным__.

## Пример

![](../images/two-dimensional_random_variables/ticket7-1.jpg)
# 8. Основные числовые характеристики двумерной с.в. и формулы для нахождения центра рассеивания, величины разброса по осям, ковариации и корреляционной матрицы.

## Центр разброса (рассеивания)

Точка на плоскости с координатами ![](https://latex.codecogs.com/svg.latex?(M\xi_1,M\xi_2))

![](../images/two-dimensional_random_variables/ticket8-1.png)

## Величина разброса

Для вычисления ![](https://latex.codecogs.com/svg.latex?D\xi_i) удобно найти отдельно закон распределения для ![](https://latex.codecogs.com/svg.latex?\xi_1) и для ![](https://latex.codecogs.com/svg.latex?\xi_2). Потом взять формулы для одномерных с.в.

![](https://latex.codecogs.com/svg.latex?D\xi_1) - по OX.
![](https://latex.codecogs.com/svg.latex?D\xi_2) - по OY.

## Ковариация с.в.

![](https://latex.codecogs.com/svg.latex?COV%28%5Cxi_1%2C%5Cxi_2%29%3DM%5C%7B%28%5Cxi_1-M%5Cxi_1%29%28%5Cxi_2-M%5Cxi_2%29%5C%7D%28definition%29%3DM%28%5Cxi_1%5Cxi_2%29-M%5Cxi_1M%5Cxi_2%28convenient%20formula%29)

![](https://latex.codecogs.com/svg.latex?M%28%5Cxi_1%5Cxi_2%29%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%20%5Csum_i%5Csum_jx_iy_jp_%7Bij%7D%2C%20%28%5Cxi_1%2C%5Cxi_2%29-discrete%5C%5C%20%5Cint_%7B-%5Cinfty%7D%5E%7B&plus;%5Cinfty%7D%5Cint_%7B-%5Cinfty%7D%5E%7B&plus;%5Cinfty%7Dxyf_%7B%5Cxi_1%5Cxi_2%7D%28x%2Cy%29%2C%28%5Cxi_1%2C%5Cxi_2%29-continuous%20%5Cend%7Bmatrix%7D%5Cright.)

## Корреляция (нормированная ковариация)

![](https://latex.codecogs.com/svg.latex?corr(\xi_1,\xi_2)=\frac{COV(\xi_1,\xi_2)}{\sqrt{D(\xi_1)}\sqrt{D(\xi_2)}}=\frac{COV(\xi_1,\xi_2)}{\sigma\xi_1\sigma\xi_2})

Величина corr характеризует степень _линейной_ зависимости между ![](https://latex.codecogs.com/svg.latex?\xi_1) и ![](https://latex.codecogs.com/svg.latex?\xi_2)

### Свойства корреляции

1. ![](https://latex.codecogs.com/svg.latex?\left&space;|&space;corr&space;\right&space;|&space;\leqslant&space;1)
2. Пусть ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) связаны __жесткой (функциональной) линейной зависимостью__.

  ![](https://latex.codecogs.com/svg.latex?\xi_2=a\xi_1&plus;b,&space;a,b&space;\in&space;R,&space;a\neq0)

  В этом случае ![](https://latex.codecogs.com/svg.latex?corr(\xi_1,\xi_2)) будет максимальна по модулю.

  ![](https://latex.codecogs.com/svg.latex?corr%28%5Cxi_1%2C%5Cxi_2%29%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%201%2C%20a%3E0%5C%5C%20-1%2C%20a%3C0%20%5Cend%7Bmatrix%7D%5Cright.)

3. Обратное к предыдущему свойству.

  Если ![](https://latex.codecogs.com/svg.latex?\left&space;|&space;corr&space;\right&space;|&space;=&space;1), то между ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) __обязательно__ есть жесткая линейная зависимость.

4.Если ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) независимы, то corr=0.

  ![](https://latex.codecogs.com/svg.latex?corr(\xi_1,\xi_2)=\frac{COV(\xi_1\xi_2)}{\sigma\xi_1\sigma\xi_2}=\frac{M(\xi_1\xi_2)-M(\xi_1)M(\xi_2)}{\sigma\xi_1\sigma\xi_2}=0)

5. Обратное к предыдущему свойству.

  Если corr=0, то это __не означает__, что с.в. независимы.

  - Если corr > 0, то говорят, что ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) связаны __положительной корреляцией__, т.е. при возрастании одной с.в. возрастает и другая
  - Если corr < 0, то говорят, что ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) связаны __отрицательной корреляцией__, т.е. при возрастании одной с.в. другая убывает.
  - Если corr = 0, то говорят, что ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) __некоррелированы__, т.е. между ними нет линейной зависимости.

# Корреляционная матрица

![](https://latex.codecogs.com/svg.latex?%5Cbegin%7Bpmatrix%7D%20cov%28%5Cxi_1%2C%5Cxi_1%29%26%20cov%28%5Cxi_1%2C%5Cxi_2%29%5C%5C%20cov%28%5Cxi_2%2C%5Cxi_1%29%26%20cov%28%5Cxi_2%2C%5Cxi_2%29%20%5Cend%7Bpmatrix%7D) - корреляционная матрица

![](https://latex.codecogs.com/svg.latex?cov%28%5Cxi_1%2C%5Cxi_1%29%3DM%28%28%5Cxi_1-M%5Cxi_1%29%28%5Cxi_1-M%5Cxi_1%29%29%3DM%5C%7B%28%5Cxi_1-M%5Cxi_1%29%5E2%5C%7D%3DD%5Cxi_1)

![](https://latex.codecogs.com/svg.latex?cov(\xi_2,\xi_1)=M((\xi_2-M\xi_2)(\xi_-M\xi_1))=&space;cov(\xi_1,\xi_2))

![](https://latex.codecogs.com/svg.latex?cov(\xi_2,\xi_2)) и ![](https://latex.codecogs.com/svg.latex?cov(\xi_2,\xi_1)) находятся аналогично.

![](https://latex.codecogs.com/svg.latex?%5Cbegin%7Bpmatrix%7D%20D%5Cxi_1%26%20cov%28%5Cxi_1%2C%5Cxi_2%29%5C%5C%20cov%28%5Cxi_1%2C%5Cxi_2%29%26%20D%5Cxi_2%20%5Cend%7Bpmatrix%7D)

![](https://latex.codecogs.com/svg.latex?cov(\xi_1,\xi_2)=M(\xi_1,\xi_2)-M\xi_1M\xi_2)

1. ![](https://latex.codecogs.com/svg.latex?M(\xi_1,\xi_2)=&space;M\xi_1M\xi_2&plus;cov(\xi_1,\xi_2))

  ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) - независимы ![](https://latex.codecogs.com/svg.latex?\Rightarrow&space;M(\xi_1,\xi_2)=M\xi_1M\xi_2)

2. ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) - независимы ![](https://latex.codecogs.com/svg.latex?\Rightarrow&space;D(\xi_1&plus;\xi_2)=D\xi_1&plus;D\xi_2)

  ![](https://latex.codecogs.com/svg.latex?D%28%5Cxi_1&plus;%5Cxi_2%29%3DM%5C%7B%28%5Cxi_1&plus;%5Cxi_2-M%28%5Cxi_1&plus;%5Cxi_2%29%5E2%29%5C%7D%3DM%5C%7B%28%5Cxi_1-m%5Cxi_1%29&plus;%28%5Cxi_2-M%5Cxi_2%29%5E2%5C%7D%3DM%5C%7B%28%5Cxi_1-m%5Cxi_1%5E2%29&plus;2%28%5Cxi_1-M%5Cxi_1%29%28%5Cxi_2-M%5Cxi_2%29&plus;%28%5Cxi_2-M%5Cxi_2%29%5E2%5C%7D%3DM%5C%7B%28%5Cxi_1-m%5Cxi_1%5E2%29%5C%7D&plus;2M%5C%7B%28%5Cxi_1-M%5Cxi_1%29%28%5Cxi_2-M%5Cxi_2%29%5C%7D&plus;M%5C%7B%28%5Cxi_2-M%5Cxi_2%29%5E2%5C%7D%3DD%5Cxi_1&plus;D%5Cxi_2&plus;2cov%28%5Cxi_1%5C%2C%5Cxi_2%29)
3. ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) - зависимы

  ![](https://latex.codecogs.com/svg.latex?D(\xi_1&plus;\xi_2)=D\xi_1&plus;D\xi_2&plus;cov(\xi_1\,\xi_2))
# 9. Свойства корреляции двух с.в.

## Корреляция (нормированная ковариация)

![](https://latex.codecogs.com/svg.latex?corr(\xi_1,\xi_2)=\frac{COV(\xi_1,\xi_2)}{\sqrt{D(\xi_1)}\sqrt{D(\xi_2)}}=\frac{COV(\xi_1,\xi_2)}{\sigma\xi_1\sigma\xi_2})

Величина corr характеризует степень _линейной_ зависимости между ![](https://latex.codecogs.com/svg.latex?\xi_1) и ![](https://latex.codecogs.com/svg.latex?\xi_2)

### Свойства корреляции

1. ![](https://latex.codecogs.com/svg.latex?\left&space;|&space;corr&space;\right&space;|&space;\leqslant&space;1)
2. Пусть ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) связаны __жесткой (функциональной) линейной зависимостью__.

  ![](https://latex.codecogs.com/svg.latex?\xi_2=a\xi_1&plus;b,&space;a,b&space;\in&space;R,&space;a\neq0)

  В этом случае ![](https://latex.codecogs.com/svg.latex?corr(\xi_1,\xi_2)) будет максимальна по модулю.

  ![](https://latex.codecogs.com/svg.latex?corr%28%5Cxi_1%2C%5Cxi_2%29%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%201%2C%20a%3E0%5C%5C%20-1%2C%20a%3C0%20%5Cend%7Bmatrix%7D%5Cright.)

3. Обратное к предыдущему свойству.

  Если ![](https://latex.codecogs.com/svg.latex?\left&space;|&space;corr&space;\right&space;|&space;=&space;1), то между ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) __обязательно__ есть жесткая линейная зависимость.

4.Если ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) независимы, то corr=0.

  ![](https://latex.codecogs.com/svg.latex?corr(\xi_1,\xi_2)=\frac{COV(\xi_1\xi_2)}{\sigma\xi_1\sigma\xi_2}=\frac{M(\xi_1\xi_2)-M(\xi_1)M(\xi_2)}{\sigma\xi_1\sigma\xi_2}=0)

5. Обратное к предыдущему свойству.

  Если corr=0, то это __не означает__, что с.в. независимы.

  - Если corr > 0, то говорят, что ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) связаны __положительной корреляцией__, т.е. при возрастании одной с.в. возрастает и другая
  - Если corr < 0, то говорят, что ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) связаны __отрицательной корреляцией__, т.е. при возрастании одной с.в. другая убывает.
  - Если corr = 0, то говорят, что ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) __некоррелированы__, т.е. между ними нет линейной зависимости.
___
___
___
___
# **МАТЕМАТИЧЕСКАЯ СТАТИСТИКА**
# 1. Предмет математической статистики. Специфика ее задач по сравнению c задачами теории вероятностей. Три основные задачи математической статистики.
**Математическая статистика** - раздел Теории вероятностей, в котором разрабатываются приемы и методы сбора, обработки и анализа экспериментальных данных с целью построения на основе этих данных адекватной вероятностной модели изучаемого случайного явления.

Математическая статистика имеет очень большую область практического применения. Она выделяется в отдельный раздел так как решает специфические задачи по сравнению с теми что решает Теория Вероятности. Их можно назвать обратными к задачам Теории вероятности.

|      | Имеем                                                | Рассчитываем                                                |
| ---- | ---------------------------------------------------- | ---------------------------------------------------------- |
| Т.В. | Вероятностная модель. Вероятность случайного события | Реальное течение процесса.  Частота происхождения процесса |
| М.С. | Реальные числовые данные                             | Подходящую адекватную вероятностную модель                 |

Основные типы задач решаемые В математической статистике:

1. Нахождение статистических законов распределения и статистических числовых характеристик
2. Оценивание неизвестных параметров распределения по статистическим данным
3. Проверка тех или иных предположений о законах распределения или параметрах этого распределения. Проверка статистических гипотез.
# 2. Понятие генеральной совокупности и выборки. Независимая выборка.
**Генеральная совокупность** ![](https://latex.codecogs.com/svg.latex?\Gamma) - множество элементов одинаковой физической природы для которых изучаются свойства некоторого их количественного признака.
N - **количество элементов**, объем ![](https://latex.codecogs.com/svg.latex?\Gamma)

Количественный признак ![](https://latex.codecogs.com/svg.latex?\Gamma) - случайная величина.

Выберем из ![](https://latex.codecogs.com/svg.latex?\Gamma) определенным образом n элементов.
V - **выборка**, n - **объем выборки**.

Обозначим количественные признаки:
Для первого элемента ![](https://latex.codecogs.com/svg.latex?\xi_{1})
Для второго элемента ![](https://latex.codecogs.com/svg.latex?\xi_{2})
...
Для n-го элемента ![](https://latex.codecogs.com/svg.latex?\xi_{n})

![](https://latex.codecogs.com/svg.latex?\xi_{1}),...,![](https://latex.codecogs.com/svg.latex?\xi_{n}) - это не новые случайные величины, а переобозначенная ![](https://latex.codecogs.com/svg.latex?\xi) (Экземпляр С.В.)

Все ![](https://latex.codecogs.com/svg.latex?\xi_{1}),...,![](https://latex.codecogs.com/svg.latex?\xi_{n}) одинаково распределены, так же как и ![](https://latex.codecogs.com/svg.latex?\xi\Rightarrow) одинаковые числовые характеристики.

### Основное правило получения выборки:
* Каждый элемент генеральной совокупности должен иметь равное право попасть в выборку.

Выборка должна быть репрезентативной **(адекватно представлять генеральную совокупность)**
Это правило обеспечивает независимость всех С.В. ![](https://latex.codecogs.com/svg.latex?\xi_{1}),...,![](https://latex.codecogs.com/svg.latex?\xi_{n})

Независимые, одинаково распределенные и упорядоченные С.В. ![](https://latex.codecogs.com/svg.latex?\xi_{1}),...,![](https://latex.codecogs.com/svg.latex?\xi_{n}) называются **повторной выборкой** объема n из ![](https://latex.codecogs.com/svg.latex?\Gamma).

Будем использовать только ее. (![](https://latex.codecogs.com/svg.latex?n\ll&space;N))
# 3. Простой и вариационный статистические ряды. Статистическое распределение выборки. Информационно-статистическая таблица.
Измерим ![](https://latex.codecogs.com/svg.latex?\xi_{1}),...,![](https://latex.codecogs.com/svg.latex?\xi_{n}) и найдем их значения.

![](https://latex.codecogs.com/svg.latex?%5Cleft.%5Cbegin%7Bmatrix%7D%20%5Cxi%20_%7B1%7D%5Crightarrow%20x_%7B1%7D%20%5C%5C%20%5Cxi%20_%7B2%7D%5Crightarrow%20x_%7B2%7D%20%5C%5C%20...%5C%5C%20%5Cxi%20_%7Bn%7D%5Crightarrow%20x_%7Bn%7D%20%5Cend%7Bmatrix%7D%5Cright%5C%7D) статистические данные

![](https://latex.codecogs.com/svg.latex?\xi_{1}),...,![](https://latex.codecogs.com/svg.latex?\xi_{n}) - С.В.

![](https://latex.codecogs.com/svg.latex?x_{1}),...,![](https://latex.codecogs.com/svg.latex?x_{n}) - числа

| N | 1 | 2 | ... | n  |
|---|---|---|-----|----|
| Значение ![](https://latex.codecogs.com/svg.latex?\xi) | ![](https://latex.codecogs.com/svg.latex?x_{1}) | ![](https://latex.codecogs.com/svg.latex?x_{2}) | ... | ![](https://latex.codecogs.com/svg.latex?x_{n}) | 

Это **простой статистический ряд**

Если эти значения упорядочиваются в порядке возрастания, то этот ряд называется **вариационным**
![](https://latex.codecogs.com/svg.latex?x_{1}\leq&space;x_{2}\leq...\leq&space;x_{n})

**Вариационный ряд** - сами значения  - варианты.

При наблюдении за дискретными или непрерывными случайными величинами, при округлении их значений может быть много одинаковых значений.
Удобно из этой таблицы выделить только разные значения и посчитать сколько они встречались.

Пусть уникальных будет ![](https://latex.codecogs.com/svg.latex?k\leq&space;n)

| ![](https://latex.codecogs.com/svg.latex?x_{i})                     | ![](https://latex.codecogs.com/svg.latex?x_{1})      | ![](https://latex.codecogs.com/svg.latex?x_{2})      | ... | ![](https://latex.codecogs.com/svg.latex?x_{k})      |
|---------------------------------------------------------------------|------------------------------------------------------|------------------------------------------------------|-----|------------------------------------------------------|
| ![](https://latex.codecogs.com/svg.latex?n_{i})                     | ![](https://latex.codecogs.com/svg.latex?n_{1})      | ![](https://latex.codecogs.com/svg.latex?n_{2})      | ... | ![](https://latex.codecogs.com/svg.latex?n_{k})      |
| ![](https://latex.codecogs.com/svg.latex?p_{i}^{*}=\frac{n_{i}}{n}) | ![](https://latex.codecogs.com/svg.latex?\frac{n_{1}}{n}) | ![](https://latex.codecogs.com/svg.latex?\frac{n_{2}}{n}) | ...    | ![](https://latex.codecogs.com/svg.latex?\frac{n_{k}}{n}) |

Это **статистическое распределение выборки**.

![](https://latex.codecogs.com/svg.latex?\sum_{i=1}^{k}n_{i}=n)

![](https://latex.codecogs.com/gif.latex?\sum_{i=1}^{k}p_{i}^{*}=1)

На практике даже такие таблицы трудно обозримы, а информация в них бывает лишней при решении. Поэтому данные укрупняют.

Расположим данные на оси.
Разобьем интервал от ![](https://latex.codecogs.com/svg.latex?x_{1}) до ![](https://latex.codecogs.com/svg.latex?x_{k}) на разряды по S штук

![](../images/Mathematical-statistics/ticket03.png)

![](https://latex.codecogs.com/svg.latex?y_{1}<y_{2}<...<y_{s}<y_{s&plus;1})

![](https://latex.codecogs.com/svg.latex?y_{1}\leq&space;x_{1})

![](https://latex.codecogs.com/svg.latex?y_{s&plus;1}\geq&space;x_{k})

Дальше считают сколько элементов выборки попало в каждый разряд.

| Разряды                                                             | ![](https://latex.codecogs.com/svg.latex?[y_{1},y_{2}]) | ![](https://latex.codecogs.com/svg.latex?[y_{2},y_{3}]) | ... | ![](https://latex.codecogs.com/svg.latex?[y_{s},y_{s+1}]) |
|---------------------------------------------------------------------|---------------------------------------------------------|---------------------------------------------------------|-----|-----------------------------------------------------------|
| ![](https://latex.codecogs.com/svg.latex?L_{i})                     | ![](https://latex.codecogs.com/svg.latex?L_{1})         | ![](https://latex.codecogs.com/svg.latex?L_{2})         | ... | ![](https://latex.codecogs.com/svg.latex?L_{s})           |
| ![](https://latex.codecogs.com/svg.latex?L_{i}^{*}=\frac{L_{i}}{n}) | ![](https://latex.codecogs.com/svg.latex?L_{1}^{*})     | ![](https://latex.codecogs.com/svg.latex?L_{2}^{*})     | ... | ![](https://latex.codecogs.com/svg.latex?L_{s}^{*})       |

![](https://latex.codecogs.com/svg.latex?\sum_{i=1}^{s}L_{i}=n)

Иногда разряды выбираются со спецификой задачи.
Такая таблица называется **информационно статистической** или **группированным статистическим рядом**.
# 4. Эмпирическая функция распределения, ее свойства. Полигон относительных частот и гистограмма.

У любой С.В. есть функция распределения
![](https://latex.codecogs.com/svg.latex?F_{\xi}(x)=P(\xi<x),&space;x\in&space;R)

![](https://latex.codecogs.com/svg.latex?F^{*}(x)) - **эмпирическая/статистическая функция распределения**

![](https://latex.codecogs.com/svg.latex?F_{n}^{*}(x)=P^{*}(\xi<x)=\frac{m(x)}{n}) 

n - общее количество элементов выборки

m(x) - число элементов выборки которые строго меньше x

**Свойства** такие же как и у F(x), график такой же как и у Д.С.В.:

1. ![](https://latex.codecogs.com/svg.latex?0\leq&space;F^{*}(x)\leq&space;1)
2. Функция является неубывающей по своему аргументу ![](https://latex.codecogs.com/svg.latex?x_{1}<x_{2}&space;\rightarrow&space;F(x_{1})\leq&space;F(x_{2}))
3. Непрерывна слева
![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow&space;x_{0}-0}F(x)=F(x_{0}))
Если ξ – непрерывная С.В., то ее функция распределения является непрерывной и справа.
4. ![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow-\infty}F(x)=0)

    ![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow+\infty}F(x)=1)
5. ![](https://latex.codecogs.com/svg.latex?P(\alpha\leq\xi\leq\beta)=F(\beta)-F(\alpha))
Для дискретной С.В. справедлива только при таких знаках. При Н.С.В. – знаки могут быть любые (<; <), (<; <=), (<=; <), (<=; <=)

_________
Пусть ξ – Д.С.В.
![](../images/Mathematical-statistics/ticket04-1.png)

**Многоугольник распределения**

![](https://latex.codecogs.com/svg.latex?k\leq&space;n)

| ![](https://latex.codecogs.com/svg.latex?x_{i})                     | ![](https://latex.codecogs.com/svg.latex?x_{1})     | ![](https://latex.codecogs.com/svg.latex?x_{2})     | ... | ![](https://latex.codecogs.com/svg.latex?x_{k})     |
|---------------------------------------------------------------------|-----------------------------------------------------|-----------------------------------------------------|-----|-----------------------------------------------------|
| ![](https://latex.codecogs.com/svg.latex?n_{i})                     | ![](https://latex.codecogs.com/svg.latex?n_{1})     | ![](https://latex.codecogs.com/svg.latex?n_{2})     | ... | ![](https://latex.codecogs.com/svg.latex?n_{k})     |
| ![](https://latex.codecogs.com/svg.latex?P_{i}^{*}=\frac{n_{i}}{n}) | ![](https://latex.codecogs.com/svg.latex?P_{1}^{*}) | ![](https://latex.codecogs.com/svg.latex?P_{2}^{*}) | ... | ![](https://latex.codecogs.com/svg.latex?P_{k}^{*}) |

**Полигон относительных частот** - статистический аналог многоугольника распределения 
_________

Пусть ξ – непрерывная С.В.

f(x) - плотность
Эмпирическая плотность/**гистограмма** - аналог плотности.

Для построения гистограммы, полученные данные нужно записать в виде информационно статистической таблицы.

| Разряды           | ![](https://latex.codecogs.com/svg.latex?[y_{1},y_{2}]) | ![](https://latex.codecogs.com/svg.latex?[y_{2},y_{3}]) | ... | ![](https://latex.codecogs.com/svg.latex?[y_{s},y_{s+1}]) |
|------------------|----------------|------------|-----|---------------|
| ![](https://latex.codecogs.com/svg.latex?L_{i})     | ![](https://latex.codecogs.com/svg.latex?L_{1})     | ![](https://latex.codecogs.com/svg.latex?L_{2})     | ... | ![](https://latex.codecogs.com/svg.latex?L_{s})        |
| ![](https://latex.codecogs.com/svg.latex?L_{i}^{*}=\frac{L_{i}}{n}) | ![](https://latex.codecogs.com/svg.latex?L_{1}^{*})   | ![](https://latex.codecogs.com/svg.latex?L_{2}^{*})   | ... | ![](https://latex.codecogs.com/svg.latex?L_{s}^{*})       |

Для каждого i-го разряда посчитаем ![](https://latex.codecogs.com/svg.latex?f_{i}^{*}=\frac{{l_{i}}}{n*\Delta&space;i})

![](https://latex.codecogs.com/svg.latex?\Delta&space;i=y_{i&plus;1}-y_{i}) - длинна i-го разряда

![](../images/Mathematical-statistics/ticket04-2.png)

Площадь этой фигуры = 1
# 5. Статистические аналоги для математического ожидания, дисперсии, начальных и центральных моментов. Формулы для их вычисления в зависимости от способа представления данных.

Статистические аналоги Mξ и Dξ - M\*ξ и D\*ξ.
Их формулы похожи на Mξ и Dξ Д.С.В.

![](https://latex.codecogs.com/svg.latex?M\xi=\sum_{i}^{n}x_{i}p_{i})

![](https://latex.codecogs.com/svg.latex?%5Csmall%20D%5Cxi%3DM%5C%7B%28%5Cxi-M%5Cxi%29%5E%7B2%7D%5C%7D%3D%5Csum_%7Bi%7D%5E%7Bn%7D%28x_%7Bi%7D-M%5Cxi%29%5E%7B2%7D*p_%7Bi%7D%3DM%28%5Cxi%29%5E%7B2%7D-%28M%5Cxi%29%5E%7B2%7D%3D%5Csum_%7Bi%7D%5E%7Bn%7Dx_%7Bi%7D%5E%7B2%7D*p_%7Bi%7D-%28M%5Cxi%29%5E%7B2%7D)

1. Данные представлены в виде простого или вариационного ряда
![](https://latex.codecogs.com/svg.latex?x_{1}),![](https://latex.codecogs.com/svg.latex?x_{2}),...,![](https://latex.codecogs.com/svg.latex?x_{n})

![](https://latex.codecogs.com/svg.latex?M\xi^{*}=\frac{1}{n}\sum_{i=1}^{n}x_{i})

![](https://latex.codecogs.com/svg.latex?D\xi^{*}=\frac{1}{n}\sum_{i=1}^{n}(x_{i}-M\xi^{*})^{2}=\frac{1}{n}\sum_{i=1}^{n}x_{i}^{2}-(M\xi&space;^{*})^{2})

2. Данные в виде статистического распределения в выборке
![](https://latex.codecogs.com/svg.latex?x_{1}),![](https://latex.codecogs.com/svg.latex?x_{2}),...,![](https://latex.codecogs.com/svg.latex?x_{n})

![](https://latex.codecogs.com/svg.latex?k\leq&space;n)

![](https://latex.codecogs.com/svg.latex?M\xi&space;^{*}=\frac{1}{n}\sum_{i=1}^{k}n_{i}*x_{i})

![](https://latex.codecogs.com/svg.latex?D\xi&space;^{*}=\frac{1}{n}\sum_{i=1}^{k}n_{i}*(x_{i}-M\xi&space;^{*})^{2}=\frac{1}{n}\sum_{i=1}^{k}n_{i}*x_{i}^{2}-(M\xi&space;^{*})^{2})

3. Данные в виде информационно-статистической таблицы

Используя эту таблицу строим таблицу следующего вида: для каждого разряда найдём его середину ![](https://latex.codecogs.com/svg.latex?\widetilde{y_{i}}=\frac{y_{i}&plus;y_{i&plus;1}}{2})

| ![](https://latex.codecogs.com/svg.latex?\widetilde{y_{i}}})      | ![](https://latex.codecogs.com/svg.latex?\widetilde{y_{1}})         | ![](https://latex.codecogs.com/svg.latex?\widetilde{y_{2}})    | ... | ![](https://latex.codecogs.com/svg.latex?\widetilde{y_{s}})             |
|-------------------------------|---------------------------|-------------------|-----|----------------------|
| ![](https://latex.codecogs.com/svg.latex?l_{i}^{*}=\frac{l_{i}}{n}) | ![](https://latex.codecogs.com/svg.latex?l_{1}^{*}) | ![](https://latex.codecogs.com/svg.latex?l_{2}^{*}) | ... | ![](https://latex.codecogs.com/svg.latex?l_{s}^{*}) |

![](https://latex.codecogs.com/svg.latex?\sum_{i}^{s}l_{i}^{*}=1)

![](https://latex.codecogs.com/svg.latex?\alpha_{k}^{*}\xi) - статистический **аналог начального момента** k-го порядка

![](https://latex.codecogs.com/svg.latex?\alpha_{k}^{*}\xi=\frac{1}{n}\sum_{i=1}^{n}x_{i}^{k})

![](https://latex.codecogs.com/svg.latex?\beta_{k}^{*}\xi) - статистический **аналог центрального момента** k-го порядка

![](https://latex.codecogs.com/svg.latex?\beta_{k}^{*}\xi=\frac{1}{n}\sum_{i=1}^{n}(x_{i}-\overline{x})^{k})

![](https://latex.codecogs.com/svg.latex?\overline{x}=\frac{1}{n}\sum_{i=1}^{n}x_{i})
# 6. Статистические оценки параметров. Требования несмещенности, состоятельности и эффективности в некотором множестве оценок. Понятие сходимости по вероятности случайной последовательности. Основные теоремы для проверки состоятельности оценок.

Пусть для случайной величины ξ признака генеральной совокупности, известна точность распределения до параметров

![](https://latex.codecogs.com/svg.latex?\xi\rightarrow(x;a_{1},a_{2},...,a_{m}),m\geq1)

С помощью методов математической статистики найти параметры нельзя. Можно только оценки для этих параметров.
Выберем из генеральной совокупности n элементов и получим n экземпляров

![](https://latex.codecogs.com/svg.latex?\xi_{1}),...,![](https://latex.codecogs.com/svg.latex?\xi_{n})

**Оценка** ![](https://latex.codecogs.com/svg.latex?a_{1}) - ![](https://latex.codecogs.com/svg.latex?\widetilde{a_{1}}=\varphi_{1}(\xi_{1},\xi_{2},...,\xi_{n}))

![](https://latex.codecogs.com/svg.latex?\widetilde{a_{2}}=\varphi_{2}(\xi_{1},\xi_{2},...,\xi_{n}))

...

![](https://latex.codecogs.com/svg.latex?\widetilde{a_{m}}=\varphi_{m}(\xi_{1},\xi_{2},...,\xi_{n}))

Все это статистические оценки для параметров. Функции от С.В. => они сами являются С.В.

### Требования к оценкам
1. **Понятие несмещенности оценки**

![](https://latex.codecogs.com/svg.latex?a\rightarrow\widetilde{a}=\varphi(\xi_{1},\xi_{2},...,\xi_{n}))

Если для любого n=1,2,..., ![](https://latex.codecogs.com/svg.latex?M(\widetilde{a})=a), то оценка называется **несмещенной**.

2. **Понятие состоятельности оценки**

Говорят, что последовательность ![](https://latex.codecogs.com/svg.latex?\xi_{1},\xi_{2},...,\xi_{n}) сходится по вероятности к неслучайной величине А, если при ![](https://latex.codecogs.com/svg.latex?n\rightarrow\infty), ![](https://latex.codecogs.com/svg.latex?\forall\varepsilon>0)

последовательность из вероятностей
![](https://latex.codecogs.com/svg.latex?P(|\xi_{1}-A|<\varepsilon),P(|\xi_{2}-A|<\varepsilon),...,P(|\xi_{n}-A|<\varepsilon)\rightarrow1)

![](https://latex.codecogs.com/svg.latex?\lim_{n\rightarrow\infty}P(|\xi_{n}-A|<\varepsilon)=1)

![](https://latex.codecogs.com/svg.latex?\xi_{n}\xrightarrow[n\rightarrow\infty]{P}A)

![](https://latex.codecogs.com/svg.latex?\widetilde{a_{n}}):

![](https://latex.codecogs.com/svg.latex?n=1\rightarrow\widetilde{a_{1}}=\varphi(\xi_{1}))

![](https://latex.codecogs.com/svg.latex?n=2\rightarrow\widetilde{a_{2}}=\varphi(\xi_{1},\xi_{2}))

При изменении n от 1 до бесконечности, возникает последовательность оценок ![](https://latex.codecogs.com/svg.latex?\widetilde{a_{1}},\widetilde{a_{2}},...,\widetilde{a_{n}})
Если эта последовательность сходится по вероятности к а
![](https://latex.codecogs.com/svg.latex?\widetilde{a_{n}}\xrightarrow[n\rightarrow\infty]{P}a)
, то построенная оценка называется **состоятельной**

___
На практике используются 3 **теоремы состоятельности**:

- **Теорема Чебышева**
![](https://latex.codecogs.com/svg.latex?\xi_{1},\xi_{2},...,\xi_{n}) - последовательность, имеющая одинаковые С.В.

![](https://latex.codecogs.com/svg.latex?M\xi_{i}=m,D\xi_{i}=d,&space;i=1,2,...,)

Образуем С.В. ![](https://latex.codecogs.com/svg.latex?\eta_{n}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})

Последовательность ![](https://latex.codecogs.com/svg.latex?\eta_{1},\eta_{2},...,\eta_{n}) сходиться при ![](https://latex.codecogs.com/svg.latex?n\rightarrow\infty) к m

![](https://latex.codecogs.com/svg.latex?\xrightarrow[n\rightarrow\infty]{P}m)

- Если оценка ![](https://latex.codecogs.com/svg.latex?\widetilde{a}) является состоятельной для параметра a, то для любой непрерывной функции g, оценка ![](https://latex.codecogs.com/svg.latex?g(\widetilde{a})) будет состоятельной для параметра g(a).

- Пусть ![](https://latex.codecogs.com/svg.latex?\widetilde{a}) является несмещенной оценкой для параметра a и ![](https://latex.codecogs.com/svg.latex?D(\widetilde{a})\underset{n\rightarrow\infty}{\rightarrow}0), тогда оценка ![](https://latex.codecogs.com/svg.latex?\widetilde{a}) будет состоятельной для параметра a.
___
3. Понятие **Эффективности** оценки в множестве оценок

Предположим, что для

![](https://latex.codecogs.com/svg.latex?a%20%5Crightarrow%20%5Cbegin%7Bmatrix%7D%20%5Cwidetilde%7Ba%7D%5E%7B%281%29%7D%5C%5C%20%5Cwidetilde%7Ba%7D%5E%7B%28n%29%7D%20%5C%5C%20...%5C%5C%20%5Cwidetilde%7Ba%7D%5E%7B%28m%29%7D%20%5Cend%7Bmatrix%7D)

существуют несмещенные оценки.

Из них нужно взять ту, у которой меньше Дисперсия ![](https://latex.codecogs.com/svg.latex?D\xi^{*}). Оценка называется **эффективной** на некотором множестве, если она имеет наименьшую Дисперсию ![](https://latex.codecogs.com/svg.latex?D\xi^{*}).
# 7. Оценка генеральной средней: свойства, формулы для вычисления.

Часто оцениваемым параметром является ![](https://latex.codecogs.com/svg.latex?M\xi)

![](https://latex.codecogs.com/svg.latex?\widetilde{M\xi}) - оценка

![](https://latex.codecogs.com/svg.latex?\widetilde{M\xi}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})

### Здесь на экзамене возможно нужно будет расписать и показать, что эта оценка хорошая (спросить на консультации)
# 8. Точность и надежность несмещенной оценки для математического ожидания. Три задачи и их решение.

![](https://latex.codecogs.com/svg.latex?\widetilde{M\xi}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})

Покажем, что эта оценка хороша

1. **Несмещенность**
![](https://latex.codecogs.com/svg.latex?M(\widetilde{M\xi})=M\xi) - выполняется

![](https://latex.codecogs.com/svg.latex?M(\frac{1}{n}\sum_{i=1}^{n}\xi_{i})=\frac{1}{n}(M\xi_{1}&plus;M\xi_{2}&plus;...&plus;M\xi_{n})=\frac{1}{n}*n*M\xi=M\xi)

2. **Состоятельность**

n = 1, 2, ...,

Получится последовательность оценок ![](https://latex.codecogs.com/svg.latex?\frac{1}{n}\sum_{i=1}^{n}\xi_{i}\xrightarrow[n\rightarrow\infty]{P}M\xi)

По Т. Чебышева.

Выполнены условия теоремы Чебышева из нее непосредственно следует это равенство.

3. **Эффективность**

Рассмотрим свойства асимптотической эффективности.

![](https://latex.codecogs.com/svg.latex?a\rightarrow\widetilde{a}=\varphi(\xi_{1},\xi_{2},...,\xi_{n}))

Если при ![](https://latex.codecogs.com/svg.latex?n\rightarrow\infty), ![](https://latex.codecogs.com/svg.latex?D(\widetilde{a_{n}})\rightarrow0), то оценка асимптотически эффективна.

4. **Точность и надежность**

![](https://latex.codecogs.com/svg.latex?P(|\widetilde{M\xi}-M\xi|<\varepsilon)=\gamma)

Где ![](https://latex.codecogs.com/svg.latex?\widetilde{M\xi}) - С.В.

![](https://latex.codecogs.com/svg.latex?M\xi) - Случайное событие

Можно показать что в этом случае Гамма вычисляется по формуле:

![](https://latex.codecogs.com/svg.latex?\gamma=\Phi(\frac{\varepsilon\sqrt{n}}{\sqrt{D\xi}}))

![](https://latex.codecogs.com/svg.latex?\Phi(x)=\frac{2}{\sqrt{2\pi}}*\int_{0}^{x}e^{-\frac{t^{2}}{2}}dt)

![](../images/Mathematical-statistics/ticket08.png)

* Для того чтобы увеличить гамму, из графика видно, что нужно увеличить аргумент X.
Если ε задана, Dξ = const, то существует единственный способ - увеличение n.
* В формуле стоит Dξ. На практике мы ее не знаем, следовательно заменяем ее оценкой Dξ.
* Полученное равенство можно рассматривать как некоторые уравнения связывающие ![](https://latex.codecogs.com/svg.latex?\gamma), ε и n.
___
### Три задачи
1. Знаем ε и n.
![](https://latex.codecogs.com/svg.latex?\gamma) = ?

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n}}{\sqrt{D\xi}}=x_{0})

| x      | ![](https://latex.codecogs.com/svg.latex?\Phi(x)) |
|--------------|------------|
| ![](https://latex.codecogs.com/svg.latex?x_{0}\rightarrow) | ![](https://latex.codecogs.com/svg.latex?\gamma) |

2. Знаем ![](https://latex.codecogs.com/svg.latex?\gamma) и n.
ε = ?

| x   | ![](https://latex.codecogs.com/svg.latex?\Phi(x))           |
|----------|----------|
| ![](https://latex.codecogs.com/svg.latex?t_{\gamma}) | ![](https://latex.codecogs.com/svg.latex?\leftarrow\gamma) |

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n}}{\sqrt{D\xi}}=t_{\gamma}\rightarrow\varepsilon)

3. Знаем ![](https://latex.codecogs.com/svg.latex?\gamma) и ε.
n = ?

| x   | ![](https://latex.codecogs.com/svg.latex?\Phi(x))           |
|----------|----------|
| ![](https://latex.codecogs.com/svg.latex?t_{\gamma}) | ![](https://latex.codecogs.com/svg.latex?\leftarrow\gamma) |

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n}}{\sqrt{D\xi}}=t_{\gamma}\rightarrow\sqrt{n}=\frac{t_{\gamma}\sqrt{D\xi}}{\varepsilon}=\frac{t_{\gamma}^{2}*D\xi}{\varepsilon^{2}})
# 9. Смещенная и несмещенная оценки для генеральной дисперсии: свойства, формулы для вычисления.

Dξ - **генеральная дисперсия**.

Строим оценку.

1. ![](https://latex.codecogs.com/svg.latex?M\xi=a) - известно

Тогда ![](https://latex.codecogs.com/svg.latex?\widetilde{D\xi}=\frac{1}{n}\sum_{i=1}^{n}(\xi_{i}-a)^{2})

- Покажем, что оценка **несмещенная**

![](https://latex.codecogs.com/svg.latex?M(\widetilde{D\xi})=\frac{1}{n}((\xi_{1}-a)^{2}&plus;(\xi_{2}-a)^{2}&plus;...&plus;(\xi_{n}-a)^{2})=\frac{1}{n}*n*D\xi=D\xi)

- ![](https://latex.codecogs.com/svg.latex?D(\widetilde{D\xi})\underset{n\rightarrow\infty}{\rightarrow}0) - **асимптотически эффективна**

- **Состоятельность**

Из a, b и Теоремы #3 - оценка состоятельна
___
##### Теорема #3
Пусть ![](https://latex.codecogs.com/svg.latex?\widetilde{a}) является состоятельной для параметра a и ![](https://latex.codecogs.com/svg.latex?D(\widetilde{a})\underset{n\rightarrow\infty}{\rightarrow}0), тогда оценка ![](https://latex.codecogs.com/svg.latex?\widetilde{a}) будет состоятельной для параметра a.
___
2. Mξ - неизвестно

Предложим оценку

![](https://latex.codecogs.com/svg.latex?\widetilde{D\xi}=\frac{1}{n}\sum_{i=1}^{n}(\xi_{i}-\widetilde{M\xi})^{2})

Где ![](https://latex.codecogs.com/svg.latex?\widetilde{M\xi}=\frac{1}{n}\sum\xi_{i})

Проверим ее несмещенность

![](https://latex.codecogs.com/svg.latex?M(\widetilde{D\xi})=\frac{1}{n}\sum_{i=1}^{n}(\xi_{i}-\widetilde{M\xi})^{2}=...=\frac{n-1}{n}D\xi\neq&space;D\xi) - не будет несмещенной => не подходит.

Исправим ![](https://latex.codecogs.com/svg.latex?\widetilde{D\xi})

![](https://latex.codecogs.com/svg.latex?\widetilde{D\xi}_{changed}=\widetilde{D\xi}*\frac{n}{n-1}=\frac{1}{n-1}\sum_{i=1}^{n}(\xi_{i}-\widetilde{M\xi})^{2}) - несмещенная, состоятельная, асимптотически эффективная

![](https://latex.codecogs.com/svg.latex?\frac{1}{n}\approx\frac{1}{n-1})
# 10. Точность и надежность несмещенной оценки для дисперсии. Три задачи и их решение.

Для точного нахождения гамма, нужно знать Dξ и четвёртый центральный момент.

Используем приближенную формулу для нахождения гамма.

![](https://latex.codecogs.com/svg.latex?\gamma=P(|\widetilde{D\xi}_{changed}-D\xi|<\varepsilon)=\Phi(\frac{\varepsilon\sqrt{n-1}}{\sqrt{2}D\xi}))

Точная формула, если ξ распределена по нормальному закону.

В этой формуле мы не знаем Dξ, поэтому заменяем ее несмещенной оценкой.

С помощью этого уравнения решаются те же самые 3 задачи.

### Три задачи
1. Знаем ε и n.

![](https://latex.codecogs.com/svg.latex?\gamma) = ?

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n-1}}{\sqrt{2}D\xi}=x_{0})

| x      | ![](https://latex.codecogs.com/svg.latex?\Phi(x)) |
|--------------|------------|
| ![](https://latex.codecogs.com/svg.latex?x_{0}\rightarrow) | ![](https://latex.codecogs.com/svg.latex?\gamma) |

2. Знаем ![](https://latex.codecogs.com/svg.latex?\gamma) и n.

ε = ?

| x   | ![](https://latex.codecogs.com/svg.latex?\Phi(x))           |
|----------|----------|
| ![](https://latex.codecogs.com/svg.latex?t_{\gamma}) | ![](https://latex.codecogs.com/svg.latex?\leftarrow\gamma) |

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n-1}}{\sqrt{2}D\xi}=t_{\gamma}\rightarrow\varepsilon)

3. Знаем ![](https://latex.codecogs.com/svg.latex?\gamma) и ε.

n = ?

| x   | ![](https://latex.codecogs.com/svg.latex?\Phi(x))           |
|----------|----------|
| ![](https://latex.codecogs.com/svg.latex?t_{\gamma}) | ![](https://latex.codecogs.com/svg.latex?\leftarrow\gamma) |

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n-1}}{\sqrt{2}D\xi}=t_{\gamma}\rightarrow\sqrt{n-1}=\frac{t_{\gamma}*D\xi*\sqrt{2}}{\varepsilon}=\frac{t_{\gamma}^{2}*D\xi^{2}*2}{\varepsilon^{2}})

___
### Нахождение
![](https://latex.codecogs.com/svg.latex?\overline{x}=\frac{1}{n}\sum_{i=1}^{n}x_{i})

![](https://latex.codecogs.com/svg.latex?D\xi_{changed}=\frac{1}{n-1}\sum_{i=1}^{n}(x_{i}-\overline{x})^{2})

По этим формулам найдем смещенную оценку ![](https://latex.codecogs.com/svg.latex?D\xi_{*}).

![](https://latex.codecogs.com/svg.latex?D\xi_{changed}=\frac{n}{n-1}D\xi_{*})
# 11. Оценка для вероятности: ее свойства, точность и надежность.

Пусть имеется случайный эксперимент

![](https://latex.codecogs.com/svg.latex?P=P(A)=?)

Задача: требуется построить оценку

![](https://latex.codecogs.com/svg.latex?\tilde{P}=\tilde{P}(A))

Проведем эксперимент 1ый раз. Пусть с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) - число появлений события А в первом опыте

Проведем 2ой раз.  с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) - число появлений события А во втором опыте. Имеет тоже самое распределение как ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1})

и т.д.
Проведем n-ый раз, получим ![](https://latex.codecogs.com/svg.latex?\xi&space;_{n}). Она имеет тоже самое распределение (Бернулливская св???)

Посчитаем их сумму

![](https://latex.codecogs.com/svg.latex?\xi=\sum_{i=1}^{n}\xi_{i}) - общее количество наступления события А

![](https://latex.codecogs.com/svg.latex?\frac{1}{n}\sum_{i=1}^{n}\xi_{i}) - относительная частота наступления события А

![](https://latex.codecogs.com/svg.latex?\tilde{P}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})


### Покажем, что эта оценка удовлетворяла всем требованиям, чтобы она была "хорошей"

![](https://latex.codecogs.com/svg.latex?M_{\xi_{i}}&space;=&space;p)

![](https://latex.codecogs.com/svg.latex?D_{\xi_{i}}&space;=&space;p^{2}&space;-&space;p&space;=&space;p(1-p)=&space;pq)

#### 1. Несмещенность
![](https://latex.codecogs.com/svg.latex?M(\tilde{P})=\frac{1}{n}(M_{\xi&space;_{1}}&plus;&space;M_{\xi&space;_{2}}&space;&plus;&space;...&space;&plus;&space;M_{\xi&space;_{n}})&space;=&space;\frac{1}{n}&space;\cdot&space;np&space;=&space;p)
#### 2. Асимптотическая эффективность
![](https://latex.codecogs.com/svg.latex?D(\tilde{P})=\frac{1}{n^{2}}(D_{\xi&space;_{1}}&plus;&space;D_{\xi&space;_{2}}&space;&plus;&space;...&space;&plus;&space;D_{\xi&space;_{n}})&space;=&space;\frac{1}{n^{2}}&space;\cdot&space;npq&space;=&space;\frac{pq}{n})

![](https://latex.codecogs.com/svg.latex?\lim_{n&space;\to&space;\propto&space;}&space;(\frac{pq}{n})&space;=&space;0)

#### 3. Состоятельность
Из 1, 2 по теореме 3 следует состоятельность

#### 4. 
![](https://latex.codecogs.com/svg.latex?\gamma&space;=&space;P(\left&space;|&space;\tilde{P}&space;-&space;P&space;\right&space;|&space;<&space;\varepsilon&space;)&space;=&space;...&space;=&space;\Phi&space;(\frac{\varepsilon&space;\sqrt{n}}{\sqrt{pq}}))

p, q - мы не знаем. p, q мы заменяем оценками.

Предположим, что опыт провели n раз и n раз наблюдали событие А. Тогда относительная частота будет

![](https://latex.codecogs.com/svg.latex?\tilde{p}=\tfrac{m}{n})

![](https://latex.codecogs.com/svg.latex?\tilde{q}=1&space;-&space;\tfrac{m}{n})

![](https://latex.codecogs.com/svg.latex?\approx&space;\Phi&space;(\frac{\varepsilon&space;\sqrt{n}}{\sqrt{\tfrac{m}{n}(1-\frac{m}{n}))}}))

Мы можем решить те же 3 задачки, рассматриваемые ранее 
Задача: ![](https://latex.codecogs.com/svg.latex?\gamma&space;,&space;\varepsilon) - известны, нужно найти n. 

![](https://latex.codecogs.com/svg.latex?\gamma=0,95), то ![](https://latex.codecogs.com/svg.latex?n\approx&space;\frac{1}{\varepsilon&space;^{2}})
# 12. Метод моментов для построения оценок неизвестных параметров распределения.

#### Теоретические моменты

![](https://latex.codecogs.com/svg.latex?%5Calpha_%7Bk%7D%5Cxi%3DM%28%5Cxi%5E%7Bk%7D%29%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%5Csum_%7Bi%7Dx_%7Bi%7D%5E%7Bk%7Dp%28%5Cxi%3Dx_%7Bi%7D%2Ca_%7B1%7D%2Ca_%7B2%7D%2C...%2Ca_%7Bn%7D%2Cesly%5Cxi-d.s.v.%29%5C%5C%5Cint_%7B-%5Cpropto%7D%5E%7B&plus;%5Cpropto%7Dx%5E%7Bk%7Df_%7B%5Cxi%7D%28x%2Ca_%7B1%7D%2Ca_%7B2%7D%2C...%2Ca_%7Bn%7D%2Cesly%5Cxi-n.s.v.%29%5Cend%7Bmatrix%7D%5Cright.)


![](https://latex.codecogs.com/svg.latex?%5Cbeta_%7Bk%7D%5Cxi%3DM%28%5Cxi-M_%7B%5Cxi%7D%29%5E%7Bk%7D%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%5Csum_%7Bi%7D%28x_%7Bi%7D-M_%7B%5Cxi%7D%29%5E%7Bk%7Dp%28%5Cxi%3Dx_%7Bi%7D%2Ca_%7B1%7D%2Ca_%7B2%7D%2C...%2Ca_%7Bn%7D%2Cesly%5Cxi-d.s.v.%29%5C%5C%5Cint_%7B-%5Cpropto%7D%5E%7B&plus;%5Cpropto%7D%28x-M_%7B%5Cxi%7D%29%5E%7Bk%7Df_%7B%5Cxi%7D%28x%2Ca_%7B1%7D%2Ca_%7B2%7D%2C...%2Ca_%7Bn%7D%2Cesly%5Cxi-n.s.v.%29%5Cend%7Bmatrix%7D%5Cright.) 


Записывают так:

![](https://latex.codecogs.com/svg.latex?\alpha&space;_{k}\xi(a_{1},a_{2},...,a_{m}),&space;\beta&space;_{k}\xi(a_{1},a_{2},...,a_{m}))

#### Статистические моменты

![](https://latex.codecogs.com/svg.latex?\alpha&space;_{k}^{*}=\frac{1}{n}\sum_{i=1}^{n}x_{i}^{k}) - **начальный момент n-го порядка**

![](https://latex.codecogs.com/svg.latex?\beta&space;_{k}^{*}=\frac{1}{n}\sum_{i=1}^{n}(x_{i}-\bar{x})^{k};\bar{x}=\frac{1}{n}\sum_{i=1}^{n}x_{i})

### Метод моментов

Если неизвестных параметров М, то нужно найти М любых теоретических моментов, а затем по выборке ![](https://latex.codecogs.com/svg.latex?x_{1},&space;x_{2},..,&space;x_{m}) посчитать соответствующие им статистические моменты.

Далее их нужно приравнять. Получим систему из М уравнений с М неизвестными. 

Ее нужно решить относительно ![](https://latex.codecogs.com/svg.latex?a_{1},&space;a_{2},..,&space;a_{m})

Возможно несколько случаев:

1. Решение единственно 

![](https://latex.codecogs.com/svg.latex?\tilde{a}_{1},&space;\tilde{a}_{2},..,&space;\tilde{a}_{m})

![](https://latex.codecogs.com/svg.latex?\tilde{a}_{1}=a_{1}^{*},&space;\tilde{a}_{2}=a_{2}^{*},..,&space;\tilde{a}_{m}=a_{m}^{*})

Утверждается, что эти оценки будут состоятельными, решение единственно

2. Решений несколько

Тогда в качестве оценок можем взять любое из них. Но в этом случае ничего о состоятельности сказать нельзя.

3. Система не имеет решений.

Говорим, что решений по методу оценок не существует.
При решении задач рекомендуется брать простые моменты
# 13. Метод максимального правдоподобия для построения оценок. (или "Максимума") 

#### Суть: 
Строится так называемая **функция правдоподобия**, которая зависит от некоторых параметров
![](https://latex.codecogs.com/svg.latex?a_{1},a_{2},...,a_{m})

Далее у этой функции находятся такие параметры ![](https://latex.codecogs.com/svg.latex?a_{1}^{*},a_{2}^{*},...,a_{m}^{*}) , которые обеспечивают максимум и эти значения берутся в качестве оценок максимального правдоподобия

Пусть
1) ![](https://latex.codecogs.com/svg.latex?\xi&space;-&space;d.s.v,&space;P(\xi&space;=&space;x;&space;a_{1},&space;a_{2},&space;...,&space;a_{m}))

получим выборку ![](https://latex.codecogs.com/svg.latex?x_{1},x_{2},...x_{n})

![](https://latex.codecogs.com/svg.latex?%5Cbegin%7Bmatrix%7DP%28%5Cxi%3Dx_%7B1%7D%3B%20a_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5C%5C%20P%28%5Cxi%3Dx_%7B2%7D%3B%20a_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5C%5C%20%5Ccdot%20%5C%5C%20%5Ccdot%20%5C%5C%20%5Ccdot%20%5C%5C%20P%28%5Cxi%3Dx_%7Bn%7D%3B%20a_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5Cend%7Bmatrix%7D)

![](https://latex.codecogs.com/svg.latex?L_{x_{1},&space;x_{2},...,x_{n}}(a_{1},a_{2},..,a_{m})=\prod_{i=1}^{n}p(\xi=x_{i},&space;a_{1},a_{2},..,a_{m}))

2) ![](https://latex.codecogs.com/svg.latex?\xi-n.s.v,f_{\xi}(x;a_{1},a_{2},...,a_{m}))

получим выборку ![](https://latex.codecogs.com/svg.latex?x_{1},x_{2},...x_{n})

Считаем эту плотность для полученных значений
![](https://latex.codecogs.com/svg.latex?L_{x_{1},x_{2},...,x_{n}}(a_{1},a_{2},..,a_{m})=\prod_{i=1}^{n}f_{\xi}(x_{i},a_{1},a_{2},..,a_{m}))

![](https://latex.codecogs.com/svg.latex?%5Cbegin%7Bmatrix%7D%20f_%7B%5Cxi%7D%28x_%7B1%7D%3Ba_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5C%5C%20f_%7B%5Cxi%7D%28x_%7B2%7D%3Ba_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5C%5C%20%5Ccdot%20%5C%5C%20%5Ccdot%20%5C%5C%20%5Ccdot%20%5C%5C%20f_%7B%5Cxi%7D%28x_%7Bn%7D%3Ba_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5Cend%7Bmatrix%7D)

Часто в практических задачах L- дифференцируема по параметрам ![](https://latex.codecogs.com/svg.latex?a_{1},a_{2},...a_{m})

Тогда для нахождения критических точек используют:

![](https://latex.codecogs.com/svg.latex?%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%5Cfrac%7B%5Cpartial%20L%28a_%7B1%7D%2Ca_%7B2%7D%2C..%2Ca_%7Bn%7D%29%7D%7B%5Cpartial%20a_%7Bj%7D%7D%20%3D%200%20%5C%5C%20j%20%3D%20%5Coverline%7B1%2C%20m%7D%20%5Cend%7Bmatrix%7D%5Cright.)

Есть свойство, если f(x)>0 и Lnf(x) - имеют одни и те же точки экстремума.

Рекомендуется находить точки экстремума не самой функции L, а у Ln(L) - это проще

Обычно находят так :

![](https://latex.codecogs.com/svg.latex?%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%5Cfrac%7B%5Cpartial%20ln%20%28L%28a_%7B1%7D%2Ca_%7B2%7D%2C..%2Ca_%7Bn%7D%29%29%7D%7B%5Cpartial%20a_%7Bj%7D%7D%20%3D%200%20%5C%5C%20j%20%3D%20%5Coverline%7B1%2C%20m%7D%20%5Cend%7Bmatrix%7D%5Cright.)
# 14. Точечные и интервальные оценки. Доверительные интервалы.

Оценки, которые задаются одним числом называться **точечными**. Если объем выборки n большой, то оценки дают достаточно хорошие результаты. 


Если n маленькое, то надежность этих оценок ![](https://latex.codecogs.com/svg.latex?\gamma) является маленькой.

Увеличить надежность можно только увеличив объем выборки. Но существует множество задач, в которых новые измерения дорогостоящие. В этом случае вместо точечных оценок строят **интервальные оценки**.

Вместо одного числа предлагают целый интервал.
параметр ![](https://latex.codecogs.com/svg.latex?a\rightarrow&space;\tilde{a}) точечная оценка

![](https://latex.codecogs.com/svg.latex?\gamma&space;=&space;p(\left&space;|&space;\tilde{a}&space;-&space;a\right&space;|<\varepsilon&space;)), где ![](https://latex.codecogs.com/svg.latex?\varepsilon) - **точечная оценка**

Если ![](https://latex.codecogs.com/svg.latex?\varepsilon&space;\rightarrow&space;0,&space;\gamma&space;\rightarrow&space;1) - это хорошо.

![](https://latex.codecogs.com/svg.latex?\tilde{a}-\varepsilon&space;<&space;a&space;<&space;\tilde{a}&plus;\varepsilon&space;;&space;\tilde{a}-\varepsilon&space;=\tilde{a_{1}};\tilde{a}&plus;\varepsilon&space;=\tilde{a_{2}}) (1)

![](https://latex.codecogs.com/svg.latex?(\tilde{a_{1}},\tilde{a_{2}})) - **доверительный интервал**, который покрывает неизвестный параметр а с данной надежностью ![](https://latex.codecogs.com/svg.latex?\gamma)

Увеличиваем надежность, тогда теряем точность (интервал)

Доверительный интервал - интервальная оценка.

Заметим, из (1) полученный интервал всегда является симметричным относительно оценки.

Задача сводится к нахождению ![](https://latex.codecogs.com/svg.latex?\varepsilon)

![](https://latex.codecogs.com/svg.latex?\gamma) - Дано. То есть мы подгоняем интервал под надежность
# 15. Построение доверительных интервалов для неизвестного математического ожидания нормального распределения при известной дисперсии.

#### Построение доверительных интервалов для неизвестного параметра а нормального распределения при известном параметре ![](https://latex.codecogs.com/svg.latex?\sigma)

![](https://latex.codecogs.com/svg.latex?f_{\varepsilon&space;}(x)=\frac{1}{\sqrt{2\pi&space;}\sigma&space;}&space;\cdot&space;e^{\frac{-(x-a)^2}{\sigma&space;^{2}}})

![](https://latex.codecogs.com/svg.latex?\sigma) - известная

требуется построить доверительный интервал ![](https://latex.codecogs.com/svg.latex?(\tilde{a_{1}},\tilde{a_{2}})), покрывающий неизвестный параметр a с заданной надежностью ![](https://latex.codecogs.com/svg.latex?\gamma) по выборочным значениям ![](https://latex.codecogs.com/svg.latex?x_{1},x_{2},...,x_{n})

Имеем:

![](https://latex.codecogs.com/svg.latex?a=M_{\xi&space;})

![](https://latex.codecogs.com/svg.latex?\tilde{a}=\tilde{M_{\xi&space;}}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})

Тогда ![](https://latex.codecogs.com/svg.latex?\gamma&space;=&space;p(\left&space;|&space;\tilde{a}-a&space;\right&space;|<\varepsilon&space;)=p(\left&space;|&space;\tilde{M_{\xi&space;}}&space;-&space;M_{\xi}\right&space;|<\varepsilon&space;)=...=\Phi&space;(\frac{\varepsilon&space;\sqrt{n}}{\sqrt{D_{\xi&space;}}})=\Phi&space;(\frac{\varepsilon&space;\sqrt{n}}{\sigma&space;}))

![](https://latex.codecogs.com/svg.latex?\gamma&space;=&space;\Phi&space;(\frac{\varepsilon&space;\sqrt{n}}{\sigma&space;})&space;\rightarrow&space;\varepsilon&space;-&space;?)

По функции Лапласа по ![](https://latex.codecogs.com/svg.latex?\phi&space;(x)) получаем x ( по ![](https://latex.codecogs.com/svg.latex?\gamma) получаем ![](https://latex.codecogs.com/svg.latex?t_{\gamma&space;}))

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon&space;\sqrt{n}}{\sigma&space;}&space;=&space;t_{\gamma&space;}\Rightarrow&space;\varepsilon&space;=&space;\frac{t_{\gamma&space;}\cdot&space;\sigma&space;}{\sqrt{n}})

Раскрываем модуль:

![](https://latex.codecogs.com/svg.latex?\tilde{a}-\varepsilon&space;<&space;a&space;<&space;\tilde{a}&plus;\varepsilon&space;;&space;\tilde{a}-\varepsilon&space;=\tilde{a_{1}};\tilde{a}&plus;\varepsilon&space;=\tilde{a_{2}})

Подставляем:

![](https://latex.codecogs.com/svg.latex?\frac{1}{n}\sum_{i=1}^{n}\xi_{i}-&space;\frac{t_{\gamma&space;}\cdot&space;\sigma&space;}{\sqrt{n}}<a<\frac{1}{n}\sum_{i=1}^{n}\xi_{i}&plus;&space;\frac{t_{\gamma&space;}\cdot&space;\sigma&space;}{\sqrt{n}})

Пусть задана выборка (конкретные числа): ![](https://latex.codecogs.com/svg.latex?x_{1},x_{2},..,x_{n})

Нужно посчитать их среднее арифметическое 

![](https://latex.codecogs.com/svg.latex?\bar{x}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})

И подставим так:

![](https://latex.codecogs.com/svg.latex?\bar{x}-&space;\frac{t_{\gamma&space;}\cdot&space;\sigma&space;}{\sqrt{n}}<a<\bar{x}&plus;&space;\frac{t_{\gamma&space;}\cdot&space;\sigma&space;}{\sqrt{n}})

### Замечание:
Полученную формулу для доверительного интервала можно использовать для любого параметра
# 16. Статистические гипотезы. Основные определения: нулевая, альтернативная, простая и сложная. Критерий согласия, критическая область.

**Статистической гипотезой** называется предположение о законе распределения или о параметре распределения случайной величины ![](https://latex.codecogs.com/svg.latex?\xi)

**Нулевая гипотеза** ![](https://latex.codecogs.com/svg.latex?H_{0}) - основное выдвинутое предположение

![](https://latex.codecogs.com/svg.latex?H_{1}) - **альтернативная или конкурирующая гипотеза** (предположение, противоречащее ![](https://latex.codecogs.com/svg.latex?H_{0}) )

Гипотеза называется **простой**, если она точно формулирует, и законы распределения, и все его параметры.
В противном случае называется **ложной** 

Для проверки гипотез выбирается **критерий согласия** - случайная величина, которая определяет правила проверки и закон распределения, который не зависит от гипотезы, которую мы выдвигаем

![](https://latex.codecogs.com/svg.latex?W_{0}) - **критической областью** называется множество значений этой случайной величины, при которой эта гипотеза отвергается.

#### Правило проверки.

Для проверки получаем независимую выборку ![](https://latex.codecogs.com/svg.latex?x_{1},&space;x_{2},..,x_{n}) По этим полученным данным получаем значение критерия согласия
Более подробно в следующем билете
# 17. Правило проверки гипотезы. Ошибки первого и второго рода. Уровень значимости и мощность критерия.

#### Правило проверки.
Для проверки получаем независимую выборку ![](https://latex.codecogs.com/svg.latex?x_{1},&space;x_{2},..,x_{n}) По этим полученным данным получаем значение критерия согласия

Если это значение попало в критическую область ![](https://latex.codecogs.com/svg.latex?W_{0}), то гипотезу ![](https://latex.codecogs.com/svg.latex?H_{0}) отвергаем и принимаем  ![](https://latex.codecogs.com/svg.latex?H_{1}).

Если значение критерия не попало в критическую область, то принимаем

При проверки гипотез можно сделать ошибки двух видов:

1. **Ошибка первого рода**.

Будет отвергнута ![](https://latex.codecogs.com/svg.latex?H_{0}) при условии, что она верна.
Вероятность этой ошибки называется **уровнем значимости критерия** ![](https://latex.codecogs.com/svg.latex?\alpha) - всегда задается постановщиком задачи (обычно 0,05 0,1)

2. **Ошибка второго рода**.

Будет принята ![](https://latex.codecogs.com/svg.latex?H_{0}) при условии, что верна ![](https://latex.codecogs.com/svg.latex?H_{1}) . Вероятность этой ошибки ![](https://latex.codecogs.com/svg.latex?\beta) - **оперативная характеристика критерия** по отношению к ![](https://latex.codecogs.com/svg.latex?H_{1}) . Обычно рассматривается ![](https://latex.codecogs.com/svg.latex?(1-\beta)) - вероятность принять ![](https://latex.codecogs.com/svg.latex?H_{0}) при условии, что она верна

Обычно рассматривается ![](https://latex.codecogs.com/svg.latex?(1-\beta)) - **мощность критерия** (вероятность правильного решения)

#### Основная задача проверки гипотез
Сконструировать такой критерий согласия, который бы при заданном уровне ![](https://latex.codecogs.com/svg.latex?\alpha) обеспечивал бы большую мощность
# 18. Критерий согласия Пирсона для дискретных случайных величин.

### Проверка гипотезы о законе распределения при помощи критерия ![](https://latex.codecogs.com/svg.latex?\chi_{cr}^{2})("Хи-квадрат") Пирсона (Согласия Пирсона)

Пусть гипотеза ![](https://latex.codecogs.com/svg.latex?H_{0}): случайная величина ![](https://latex.codecogs.com/svg.latex?\xi) имеет функция распределения ![](https://latex.codecogs.com/svg.latex?F_{\xi}(x)=) - формула (не важно какая)

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

**Мера расхождения** между ними:

![](https://latex.codecogs.com/svg.latex?R=\sum_{i=1}^{k}C_{i}(p_{i}^{*}-p_{i})^2)

![](https://latex.codecogs.com/svg.latex?C_{i}) - **веса, константы**

Пирсон предложил в качестве ![](https://latex.codecogs.com/svg.latex?C_{i}) взять величину ![](https://latex.codecogs.com/svg.latex?\frac{n}{p_{i}})

![](https://latex.codecogs.com/svg.latex?R=\sum_{i=1}^{k}\frac{n}{p_{i}}\cdot&space;C_{i}(p_{i}^{*}-p_{i})^2&space;=&space;...&space;=\sum_{i=1}^{k}\frac{(n_{i}-np_{i})^2}{np_{i}})

В этой формуле ![](https://latex.codecogs.com/svg.latex?n_{1},&space;n_{2},&space;...,&space;n_{k}) есть случайные величины

Тогда R - это случайная величина

Пирсон доказал, что данная случайная величина при достаточно больших значений n не зависит
от функции ![](https://latex.codecogs.com/svg.latex?F_{\xi&space;}(x)) и имеет распределение ![](https://latex.codecogs.com/svg.latex?\chi_{cr}^{2})

Пусть случайные величины ![](https://latex.codecogs.com/svg.latex?\xi_{1},&space;\xi_{2},&space;...,&space;\xi_{r}) являются независимыми и все они имеют стандартное нормальное распределение

![](https://latex.codecogs.com/svg.latex?\chi_{r}^{2}&space;=&space;\sum_{i=1}^{r}\xi&space;^{2}_{i})

(2 - это не квадрат, а обозначение)

Параметр r - называют **число степеней свобод**

Для нее составлено много разных таблиц, которыми мы можем пользоваться. Для использования этого критерия нужно найти число степеней свободы r

Если в гипотезе ![](https://latex.codecogs.com/svg.latex?H_{0}) указаны все параметры распределения точно, то число степеней свободы r вычисляется по формуле ![](https://latex.codecogs.com/svg.latex?r=k-1 ) 

Если в гипотезе ![](https://latex.codecogs.com/svg.latex?H_{0}) не все параметры указаны точно и S параметр приходится считать по выборке ![](https://latex.codecogs.com/svg.latex?r=k-1-S ) 

#### Правила применения критерия ![](https://latex.codecogs.com/svg.latex?\chi_{cr}^{2}) на практике

1. По полученным данным, где в таблице конкретные числа нужно вычислить R наблюдаемое

![](https://latex.codecogs.com/svg.latex?R=\sum_{i=1}^{k}\frac{(n_{i}-np_{i})^2}{np_{i}})

(это будет число, а не св)

2. Высчитываем r=k-1-S

3. Далее есть 2 пути (в зависимости от таблиц)

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
# 19. Критерий согласия Пирсона для непрерывных случайных величин.

### Проверка гипотезы о законе распределения при помощи критерия ![](https://latex.codecogs.com/svg.latex?\chi_{cr}^{2})("Хи-квадрат") Пирсона (Согласия Пирсона)

Пусть гипотеза ![](https://latex.codecogs.com/svg.latex?H_{0}): случайная величина ![](https://latex.codecogs.com/svg.latex?\xi) имеет функция распределения ![](https://latex.codecogs.com/svg.latex?F_{\xi}(x)=) - формула(не важно какая)

Гипотеза ![](https://latex.codecogs.com/svg.latex?H_{1}): функция распределения - другая формула

Требуется проверить ![](https://latex.codecogs.com/svg.latex?H_{0}) с заданным уровнем значимости 
![](https://latex.codecogs.com/svg.latex?\alpha)

2) Рассмотрим случай, когда ![](https://latex.codecogs.com/svg.latex?\xi) - непрерывная случайная величина. (первый случай в предыдущем билете)

Получим n значений этой случайной величины ![](https://latex.codecogs.com/svg.latex?x_{1},x_{2},...,x_{n}). Т.к. ![](https://latex.codecogs.com/svg.latex?\xi) - непрерывная, то вообще говоря одинаковых среди них быть не должно. Для того, чтобы применить критерий нужно обязательно построить группированный ряд:

| ![](https://latex.codecogs.com/svg.latex?(y_{i};y_{i&plus;1}))  | ![](https://latex.codecogs.com/svg.latex?[y_{1};y_{2}))  |  ![](https://latex.codecogs.com/svg.latex?[y_{2};y_{3})) | ...  |  ![](https://latex.codecogs.com/svg.latex?(y_{k};y_{k&plus;1})) |
|---|---|---|---|---|
| ![](https://latex.codecogs.com/svg.latex?l_{i})  |  ![](https://latex.codecogs.com/svg.latex?l_{1}) | ![](https://latex.codecogs.com/svg.latex?l_{2})  | ...  |  ![](https://latex.codecogs.com/svg.latex?l_{k}) |

![](https://latex.codecogs.com/svg.latex?l_{i}) - число точек, попавших в разряд

![](https://latex.codecogs.com/svg.latex?\sum_{i=1}^{k}l_{i}=n)

На практике берем 3-4 разряда

В этом случае взяли k разрядов

Рассмотрим случайную величину ![](https://latex.codecogs.com/svg.latex?R=\sum_{i=1}^{k}\frac{(l_{i}-np_{i})^2}{np_{i}})

Используя данные нашей таблички подставим ![](https://latex.codecogs.com/svg.latex?l_{i})  и вычислим R наблюдаемое. Где k - число разрядов, которые мы выбрали сами.

n - число выборки

![](https://latex.codecogs.com/svg.latex?p_{i})  - вероятность, что ![](https://latex.codecogs.com/svg.latex?\xi_{i}) (??) попадет в i-ый разряд

![](https://latex.codecogs.com/svg.latex?P_%7Bi%7D%3DP%20%5Cleft%20%28%20%5Cxi%20%5Cin%20%5By_%7Bi%7D%2Cy_%7Bi&plus;1%7D%29%20%5Cright%20%29%3DF_%7B%5Cxi%7D%28y_%7Bi&plus;1%7D%29-F_%7B%5Cxi%7D%28y_%7Bi%7D%29)

Вычисляется согласно гипотезе ![](https://latex.codecogs.com/svg.latex?H_{0})

r - число степеней свобод - считается также как и с д.с.в.

Остальное считается также как и с д.с.в.
