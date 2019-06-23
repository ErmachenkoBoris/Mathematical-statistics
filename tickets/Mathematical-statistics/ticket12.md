# 12 Метод моментов для построения оценок неизвестных параметров распределения.

#### Теоретические моменты

![](https://latex.codecogs.com/gif.latex?\alpha&space;_{k}\xi&space;=&space;M&space;(\xi&space;^{k})=\left\{\begin{matrix}&space;\sum_{i}x_{i}^{k}p(\xi&space;=&space;x_{i},&space;a_{1},&space;a_{2},...,&space;a_{n},&space;esly&space;\xi&space;-&space;d.s.v.)\\&space;\int_{-\propto&space;}^{&plus;\propto&space;}x^{k}f_{\xi&space;}(x,&space;a_{1},&space;a_{2},...,&space;a_{n},&space;esly&space;\xi&space;-&space;n.s.v.)&space;\end{matrix}\right.)
(тут фигурная скобка)

![](https://latex.codecogs.com/gif.latex?\beta&space;_{k}\xi&space;=&space;M&space;(\xi-M_{\xi})&space;^{k}=\left\{\begin{matrix}&space;\sum_{i}(x_{i}-M_{\xi})^{k}p(\xi&space;=&space;x_{i},&space;a_{1},&space;a_{2},...,&space;a_{n},&space;esly&space;\xi&space;-&space;d.s.v.)\\&space;\int_{-\propto&space;}^{&plus;\propto&space;}(x-M_{\xi&space;})^{k}f_{\xi&space;}(x,&space;a_{1},&space;a_{2},...,&space;a_{n},&space;esly&space;\xi&space;-&space;n.s.v.)&space;\end{matrix}\right.) 
(тут фигурная скобка)

Записывают так :

![](https://latex.codecogs.com/gif.latex?\alpha&space;_{k}\xi(a_{1},a_{2},...,a_{m}),&space;\beta&space;_{k}\xi(a_{1},a_{2},...,a_{m}))

#### Статистические моменты

![](https://latex.codecogs.com/gif.latex?\alpha&space;_{k}^{*}=\frac{1}{n}\sum_{i=1}^{n}x_{i}^{k}) - начальный момент n-го порядка

![](https://latex.codecogs.com/gif.latex?\beta&space;_{k}^{*}=\frac{1}{n}\sum_{i=1}^{n}(x_{i}-\bar{x})^{k};\bar{x}=\frac{1}{n}\sum_{i=1}^{n}x_{i})

### Метод моментов

Если неизвестных параметров М, то нужно найти М любых теоретических моментов, а затем по выборке ![](https://latex.codecogs.com/gif.latex?x_{1},&space;x_{2},..,&space;x_{m}) посчитать соответсвующие им статистические моменты.

Далее их нужно приравнять. Получим систему из М уравнений с М неизвестными. 

Ее нужно решить относительно ![](https://latex.codecogs.com/gif.latex?a_{1},&space;a_{2},..,&space;a_{m})

Возможный несколько случаев

1. Решение едиственно 

![](https://latex.codecogs.com/gif.latex?\tilde{a}_{1},&space;\tilde{a}_{2},..,&space;\tilde{a}_{m})

![](https://latex.codecogs.com/gif.latex?\tilde{a}_{1}=a_{1}^{*},&space;\tilde{a}_{2}=a_{2}^{*},..,&space;\tilde{a}_{m}=a_{m}^{*})

Утверждается, что эти оценки будут состоятельными, решение единственно

2. Решений несколько

Тогда в качестве оценок можем взять любое из них. Но в этом случае ничего о состоятельности сказать нельзя.

3. Система не имеет решений.

Говорим, что решений по методу оценок не существует.

При решении задач рекомендуется брать простые моменты

Пример решения задачи смотри в лекциях