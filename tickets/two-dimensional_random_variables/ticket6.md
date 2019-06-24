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
