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