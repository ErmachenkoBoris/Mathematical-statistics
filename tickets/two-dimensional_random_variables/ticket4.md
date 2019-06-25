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

![](../../images/two-dimensional_random_variables/ticket4-1.png)

![](https://latex.codecogs.com/svg.latex?D%3D%5C%7B%28U%2CV%29%3AU%3Cx%2C%20V%3Cy%20%5C%7D)

![](https://latex.codecogs.com/svg.latex?P((\xi_1,\xi_2)&space;\in&space;D)=P(\xi_1<x,\xi_2<y)(==F_{\xi_1\xi_2}(x,y))=\int_{-\infty}^x\int_{-\infty}^yf(U,V)dUdV)

![](https://latex.codecogs.com/svg.latex?F_%7B%5Cxi_1%5Cxi_2%7D%28x%2Cy%29%3D%5Cint_%7B-%5Cinfty%7D%5Ex%5Cint_%7B-%5Cinfty%7D%5Eyf%28U%2CV%29dUdV%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%20%5Cint_%7B-%5Cinfty%7D%5ExdU%28%5Cint_%7B%5Cinfty%7D%5Eyf%28U%2CV%29dV%29%5C%5C%20%5Cint_%7B-%5Cinfty%7D%5EydV%28%5Cint_%7B%5Cinfty%7D%5Exf%28U%2CV%29dU%29%20%5Cend%7Bmatrix%7D%5Cright.)

  2.1. ![](https://latex.codecogs.com/svg.latex?f(x,y)&space;\rightarrow&space;F(x,y))
  2.2. ![](https://latex.codecogs.com/svg.latex?F(x,y),f(x,y)=\frac{\partial^2&space;F(x,y)}{\partial&space;x\partial&space;y})

Зная совместную плотность, можно всегда и притом однозначно найти плотность отдельно для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) и для ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2})

- ![](https://latex.codecogs.com/svg.latex?f_{\xi_1}(x)=\int_{-\infty}^{&plus;\infty}f(x,y)dy)
- ![](https://latex.codecogs.com/svg.latex?f_{\xi_2}(y)=\int_{-\infty}^{&plus;\infty}f(x,y)dx)

### Замечание

Но зная отдельно ![](https://latex.codecogs.com/svg.latex?f_{\xi_1}(x)) и ![](https://latex.codecogs.com/svg.latex?f_{\xi_2}(y)) в общем случае нельзя найти ![](https://latex.codecogs.com/svg.latex?f_{\xi_1\xi_2}(x,y))
