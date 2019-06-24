# 19. Критерий согласия Пирсона для непрерывных случайных величин.

### Проверка гипотезы о законе распределения при помощи критерия ![](https://latex.codecogs.com/svg.latex?\chi_{cr}^{2})("Хи-квадрат") Пирсона (Согласия Пирсона)

Пусть гипотеза ![](https://latex.codecogs.com/svg.latex?H_{0}): случайная величина ![](https://latex.codecogs.com/svg.latex?\xi) имеет функция распределения ![](https://latex.codecogs.com/svg.latex?F_{\xi}(x)=) - формула(не важно какая)

Гипотеза ![](https://latex.codecogs.com/svg.latex?H_{1}): функция распределения - другая формула

Требуется проверить ![](https://latex.codecogs.com/svg.latex?H_{0}) с заданным уровнем значимости 
![](https://latex.codecogs.com/svg.latex?\alpha)

2) Рассмотрим случай, когда ![](https://latex.codecogs.com/svg.latex?\xi) - непрерывная случайная величина. (первый случай в предыдущем билете)

Получим n значений этой случайной величины ![](https://latex.codecogs.com/svg.latex?x_{1},x_{2},...,x_{n}). Т.к. ![](https://latex.codecogs.com/svg.latex?\xi) - непрерывная, то вообще говоря одинаковых среди них быть не должно. Для того, чтобы применить критерий нужно обязательно построить группированный ряд:

| ![](https://latex.codecogs.com/svg.latex?(y_{i};y_{i&plus;1}))  | ![](https://latex.codecogs.com/svg.latex?[y_{1};y_{2}))  |  ![](https://latex.codecogs.com/svg.latex?[y_{2};y_{3})) | ...  |  ![](https://latex.codecogs.com/svg.latex?(y_{k};y_{k&plus;1})) |
|---|---|---|---|---|
| ![](https://latex.codecogs.com/svg.latex?l_{i})  |  ![](https://latex.codecogs.com/svg.latex?l_{1}) | ![](https://latex.codecogs.com/svg.latex?l_{2})  | ...  |  ![](https://latex.codecogs.com/svg.latex?l_{k}) |

![](https://latex.codecogs.com/svg.latex?l_{i}) - число точек, попавших в разряд

![](https://latex.codecogs.com/svg.latex?\sum_{i=1}^{k}l_{i}=n)

На практике берем 3-4 разряда

В этом случае взяли k разрядов

Рассмотрим случайную величину ![](https://latex.codecogs.com/svg.latex?R=\sum_{i=1}^{k}\frac{(l_{i}-np_{i})^2}{np_{i}})

Используя данные нашей таблички подставим ![](https://latex.codecogs.com/svg.latex?l_{i})  и вычислим R наблюдаемое. Где k - число разрядов, которые мы выбрали сами.

n - число выборки

![](https://latex.codecogs.com/svg.latex?p_{i})  - вероятность, что ![](https://latex.codecogs.com/svg.latex?\xi_{i}) (??) попадет в i-ый разряд

![](https://latex.codecogs.com/svg.latex?P_%7Bi%7D%3DP%20%5Cleft%20%28%20%5Cxi%20%5Cin%20%5By_%7Bi%7D%2Cy_%7Bi&plus;1%7D%29%20%5Cright%20%29%3DF_%7B%5Cxi%7D%28y_%7Bi&plus;1%7D%29-F_%7B%5Cxi%7D%28y_%7Bi%7D%29)

Вычисляется согласно гипотезе ![](https://latex.codecogs.com/svg.latex?H_{0})

r - число степеней свобод - считается также как и с д.с.в.

Остальное считается также как и с д.с.в.
