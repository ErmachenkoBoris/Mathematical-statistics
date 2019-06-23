# 2. Определение двумерной совместной функции распределения F(x,y), ее свойства.

![](https://latex.codecogs.com/svg.latex?F(x,y)_{-\infty<x,y<&plus;\infty}=P(\{\xi_{1}<x&space;\}\cap&space;\{\xi_{2}<y&space;\})=P(\xi_{1}<x,\xi_{2}<y)) - совместная функция распределения

### **Свойства**:
- ![](https://latex.codecogs.com/svg.latex?0\leqslant&space;F(x,y)\leqslant1,&space;\forall&space;x,&space;\forall&space;y)
- Функция убывает по каждому своему аргументу
- Функция непрерывна слева по каждому своему аргументу
- Предельные свойства
  - ![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow&space;-\infty,&space;y\rightarrow&space;-\infty}F(x,y)=&space;F(-\infty,&space;-\infty)=P(\xi_{1}<-\infty,&space;\xi_{2}<-\infty)=P(\O&space;)=0)
  - ![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow&space;-\infty,&space;\forall&space;y-fixed}F(x,y)=&space;F(-\infty,&space;y)=P(\xi_{1}<-\infty,&space;\xi_{2}<y)=P(\O&space;)=0)
  - ![](https://latex.codecogs.com/svg.latex?\lim_{\forall&space;x-fixed,&space;y\rightarrow&space;-\infty}F(x,y)=&space;F(x,-\infty)=P(\xi_{1}<x,&space;\xi_{2}<-\infty)=P(\O&space;)=0)
  - ![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow&space;&plus;\infty,&space;\forall&space;y\rightarrow&space;&plus;\infty}F(x,y)=&space;F(&plus;\infty,&space;&plus;\infty)=P(\xi_{1}<&plus;\infty,&space;\xi_{2}<&plus;\infty)=P(\Omega&space;)=1)
  - ![](https://latex.codecogs.com/svg.latex?\lim_{x\rightarrow&space;&plus;\infty,&space;\forall&space;y-fixed}F(x,y)=&space;F(&plus;\infty,&space;y)=P(\xi_{1}<&plus;\infty,&space;\xi_{2}<y)=P(\xi_{2}<y)=F_{\xi_{2}}(y))
  - ![](https://latex.codecogs.com/svg.latex?\lim_{\forall&space;x-fixed,&space;y\rightarrow&space;&plus;\infty}F(x,y)=&space;F(x,&plus;\infty)=P(\xi{1}<x,\xi_{2}<&plus;\infty)=P(\xi_{1}<x)=F_{\xi_{1}}(x))
- Вероятность попадания с.в. ![](https://latex.codecogs.com/svg.latex?(\xi_1,\xi_2)) в прямоугольник
  ![](../../images/two-dimensional_random_variables/ticket2-1.png)
  ![](https://latex.codecogs.com/svg.latex?a&space;\leqslant&space;x<b,&space;c&space;\leqslant&space;y<d)
  ![](https://latex.codecogs.com/svg.latex?P(a&space;\leqslant&space;\xi_1<b,&space;c&space;\leqslant&space;\xi_2<d)=F(b,d)&plus;F(a,c)-F(b,c)-F(a,d))

### Замечание
Если ![](https://latex.codecogs.com/svg.latex?(\xi_1,\xi_2)) непрерывного типа, то:
- Функция F(x,y) также непрерывна справа по каждому своему аргументу, т.е. является просто непрерывной функцией и по x, и по y.
- Вероятность попадания в прямоугольник будет вычисляться независимо от того, как стоят знаки.


![](https://latex.codecogs.com/svg.latex?F_\xi_1(x)=F_{\xi_1\xi_2}(x,&plus;\infty))
![](https://latex.codecogs.com/svg.latex?F_\xi_2(y)=F_{\xi_1\xi_2}(&plus;\infty,y))

Зная совместную двумерную функцию распределения, можно всегда, и притом однозначно, получить фукнции распределения отдельно для ![](https://latex.codecogs.com/svg.latex?\xi_1) и для ![](https://latex.codecogs.com/svg.latex?\xi_2). Неверно в обратную сторону.