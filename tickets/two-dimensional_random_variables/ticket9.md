# 9. Свойства корреляции двух с.в.

## Корреляция (нормированная ковариация)

![](https://latex.codecogs.com/svg.latex?corr(\xi_1,\xi_2)=\frac{COV(\xi_1,\xi_2)}{\sqrt{D(\xi_1)}\sqrt{D(\xi_2)}}=\frac{COV(\xi_1,\xi_2)}{\sigma\xi_1\sigma\xi_2})

Величина corr характеризует степень _линейной_ зависимости между ![](https://latex.codecogs.com/svg.latex?\xi_1) и ![](https://latex.codecogs.com/svg.latex?\xi_2)

### Свойства корреляции

1. ![](https://latex.codecogs.com/svg.latex?\left&space;|&space;corr&space;\right&space;|&space;\leqslant&space;1)
2. Пусть ![](https://latex.codecogs.com/svg.latex?\xi_1,\xi_2) связаны __жесткой (функциональной) линейной зависимостью__.

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
