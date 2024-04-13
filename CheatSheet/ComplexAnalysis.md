## Cauchy's integral theorem

Analytic 하고 simply connected (가운데 구멍이 없는) 영역의 선적분은 0이다.

$$
\oint_C f(z)dz = 0
$$


## Circle line integral

circle of radius $\rho$ around $z_0$ (이 경우 $z_0$에서 정의가 안되므로 simply connected 가 아님)

$$
\oint_C (z-z_0)^m = \begin{cases}
2\pi i & m=-1 \\
0 & m \neq -1
\end{cases}
$$

## Cauchy's integral formula
$f(z)$가 analytic 하고 simply connected 하다면
$$
 \oint_C \frac{f(z)}{(z-z_0)^{n+1}}dz=\frac{2\pi i}{n!} f^{(n)}(z_0)
$$

## Residue

pole 지점 (분모가 0인 지점) $z_0$ 에 대해 
$$
Resf(z_0) = \lim_{z\to z_0}(z-z_0)f(z)
$$

이때

$$
f'(z) = \lim_{z\to z_0} \frac{f(z)-f(z_0)}{z-z_0}
$$
인데, $f(z_0)=0$ 이면 

$$
Res f(z_0) = f'(z_0)
$$
로 쓸 수 있다.

만약 미분한 값에 pole 있다면 second order다. $m$ th-order 에 대해선

$$
Resf(z_0) = \frac{1}{(m-1)!}\lim_{z\to z_0}\frac{d^{m-1}}{dz^{m-1}}((z-z_0)^mf(z))
$$

## Residue theorem

$f(z)$ 안에 pole 지점이 $z_1,z_2,...,z_k$ 가 있을 경우 

$$
\oint_C f(z)dz = 2\pi i \sum_{j} Resf(z_j)
$$

## Residue integral

$$
\int_{-\infty}^{\infty} f(x)dx =2\pi i \sum_j Res f(z_j)
$$

## Cauchy principal value

pole 이 real axis 위에 있을 때 ($x_0$), Cauchy principal value 를 이용해 integral 을 정의할 수 있다.

$$
\int_{A}^{B} f(x)dx = \lim_{\epsilon \to 0} \left( \int_{A}^{x_0-\epsilon} f(x)dx + \int_{x_0+\epsilon}^{B} f(x)dx \right)
$$

이렇게 계산한 $\int_{A}^{B} f(x)dx $ 의 값을 Cauchy principal value 라고 한다.


## Pole at real axis

만약 pole 이 real axis 위에 있다면 principal value 는

$$
\int_{-\infty}^{\infty} f(x)dx = \pi i \sum_k Resf(x_k)
$$
이다. 그럼 복소평면에 있는 pole 과 axis 에 있는 pole 을 모두 고려한다면, 

$$
\int_{-\infty}^{\infty} f(x)dx = 2\pi i \sum_j Resf(z_j)+\pi i \sum_k Resf(x_k)
$$


## Liouville's theorem
$|f(z)|$ 가 모든 $z$에 대해 bound 되어 있다면($|f(z)|<K$), $f(z)$ 는 상수함수이다. (proof: Cauchy's inequality)
$$

$$



## Cauchy-Riemann equation

$f(z) = u(x,y)+iv(x,y)$ 가 $z=x+iy$ 근처에서 $z$ 로 미분가능하다면(analytic 하다면), $\partial u/ \partial x = \partial v/ \partial y$ 이고 $\partial u/ \partial y = -\partial v/ \partial x$ 이다. 그 역도 성립한다. (if and only if)

## Laplace's equation

f(x)=u(x,y)+iv(x,y) 가 analytic 하다면, 

$$
\nabla^2 u = \frac{\partial^2 u}{\partial x ^2}+\frac{\partial^2 u}{\partial y^2}=0
\\
\nabla^2 v = \frac{\partial^2 v}{\partial x ^2}+\frac{\partial^2 v}{\partial y^2}=0
$$

이다.

## Principal value

$$
z=re^{i\theta}
$$

principal value of $z$ is $Ln(z)=ln|z|+i\theta$