# 1. Свойства матрицы распределения вероятностей для дискретной двумерной с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) и с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) по матрице распределения.

![](https://latex.codecogs.com/svg.latex?(\xi_{1},&space;\xi_{2})) - двумерная случайная величина.

Для того, чтобы задать двумерную дискретную случайную величину, нужно задать все ее пары, а также все вероятности ![](https://latex.codecogs.com/svg.latex?P_{ij}). Тогда говорят, что задан __Закон распределения вероятностей двумерной с.в.__

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
