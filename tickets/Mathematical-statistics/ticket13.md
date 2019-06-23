# 13 Метод максимального правдоподобия для построения оценок. (или "Максимума") 

Суть: строится так называемая функция правдоподобияЮ которая зависит от некоторых параметров
![](https://latex.codecogs.com/gif.latex?a_{1},a_{2},...,a_{m})

Далее у этой функции находятся такие параметры ![](https://latex.codecogs.com/gif.latex?a_{1}^{*},a_{2}^{*},...,a_{m}^{*}) , которые обеспечивают максимум и эти значения берутся в качестве оценок максимального правдоподобия

Пусть
1) ![](https://latex.codecogs.com/gif.latex?\xi&space;-&space;d.s.v,&space;P(\xi&space;=&space;x;&space;a_{1},&space;a_{2},&space;...,&space;a_{m}))

получим выборку

![](https://latex.codecogs.com/gif.latex?x_{1},x_{2},...x_{n})

![](https://latex.codecogs.com/gif.latex?%5Cbegin%7Bmatrix%7DP%28%5Cxi%3Dx_%7B1%7D%3B%20a_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5C%5C%20P%28%5Cxi%3Dx_%7B2%7D%3B%20a_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5C%5C%20%5Ccdot%20%5C%5C%20%5Ccdot%20%5C%5C%20%5Ccdot%20%5C%5C%20P%28%5Cxi%3Dx_%7Bn%7D%3B%20a_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5Cend%7Bmatrix%7D)

![](https://latex.codecogs.com/gif.latex?L_{x_{1},&space;x_{2},...,x_{n}}(a_{1},a_{2},..,a_{m})=\prod_{i=1}^{n}p(\xi=x_{i},&space;a_{1},a_{2},..,a_{m}))

2) ![](https://latex.codecogs.com/gif.latex?\xi-n.s.v,f_{\xi}(x;a_{1},a_{2},...,a_{m}))

получим выборку

![](https://latex.codecogs.com/gif.latex?x_{1},x_{2},...x_{n})

Считаем эту плотность для полученных значений
![](https://latex.codecogs.com/gif.latex?L_{x_{1},x_{2},...,x_{n}}(a_{1},a_{2},..,a_{m})=\prod_{i=1}^{n}f_{\xi}(x_{i},a_{1},a_{2},..,a_{m}))

![](https://latex.codecogs.com/gif.latex?%5Cbegin%7Bmatrix%7D%20f_%7B%5Cxi%7D%28x_%7B1%7D%3Ba_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5C%5C%20f_%7B%5Cxi%7D%28x_%7B2%7D%3Ba_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5C%5C%20%5Ccdot%20%5C%5C%20%5Ccdot%20%5C%5C%20%5Ccdot%20%5C%5C%20f_%7B%5Cxi%7D%28x_%7Bn%7D%3Ba_%7B1%7D%2C..%2Ca_%7Bm%7D%29%20%5Cend%7Bmatrix%7D)

Часто в практических задачах L- диффференцируема по параметрам ![](https://latex.codecogs.com/gif.latex?a_{1},a_{2},...a_{m})

Тогда для нахождения критических точек используют:

![](https://latex.codecogs.com/gif.latex?%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%5Cfrac%7B%5Cpartial%20L%28a_%7B1%7D%2Ca_%7B2%7D%2C..%2Ca_%7Bn%7D%29%7D%7B%5Cpartial%20a_%7Bj%7D%7D%20%3D%200%20%5C%5C%20j%20%3D%20%5Coverline%7B1%2C%20m%7D%20%5Cend%7Bmatrix%7D%5Cright.)

Есть свойство, если f(x)>0 и Lnf(x) - имеют одни и те же точки экстренума.

Рекомендуется находить точки экстренума не самой функции L, а у Ln(L) - это проще

Обычно находят так :

![](https://latex.codecogs.com/gif.latex?%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%5Cfrac%7B%5Cpartial%20ln%20%28L%28a_%7B1%7D%2Ca_%7B2%7D%2C..%2Ca_%7Bn%7D%29%29%7D%7B%5Cpartial%20a_%7Bj%7D%7D%20%3D%200%20%5C%5C%20j%20%3D%20%5Coverline%7B1%2C%20m%7D%20%5Cend%7Bmatrix%7D%5Cright.)

Примеры решения задач смотреть в лекциях