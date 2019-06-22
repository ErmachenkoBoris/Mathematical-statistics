# 9. Смещенная и несмещенная оценки для генеральной дисперсии: свойства, формулы для вычисления.
Dξ - генеральная дисперсия.
Строим оценку.

1. ![](https://latex.codecogs.com/svg.latex?M\xi=a) - известно

Тогда ![](https://latex.codecogs.com/svg.latex?\widetilde{D\xi}=\frac{1}{n}\sum_{i=1}^{n}(\xi_{i}-a)^{2})

a) Покажем, что оценка **несмещенная**

![](https://latex.codecogs.com/svg.latex?M(\widetilde{D\xi})=\frac{1}{n}((\xi_{1}-a)^{2}&plus;(\xi_{2}-a)^{2}&plus;...&plus;(\xi_{n}-a)^{2})=\frac{1}{n}*n*D\xi=D\xi)

b) ![](https://latex.codecogs.com/svg.latex?D(\widetilde{D\xi})\underset{n\rightarrow\infty}{\rightarrow}0) - **асимптотически эффективна**

c) **Состоятельность**

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
