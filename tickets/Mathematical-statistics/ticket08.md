# 8. Точность и надежность несмещенной оценки для математического ожидания. Три задачи и их решение.
![](https://latex.codecogs.com/svg.latex?\widetilde{M\xi}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})

Покажем, что эта оценка хороша

1. **Несмещенность**
![](https://latex.codecogs.com/svg.latex?M(\widetilde{M\xi})=M\xi) - выполняется

![](https://latex.codecogs.com/svg.latex?M(\frac{1}{n}\sum_{i=1}^{n}\xi_{i})=\frac{1}{n}(M\xi_{1}&plus;M\xi_{2}&plus;...&plus;M\xi_{n})=\frac{1}{n}*n*M\xi=M\xi)

2. **Состоятельность**
n = 1, 2, ...,


Получится последовательность оценок
![](https://latex.codecogs.com/svg.latex?\frac{1}{n}\sum_{i=1}^{n}\xi_{i}\xrightarrow[n\rightarrow\infty]{P}M\xi)

По Т. Чебышева.

Выполнены условия теоремы Чебышева из нее непосредственно следует это равенство.

3. **Эффективность**
Рассмотрим свойства асимптотической эффективности.

![](https://latex.codecogs.com/svg.latex?a\rightarrow\widetilde{a}=\varphi(\xi_{1},\xi_{2},...,\xi_{n}))

Если при ![](https://latex.codecogs.com/svg.latex?n\rightarrow\infty), ![](https://latex.codecogs.com/svg.latex?D(\widetilde{a_{n}})\rightarrow0), то оценка асимптотически эффективна.

4. Точность и надежность
![](https://latex.codecogs.com/svg.latex?P(|\widetilde{M\xi}-M\xi|<\varepsilon)=\gamma)

Где ![](https://latex.codecogs.com/svg.latex?\widetilde{M\xi}) - С.В.

![](https://latex.codecogs.com/svg.latex?M\xi) - Случайное событие

Можно показать что в этом случае Гамма вычисляется по формуле:

![](https://latex.codecogs.com/svg.latex?\gamma=\Phi(\frac{\varepsilon\sqrt{n}}{\sqrt{D\xi}}))

![](https://latex.codecogs.com/svg.latex?\Phi(x)=\frac{2}{\sqrt{2\pi}}*\int_{0}^{x}e^{-\frac{t^{2}}{2}}dt)

![](../../images/Mathematical-statistics/ticket08.png)

* Для того чтобы увеличить гамму, из графика видно, что нужно увеличить аргумент X.
Если ε задана, Dξ = const, то существует единственный способ - увеличение n.
* В формуле стоит Dξ. На практике мы ее не знаем, следовательно заменяем ее оценкой Dξ.
* Полученное равенство можно рассматривать как некоторые уравнения связывающие ![](https://latex.codecogs.com/svg.latex?\gamma), ε и n.
___
### Три задачи
1. Знаем ε и n.
![](https://latex.codecogs.com/svg.latex?\gamma) = ?

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n}}{\sqrt{D\xi}}=x_{0})

| x      | ![](https://latex.codecogs.com/svg.latex?\Phi(x)) |
|--------------|------------|
| ![](https://latex.codecogs.com/svg.latex?x_{0}\rightarrow) | ![](https://latex.codecogs.com/svg.latex?\gamma) |

2. Знаем ![](https://latex.codecogs.com/svg.latex?\gamma) и n.
ε = ?

| x   | ![](https://latex.codecogs.com/svg.latex?\Phi(x))           |
|----------|----------|
| ![](https://latex.codecogs.com/svg.latex?t_{\gamma}) | ![](https://latex.codecogs.com/svg.latex?\leftarrow\gamma) |

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n}}{\sqrt{D\xi}}=t_{\gamma}\rightarrow\varepsilon)

3. Знаем ![](https://latex.codecogs.com/svg.latex?\gamma) и ε.
n = ?

| x   | ![](https://latex.codecogs.com/svg.latex?\Phi(x))           |
|----------|----------|
| ![](https://latex.codecogs.com/svg.latex?t_{\gamma}) | ![](https://latex.codecogs.com/svg.latex?\leftarrow\gamma) |

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n}}{\sqrt{D\xi}}=t_{\gamma}\rightarrow\sqrt{n}=\frac{t_{\gamma}\sqrt{D\xi}}{\varepsilon}=\frac{t_{\gamma}^{2}*D\xi}{\varepsilon^{2}})
