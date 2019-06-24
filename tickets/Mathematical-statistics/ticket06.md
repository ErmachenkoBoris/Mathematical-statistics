# 6. Статистические оценки параметров. Требования несмещенности, состоятельности и эффективности в некотором множестве оценок. Понятие сходимости по вероятности случайной последовательности. Основные теоремы для проверки состоятельности оценок.

Пусть для случайной величины ξ признака генеральной совокупности, известна точность распределения до параметров

![](https://latex.codecogs.com/svg.latex?\xi\rightarrow(x;a_{1},a_{2},...,a_{m}),m\geq1)

С помощью методов математической статистики найти параметры нельзя. Можно только оценки для этих параметров.
Выберем из генеральной совокупности n элементов и получим n экземпляров
![](https://latex.codecogs.com/svg.latex?\xi_{1}),...,![](https://latex.codecogs.com/svg.latex?\xi_{n})

Оценка ![](https://latex.codecogs.com/svg.latex?a_{1}) - ![](https://latex.codecogs.com/svg.latex?\widetilde{a_{1}}=\varphi_{1}(\xi_{1},\xi_{2},...,\xi_{n}))

![](https://latex.codecogs.com/svg.latex?\widetilde{a_{2}}=\varphi_{2}(\xi_{1},\xi_{2},...,\xi_{n}))

...

![](https://latex.codecogs.com/svg.latex?\widetilde{a_{m}}=\varphi_{m}(\xi_{1},\xi_{2},...,\xi_{n}))

Все это статистические оценки для параметров. Функции от С.В. => они сами являются С.В.

### Требования к оценкам
1. **Понятие несмещенности оценки**
![](https://latex.codecogs.com/svg.latex?a\rightarrow\widetilde{a}=\varphi(\xi_{1},\xi_{2},...,\xi_{n}))

Если для любого n=1,2,...,

![](https://latex.codecogs.com/svg.latex?M(\widetilde{a})=a)
, то оценка называется несмещенной.

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

, то построенная оценка называется состоятельной

___
На практике используются 3 теоремы состоятельности.

1. **Теорема Чебышева**
![](https://latex.codecogs.com/svg.latex?\xi_{1},\xi_{2},...,\xi_{n}) - последовательность, имеющая одинаковые С.В.

![](https://latex.codecogs.com/svg.latex?M\xi_{i}=m,D\xi_{i}=d,&space;i=1,2,...,)

Образуем С.В. ![](https://latex.codecogs.com/svg.latex?\eta_{n}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})

Последовательность ![](https://latex.codecogs.com/svg.latex?\eta_{1},\eta_{2},...,\eta_{n}) сходиться при ![](https://latex.codecogs.com/svg.latex?n\rightarrow\infty) к m

![](https://latex.codecogs.com/svg.latex?\xrightarrow[n\rightarrow\infty]{P}m)

2. Если оценка ![](https://latex.codecogs.com/svg.latex?\widetilde{a}) является состоятельной для параметра a, то для любой непрерывной функции g, оценка ![](https://latex.codecogs.com/svg.latex?g(\widetilde{a})) будет состоятельной для параметра g(a).

3. Пусть ![](https://latex.codecogs.com/svg.latex?\widetilde{a}) является несмещенной оценкой для параметра a и ![](https://latex.codecogs.com/svg.latex?D(\widetilde{a})\underset{n\rightarrow\infty}{\rightarrow}0), тогда оценка ![](https://latex.codecogs.com/svg.latex?\widetilde{a}) будет состоятельной для параметра a.
___
3. Понятие **Эффективности** оценки в множестве оценок
Предположим, что для

![](https://latex.codecogs.com/svg.latex?a%20%5Crightarrow%20%5Cbegin%7Bmatrix%7D%20%5Cwidetilde%7Ba%7D%5E%7B%281%29%7D%5C%5C%20%5Cwidetilde%7Ba%7D%5E%7B%28n%29%7D%20%5C%5C%20...%5C%5C%20%5Cwidetilde%7Ba%7D%5E%7B%28m%29%7D%20%5Cend%7Bmatrix%7D)

существуют несмещенные оценки.
Из них нужно взять ту, у которой меньше Дисперсия ![](https://latex.codecogs.com/svg.latex?D\xi^{*}).

Оценка называется эффективной на некотором множестве, если она имеет наименьшую Дисперсию ![](https://latex.codecogs.com/svg.latex?D\xi^{*}).
