# 12 Метод моментов для построения оценок неизвестных параметров распределения.

#### Теоретические моменты

![](https://latex.codecogs.com/svg.latex?%5Calpha_%7Bk%7D%5Cxi%3DM%28%5Cxi%5E%7Bk%7D%29%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%5Csum_%7Bi%7Dx_%7Bi%7D%5E%7Bk%7Dp%28%5Cxi%3Dx_%7Bi%7D%2Ca_%7B1%7D%2Ca_%7B2%7D%2C...%2Ca_%7Bn%7D%2Cesly%5Cxi-d.s.v.%29%5C%5C%5Cint_%7B-%5Cpropto%7D%5E%7B&plus;%5Cpropto%7Dx%5E%7Bk%7Df_%7B%5Cxi%7D%28x%2Ca_%7B1%7D%2Ca_%7B2%7D%2C...%2Ca_%7Bn%7D%2Cesly%5Cxi-n.s.v.%29%5Cend%7Bmatrix%7D%5Cright.)


![](https://latex.codecogs.com/svg.latex?%5Cbeta_%7Bk%7D%5Cxi%3DM%28%5Cxi-M_%7B%5Cxi%7D%29%5E%7Bk%7D%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%5Csum_%7Bi%7D%28x_%7Bi%7D-M_%7B%5Cxi%7D%29%5E%7Bk%7Dp%28%5Cxi%3Dx_%7Bi%7D%2Ca_%7B1%7D%2Ca_%7B2%7D%2C...%2Ca_%7Bn%7D%2Cesly%5Cxi-d.s.v.%29%5C%5C%5Cint_%7B-%5Cpropto%7D%5E%7B&plus;%5Cpropto%7D%28x-M_%7B%5Cxi%7D%29%5E%7Bk%7Df_%7B%5Cxi%7D%28x%2Ca_%7B1%7D%2Ca_%7B2%7D%2C...%2Ca_%7Bn%7D%2Cesly%5Cxi-n.s.v.%29%5Cend%7Bmatrix%7D%5Cright.) 


Записывают так :

![](https://latex.codecogs.com/svg.latex?\alpha&space;_{k}\xi(a_{1},a_{2},...,a_{m}),&space;\beta&space;_{k}\xi(a_{1},a_{2},...,a_{m}))

#### Статистические моменты

![](https://latex.codecogs.com/svg.latex?\alpha&space;_{k}^{*}=\frac{1}{n}\sum_{i=1}^{n}x_{i}^{k}) - начальный момент n-го порядка

![](https://latex.codecogs.com/svg.latex?\beta&space;_{k}^{*}=\frac{1}{n}\sum_{i=1}^{n}(x_{i}-\bar{x})^{k};\bar{x}=\frac{1}{n}\sum_{i=1}^{n}x_{i})

### Метод моментов

Если неизвестных параметров М, то нужно найти М любых теоретических моментов, а затем по выборке ![](https://latex.codecogs.com/svg.latex?x_{1},&space;x_{2},..,&space;x_{m}) посчитать соответсвующие им статистические моменты.

Далее их нужно приравнять. Получим систему из М уравнений с М неизвестными. 

Ее нужно решить относительно ![](https://latex.codecogs.com/svg.latex?a_{1},&space;a_{2},..,&space;a_{m})

Возможный несколько случаев

1. Решение едиственно 

![](https://latex.codecogs.com/svg.latex?\tilde{a}_{1},&space;\tilde{a}_{2},..,&space;\tilde{a}_{m})

![](https://latex.codecogs.com/svg.latex?\tilde{a}_{1}=a_{1}^{*},&space;\tilde{a}_{2}=a_{2}^{*},..,&space;\tilde{a}_{m}=a_{m}^{*})

Утверждается, что эти оценки будут состоятельными, решение единственно

2. Решений несколько

Тогда в качестве оценок можем взять любое из них. Но в этом случае ничего о состоятельности сказать нельзя.

3. Система не имеет решений.

Говорим, что решений по методу оценок не существует.

При решении задач рекомендуется брать простые моменты

Пример решения задачи смотри в лекциях
