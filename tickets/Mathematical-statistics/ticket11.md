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


### Покажем, что эта оценка удовлетворяла всем требованиям, чтобы она была "хорошей"

![](https://latex.codecogs.com/svg.latex?M_{\xi_{i}}&space;=&space;p)

![](https://latex.codecogs.com/svg.latex?D_{\xi_{i}}&space;=&space;p^{2}&space;-&space;p&space;=&space;p(1-p)=&space;pq)

#### 1. Несмещенность
![](https://latex.codecogs.com/svg.latex?M(\tilde{P})=\frac{1}{n}(M_{\xi&space;_{1}}&plus;&space;M_{\xi&space;_{2}}&space;&plus;&space;...&space;&plus;&space;M_{\xi&space;_{n}})&space;=&space;\frac{1}{n}&space;\cdot&space;np&space;=&space;p)
#### 2. Асимптотическая эффективность
![](https://latex.codecogs.com/svg.latex?D(\tilde{P})=\frac{1}{n^{2}}(D_{\xi&space;_{1}}&plus;&space;D_{\xi&space;_{2}}&space;&plus;&space;...&space;&plus;&space;D_{\xi&space;_{n}})&space;=&space;\frac{1}{n^{2}}&space;\cdot&space;npq&space;=&space;\frac{pq}{n})

![](https://latex.codecogs.com/svg.latex?\lim_{n&space;\to&space;\propto&space;}&space;(\frac{pq}{n})&space;=&space;0)

#### 3. Состоятельность
Из 1, 2 по теореме 3 следует состоятельность

#### 4. 
![](https://latex.codecogs.com/svg.latex?\gamma&space;=&space;P(\left&space;|&space;\tilde{P}&space;-&space;P&space;\right&space;|&space;<&space;\varepsilon&space;)&space;=&space;...&space;=&space;\Phi&space;(\frac{\varepsilon&space;\sqrt{n}}{\sqrt{pq}}))

p, q - мы не знаем. p, q мы заменяем оценками.

Предположим, что опыт провели n раз и n раз наблюдали событие А. Тогда относительная частота будет

![](https://latex.codecogs.com/svg.latex?\tilde{p}=\tfrac{m}{n})

![](https://latex.codecogs.com/svg.latex?\tilde{q}=1&space;-&space;\tfrac{m}{n})

![](https://latex.codecogs.com/svg.latex?\approx&space;\Phi&space;(\frac{\varepsilon&space;\sqrt{n}}{\sqrt{\tfrac{m}{n}(1-\frac{m}{n}))}}))

Мы можем решить те же 3 задачки, рассматриваемые ранее 
Задача: ![](https://latex.codecogs.com/svg.latex?\gamma&space;,&space;\varepsilon) - известны, нужно найти n. 

![](https://latex.codecogs.com/svg.latex?\gamma=0,95), то ![](https://latex.codecogs.com/svg.latex?n\approx&space;\frac{1}{\varepsilon&space;^{2}})
