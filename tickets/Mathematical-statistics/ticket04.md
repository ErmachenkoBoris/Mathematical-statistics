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
![](../../images/Mathematical-statistics/ticket04-1.png)

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

![](../../images/Mathematical-statistics/ticket04-2.png)

Площадь этой фигуры = 1
