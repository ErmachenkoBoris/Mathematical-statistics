# 5. Статистические аналоги для математического ожидания, дисперсии, начальных и центральных моментов. Формулы для их вычисления в зависимости от способа представления данных.

Статистические аналоги Mξ и Dξ - M\*ξ и D\*ξ.
Их формулы похожи на Mξ и Dξ Д.С.В.

![](https://latex.codecogs.com/svg.latex?M\xi=\sum_{i}^{n}x_{i}p_{i})

![](https://latex.codecogs.com/svg.latex?%5Csmall%20D%5Cxi%3DM%5C%7B%28%5Cxi-M%5Cxi%29%5E%7B2%7D%5C%7D%3D%5Csum_%7Bi%7D%5E%7Bn%7D%28x_%7Bi%7D-M%5Cxi%29%5E%7B2%7D*p_%7Bi%7D%3DM%28%5Cxi%29%5E%7B2%7D-%28M%5Cxi%29%5E%7B2%7D%3D%5Csum_%7Bi%7D%5E%7Bn%7Dx_%7Bi%7D%5E%7B2%7D*p_%7Bi%7D-%28M%5Cxi%29%5E%7B2%7D)

1. Данные представлены в виде простого или вариационного ряда
![](https://latex.codecogs.com/svg.latex?x_{1}),![](https://latex.codecogs.com/svg.latex?x_{2}),...,![](https://latex.codecogs.com/svg.latex?x_{n})
![](https://latex.codecogs.com/svg.latex?M\xi&space;^{*}=\frac{1}{n}\sum_{i=1}^{n}x_{i})
![](https://latex.codecogs.com/svg.latex?D\xi&space;^{*}=\frac{1}{n}\sum_{i=1}^{n}(x_{i}-M\xi&space;^{*})^{2}=\frac{1}{n}\sum_{i=1}^{n}x_{i}^{2}-(M\xi&space;^{*})^{2})

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

![](https://latex.codecogs.com/svg.latex?\alpha_{k}^{*}\xi) - статистический аналог начального момента k-го порядка

![](https://latex.codecogs.com/svg.latex?\alpha_{k}^{*}\xi=\frac{1}{n}\sum_{i=1}^{n}x_{i}^{k})

![](https://latex.codecogs.com/svg.latex?\beta_{k}^{*}\xi) - статистический аналог центрального момента k-го порядка

![](https://latex.codecogs.com/svg.latex?\beta_{k}^{*}\xi=\frac{1}{n}\sum_{i=1}^{n}(x_{i}-\overline{x})^{k})

![](https://latex.codecogs.com/svg.latex?\overline{x}=\frac{1}{n}\sum_{i=1}^{n}x_{i})
