# Билет 11. Оценка для вероятности: ее свойства, точность и надежность.
Пусть имеется случайный эксперимент

![](https://latex.codecogs.com/svg.latex?P=P(A)=?)

Задача: требуется построить оценку

![](https://latex.codecogs.com/svg.latex?\tilde{P}=\tilde{P}(A))

Проведем эксперимент 1ый раз. Пусть с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1}) - число появлений события А в первом опыте

Проведем 2ой раз.  с.в. ![](https://latex.codecogs.com/svg.latex?\xi&space;_{2}) - число появлений события А во втором опыте. Имеет тоже самое распределение как ![](https://latex.codecogs.com/svg.latex?\xi&space;_{1})

и т.д.
Проведем n-ый раз, получим ![](https://latex.codecogs.com/svg.latex?\xi&space;_{n}). Она имеет тоже самое распределение (Бернуллевская св???)

Посчитаем их сумму

![](https://latex.codecogs.com/svg.latex?\xi=\sum_{i=1}^{n}\xi_{i}) - общее количество наступления события А

![](https://latex.codecogs.com/svg.latex?\frac{1}{n}\sum_{i=1}^{n}\xi_{i}) - относительная частота наступления события А

![](https://latex.codecogs.com/svg.latex?\tilde{P}=\frac{1}{n}\sum_{i=1}^{n}\xi_{i})


## Покажем, что эта оценка удовлетворяла всем требованиям, чтобы она была "хорошей"

![](https://latex.codecogs.com/svg.latex?M_{\xi_{i}}&space;=&space;p)

![](https://latex.codecogs.com/svg.latex?D_{\xi_{i}}&space;=&space;p^{2}&space;-&space;p&space;=&space;p(1-p)=&space;pq)

### 1. Несмещенность
![](https://latex.codecogs.com/svg.latex?M(\tilde{P})=\frac{1}{n}(M_{\xi&space;_{1}}&plus;&space;M_{\xi&space;_{2}}&space;&plus;&space;...&space;&plus;&space;M_{\xi&space;_{n}})&space;=&space;\frac{1}{n}&space;\cdot&space;np&space;=&space;p)
### 2. Асимптотическая эффективностб

### 3. Состоятельность

###

###
