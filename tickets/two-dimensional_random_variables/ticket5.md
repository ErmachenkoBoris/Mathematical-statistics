# 5. Понятие независимости двух с.в. Критерии независимости для дискретных и непрерывных с.в.

Случайные величины называются независимыми, если:

![](https://latex.codecogs.com/svg.latex?\forall&space;x,&space;\forall&space;y&space;\Rightarrow&space;F_{\xi_1\xi_2}(x,y)=F_\xi_1(x)F_\xi_2(y))

![](https://latex.codecogs.com/svg.latex?F_\xi_1(x)=F_{\xi_1\xi_2}(x,&plus;\infty);&space;F_\xi_2(y)=F_{\xi_1\xi_2}(&plus;\infty,y))

### Следствия
1. Для двумерных дискретных с.в. (__Критерий независимоссти дискретных с.в.__)

   ![](https://latex.codecogs.com/svg.latex?\xi_1:x_1,x_2,&space;\dots,&space;x_i,&space;\dots)
   ![](https://latex.codecogs.com/svg.latex?\xi_2:y_1,y_2,&space;\dots,&space;y_j,&space;\dots)

   Если ![](https://latex.codecogs.com/svg.latex?\xi_1) и ![](https://latex.codecogs.com/svg.latex?\xi_2) дискретные с.в., то для того, чтобы они были независимы, необходимо и достаточно, чтобы ![](https://latex.codecogs.com/svg.latex?\forall&space;x_i&space;\in&space;\xi_1,\forall&space;y_j&space;\in&space;\xi_2) выполнялось условие:

   ![](https://latex.codecogs.com/svg.latex?%5Cleft%5C%7B%5Cbegin%7Bmatrix%7D%20P_%7Bij%7D%3DP%28%5Cxi_1%3Dx_i%2C%5Cxi_2%3Dy_j%29%3DP%28%5Cxi_1%3Dx_i%29P%28%5Cxi_2%3Dy_j%29%5C%5C%20%5Cforall%20x_i%2C%5Cforall%20y_j%20%5Cend%7Bmatrix%7D%5Cright.)
2. Для непрерывных с.в.

  Для того, чтобы непрерывные с.в. ![](https://latex.codecogs.com/svg.latex?\xi_1) и ![](https://latex.codecogs.com/svg.latex?\xi_2) были независимы, необходимо и достаточно:

  ![](https://latex.codecogs.com/svg.latex?\forall&space;x_i,\forall&space;y_j&space;\rightarrow&space;f_{\xi_1\xi_2}(x,y)=f_\xi_1(x)f_\xi_2(y))
