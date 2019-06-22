# 10. Точность и надежность несмещенной оценки для дисперсии. Три задачи и их решение.
Для точного нахождения гамма, нужно знать Dξ и четвёртый центральный момент.
Используем приближенную формулу для нахождения гамма.
![](https://latex.codecogs.com/svg.latex?\gamma=P(|\widetilde{D\xi}_{changed}-D\xi|<\varepsilon)=\Phi(\frac{\varepsilon\sqrt{n-1}}{\sqrt{2}D\xi}))
Точная формула, если ξ распределена по нормальному закону.
В этой формуле мы не знаем Dξ, поэтому заменяем ее несмещенной оценкой.

С помощью этого уравнения решаются те же самые 3 задачи.

### Три задачи
1. Знаем ε и n.
![](https://latex.codecogs.com/svg.latex?\gamma) = ?
![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n-1}}{\sqrt{2}D\xi}=x_{0})

| x      | ![](https://latex.codecogs.com/svg.latex?\Phi(x)) |
|--------------|------------|
| ![](https://latex.codecogs.com/svg.latex?x_{0}\rightarrow) | ![](https://latex.codecogs.com/svg.latex?\gamma) |

2. Знаем ![](https://latex.codecogs.com/svg.latex?\gamma) и n.
ε = ?

| x   | ![](https://latex.codecogs.com/svg.latex?\Phi(x))           |
|----------|----------|
| ![](https://latex.codecogs.com/svg.latex?t_{\gamma}) | ![](https://latex.codecogs.com/svg.latex?\leftarrow\gamma) |

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n-1}}{\sqrt{2}D\xi}=t_{\gamma}\rightarrow\varepsilon)

3. Знаем ![](https://latex.codecogs.com/svg.latex?\gamma) и ε.
n = ?

| x   | ![](https://latex.codecogs.com/svg.latex?\Phi(x))           |
|----------|----------|
| ![](https://latex.codecogs.com/svg.latex?t_{\gamma}) | ![](https://latex.codecogs.com/svg.latex?\leftarrow\gamma) |

![](https://latex.codecogs.com/svg.latex?\frac{\varepsilon\sqrt{n-1}}{\sqrt{2}D\xi}=t_{\gamma}\rightarrow\sqrt{n-1}=\frac{t_{\gamma}*D\xi*\sqrt{2}}{\varepsilon}=\frac{t_{\gamma}^{2}*D\xi^{2}*2}{\varepsilon^{2}})

___
### Нахождение
![](https://latex.codecogs.com/svg.latex?\overline{x}=\frac{1}{n}\sum_{i=1}^{n}x_{i})

![](https://latex.codecogs.com/svg.latex?D\xi_{changed}=\frac{1}{n-1}\sum_{i=1}^{n}(x_{i}-\overline{x})^{2})

По этим формулам найдем смещенную оценку ![](https://latex.codecogs.com/svg.latex?D\xi_{*}).

![](https://latex.codecogs.com/svg.latex?D\xi_{changed}=\frac{n}{n-1}D\xi_{*})