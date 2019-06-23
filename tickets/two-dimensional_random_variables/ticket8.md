# 8. Основные числовые характеристики двумерной с.в. и формулы для нахождения центра рассеивания, величины разброса по осям, ковариации и корреляционной матрицы.

## Центр разброса (рассеивания)

Точка на плоскости с координатами ![](https://latex.codecogs.com/svg.latex?(M\xi_1,M\xi_2))

![](../../images/two-dimensional_random_variables/ticket8-1.png)

## Величина разброса

Для вычисления ![](https://latex.codecogs.com/svg.latex?D\xi_i) удобно найти отдельно закон распределения для ![](https://latex.codecogs.com/svg.latex?\xi_1) и для ![](https://latex.codecogs.com/svg.latex?\xi_2). Потом взять формулы для одномерных с.в.

![](https://latex.codecogs.com/svg.latex?D\xi_1) - по OX.
![](https://latex.codecogs.com/svg.latex?D\xi_2) - по OY.

## Ковариация с.в.

![](https://latex.codecogs.com/svg.latex?COV%28%5Cxi_1%2C%5Cxi_2%29%3DM%5C%7B%28%5Cxi_1-M%5Cxi_1%29%28%5Cxi_2-M%5Cxi_2%29%5C%7D%28definition%29%3DM%28%5Cxi_1%5Cxi_2%29-M%5Cxi_1M%5Cxi_2%28convenient%20formula%29)

![](https://latex.codecogs.com/svg.latex?M%28%5Cxi_1%5Cxi_2%29%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%20%5Csum_i%5Csum_jx_iy_jp_%7Bij%7D%2C%20%28%5Cxi_1%2C%5Cxi_2%29-discrete%5C%5C%20%5Cint_%7B-%5Cinfty%7D%5E%7B&plus;%5Cinfty%7D%5Cint_%7B-%5Cinfty%7D%5E%7B&plus;%5Cinfty%7Dxyf_%7B%5Cxi_1%5Cxi_2%7D%28x%2Cy%29%2C%28%5Cxi_1%2C%5Cxi_2%29-continuous%20%5Cend%7Bmatrix%7D%5Cright.)

## Корреляция (нормированная ковариация)

![](https://latex.codecogs.com/svg.latex?corr(\xi_1,\xi_2)=\frac{COV(\xi_1,\xi_2)}{\sqrt{D(\xi_1)}\sqrt{D(\xi_2)}}=\frac{COV(\xi_1,\xi_2)}{\sigma\xi_1\sigma\xi_2})

Величина corr характеризует степень _линейной_ зависимости между ![](https://latex.codecogs.com/svg.latex?\xi_1) и ![](https://latex.codecogs.com/svg.latex?\xi_2)

### Свойства корреляции

1. ![](https://latex.codecogs.com/svg.latex?\left&space;|&space;corr&space;\right&space;|&space;\leqslant&space;1)
2. Пусть ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) связаны __жесткой (функциональной) линейной зависимостью.
  ![](https://latex.codecogs.com/svg.latex?\xi_2=a\xi_1&plus;b,&space;a,b&space;\in&space;R,&space;a\neq0)

  В этом случае ![](https://latex.codecogs.com/svg.latex?corr(\xi_1,\xi_2)) будет максимальна по модулю.
  ![](https://latex.codecogs.com/svg.latex?corr%28%5Cxi_1%2C%5Cxi_2%29%3D%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%201%2C%20a%3E0%5C%5C%20-1%2C%20a%3C0%20%5Cend%7Bmatrix%7D%5Cright.)

3. Обратное к предыдущему свойству.
  Если ![](https://latex.codecogs.com/svg.latex?\left&space;|&space;corr&space;\right&space;|&space;=&space;1), то между ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) __обязательно__ есть жесткая линейная зависимость.

4.Если ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) независимы, то corr=0.
  ![](https://latex.codecogs.com/svg.latex?corr(\xi_1,\xi_2)=\frac{COV(\xi_1\xi_2)}{\sigma\xi_1\sigma\xi_2}=\frac{M(\xi_1\xi_2)-M(\xi_1)M(\xi_2)}{\sigma\xi_1\sigma\xi_2}=0)

5. Обратное к предыдущему свойству.
  Если corr=0, то это __не означает__, что с.в. независимы.

  - Если corr > 0, то говорят, что ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) связаны __положительной корреляцией__, т.е. при возрастании одной с.в. возрастает и другая
  - Если corr < 0, то говорят, что ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) связаны __отрицательной корреляцией__, т.е. при возрастании одной с.в. другая убывает.
  - Если corr = 0, то говорят, что ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) __некоррелированы__, т.е. между ними нет линейной зависимости.

# Корреляционная матрица

![](https://latex.codecogs.com/svg.latex?%5Cbegin%7Bpmatrix%7D%20cov%28%5Cxi_1%2C%5Cxi_1%29%26%20cov%28%5Cxi_1%2C%5Cxi_2%29%5C%5C%20cov%28%5Cxi_2%2C%5Cxi_1%29%26%20cov%28%5Cxi_2%2C%5Cxi_2%29%20%5Cend%7Bpmatrix%7D) - корреляционная матрица

![](https://latex.codecogs.com/svg.latex?cov%28%5Cxi_1%2C%5Cxi_1%29%3DM%28%28%5Cxi_1-M%5Cxi_1%29%28%5Cxi_1-M%5Cxi_1%29%29%3DM%5C%7B%28%5Cxi_1-M%5Cxi_1%29%5E2%5C%7D%3DD%5Cxi_1)

![](https://latex.codecogs.com/svg.latex?cov(\xi_2,\xi_1)=M((\xi_2-M\xi_2)(\xi_-M\xi_1))=&space;cov(\xi_1,\xi_2))

![](https://latex.codecogs.com/svg.latex?cov(\xi_2,\xi_2)) и ![](https://latex.codecogs.com/svg.latex?cov(\xi_2,\xi_1)) находятся аналогично.

![](https://latex.codecogs.com/svg.latex?%5Cbegin%7Bpmatrix%7D%20D%5Cxi_1%26%20cov%28%5Cxi_1%2C%5Cxi_2%29%5C%5C%20cov%28%5Cxi_1%2C%5Cxi_2%29%26%20D%5Cxi_2%20%5Cend%7Bpmatrix%7D)

![](https://latex.codecogs.com/svg.latex?cov(\xi_1,\xi_2)=M(\xi_1,\xi_2)-M\xi_1M\xi_2)

1. ![](https://latex.codecogs.com/svg.latex?M(\xi_1,\xi_2)=&space;M\xi_1M\xi_2&plus;cov(\xi_1,\xi_2))
  ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) - независимы ![](https://latex.codecogs.com/svg.latex?\Rightarrow&space;M(\xi_1,\xi_2)=M\xi_1M\xi_2)
2. ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) - независимы ![](https://latex.codecogs.com/svg.latex?\Rightarrow&space;D(\xi_1&plus;\xi_2)=D\xi_1&plus;D\xi_2)
  ![](https://latex.codecogs.com/svg.latex?D%28%5Cxi_1&plus;%5Cxi_2%29%3DM%5C%7B%28%5Cxi_1&plus;%5Cxi_2-M%28%5Cxi_1&plus;%5Cxi_2%29%5E2%29%5C%7D%3DM%5C%7B%28%5Cxi_1-m%5Cxi_1%29&plus;%28%5Cxi_2-M%5Cxi_2%29%5E2%5C%7D%3DM%5C%7B%28%5Cxi_1-m%5Cxi_1%5E2%29&plus;2%28%5Cxi_1-M%5Cxi_1%29%28%5Cxi_2-M%5Cxi_2%29&plus;%28%5Cxi_2-M%5Cxi_2%29%5E2%5C%7D%3DM%5C%7B%28%5Cxi_1-m%5Cxi_1%5E2%29%5C%7D&plus;2M%5C%7B%28%5Cxi_1-M%5Cxi_1%29%28%5Cxi_2-M%5Cxi_2%29%5C%7D&plus;M%5C%7B%28%5Cxi_2-M%5Cxi_2%29%5E2%5C%7D%3DD%5Cxi_1&plus;D%5Cxi_2&plus;2cov%28%5Cxi_1%5C%2C%5Cxi_2%29)
3. ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) - зависимы
  ![](https://latex.codecogs.com/svg.latex?D(\xi_1&plus;\xi_2)=D\xi_1&plus;D\xi_2&plus;cov(\xi_1\,\xi_2))
