# 3. Простой и вариационный статистические ряды. Статистическое распределение выборки. Информационно-статистическая таблица.
Измерим ![](https://latex.codecogs.com/svg.latex?\xi_{1}),...,![](https://latex.codecogs.com/svg.latex?\xi_{n}) и найдем их значения.

![](https://latex.codecogs.com/svg.latex?%5Cleft.%5Cbegin%7Bmatrix%7D%20%5Cxi%20_%7B1%7D%5Crightarrow%20x_%7B1%7D%20%5C%5C%20%5Cxi%20_%7B2%7D%5Crightarrow%20x_%7B2%7D%20%5C%5C%20...%5C%5C%20%5Cxi%20_%7Bn%7D%5Crightarrow%20x_%7Bn%7D%20%5Cend%7Bmatrix%7D%5Cright%5C%7D) статистические данные

![](https://latex.codecogs.com/svg.latex?\xi_{1}),...,![](https://latex.codecogs.com/svg.latex?\xi_{n}) - С.В.

![](https://latex.codecogs.com/svg.latex?x_{1}),...,![](https://latex.codecogs.com/svg.latex?x_{n}) - числа

| N | 1 | 2 | ... | n  |
|---|---|---|-----|----|
| Значение ![](https://latex.codecogs.com/svg.latex?\xi) | ![](https://latex.codecogs.com/svg.latex?x_{1}) | ![](https://latex.codecogs.com/svg.latex?x_{2}) | ... | ![](https://latex.codecogs.com/svg.latex?x_{n}) | 

Это **простой статистический ряд**

Если эти значения упорядочиваются в порядке возрастания, то этот ряд называется **вариационным**
![](https://latex.codecogs.com/svg.latex?x_{1}\leq&space;x_{2}\leq...\leq&space;x_{n})

**Вариационный ряд** - сами значения  - варианты.

При наблюдении за дискретными или непрерывными случайными величинами, при округлении их значений может быть много одинаковых значений.
Удобно из этой таблицы выделить только разные значения и посчитать сколько они встречались.

Пусть уникальных будет ![](https://latex.codecogs.com/svg.latex?k\leq&space;n)

| ![](https://latex.codecogs.com/svg.latex?x_{i})                     | ![](https://latex.codecogs.com/svg.latex?x_{1})      | ![](https://latex.codecogs.com/svg.latex?x_{2})      | ... | ![](https://latex.codecogs.com/svg.latex?x_{k})      |
|---------------------------------------------------------------------|------------------------------------------------------|------------------------------------------------------|-----|------------------------------------------------------|
| ![](https://latex.codecogs.com/svg.latex?n_{i})                     | ![](https://latex.codecogs.com/svg.latex?n_{1})      | ![](https://latex.codecogs.com/svg.latex?n_{2})      | ... | ![](https://latex.codecogs.com/svg.latex?n_{k})      |
| ![](https://latex.codecogs.com/svg.latex?p_{i}^{*}=\frac{n_{i}}{n}) | ![](https://latex.codecogs.com/svg.latex?\frac{n_{1}}{n}) | ![](https://latex.codecogs.com/svg.latex?\frac{n_{2}}{n}) | ...    | ![](https://latex.codecogs.com/svg.latex?\frac{n_{k}}{n}) |

Это **статистическое распределение выборки**.

![](https://latex.codecogs.com/svg.latex?\sum_{i=1}^{k}n_{i}=n)

![](https://latex.codecogs.com/gif.latex?\sum_{i=1}^{k}p_{i}^{*}=1)

На практике даже такие таблицы трудно обозримы, а информация в них бывает лишней при решении. Поэтому данные укрупняют.

Расположим данные на оси.
Разобьем интервал от ![](https://latex.codecogs.com/svg.latex?x_{1}) до ![](https://latex.codecogs.com/svg.latex?x_{k}) на разряды по S штук

![](../../images/Mathematical-statistics/ticket03.png)

![](https://latex.codecogs.com/svg.latex?y_{1}<y_{2}<...<y_{s}<y_{s&plus;1})

![](https://latex.codecogs.com/svg.latex?y_{1}\leq&space;x_{1})

![](https://latex.codecogs.com/svg.latex?y_{s&plus;1}\geq&space;x_{k})

Дальше считают сколько элементов выборки попало в каждый разряд.

| Разряды                                                             | ![](https://latex.codecogs.com/svg.latex?[y_{1},y_{2}]) | ![](https://latex.codecogs.com/svg.latex?[y_{2},y_{3}]) | ... | ![](https://latex.codecogs.com/svg.latex?[y_{s},y_{s+1}]) |
|---------------------------------------------------------------------|---------------------------------------------------------|---------------------------------------------------------|-----|-----------------------------------------------------------|
| ![](https://latex.codecogs.com/svg.latex?L_{i})                     | ![](https://latex.codecogs.com/svg.latex?L_{1})         | ![](https://latex.codecogs.com/svg.latex?L_{2})         | ... | ![](https://latex.codecogs.com/svg.latex?L_{s})           |
| ![](https://latex.codecogs.com/svg.latex?L_{i}^{*}=\frac{L_{i}}{n}) | ![](https://latex.codecogs.com/svg.latex?L_{1}^{*})     | ![](https://latex.codecogs.com/svg.latex?L_{2}^{*})     | ... | ![](https://latex.codecogs.com/svg.latex?L_{s}^{*})       |

![](https://latex.codecogs.com/svg.latex?\sum_{i=1}^{s}L_{i}=n)

Иногда разряды выбираются со спецификой задачи.
Такая таблица называется **информационно статистической** или **группированным статистическим рядом**.
