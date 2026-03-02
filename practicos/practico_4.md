## Ejercicios conceptuales de probabilidad conjunta
### Ejercicio 1 
Cierto supermercado tiene una caja rápida y una común. Sea $X_{1}$ el número de clientes que están en espera en la caja común en un momento particular del día, y $X_{2}$ el numero de clientes que están en espera en la caja rápida al mismo tiempo. Si la función de probabilidad conjunta de $X_{1}$ y $X_{2}$ esta dada por:
$$
\begin{array}{|c|cccc|}
\hline X_{1}/X_{2} & 0 & 1 & 2 & 3  \\
\hline 0 & 0.08 & 0.07 & 0.04 & 0.00  \\
1 & 0.06 & 0.15 &  0.05 & 0.04 \\
2 & 0.05 & 0.04 & 0.10 & 0.06  \\
3 & 0.00 & 0.03 & 0.04 & 0.07 \\
4 & 0.00 & 0.01 & 0.05 & 0.06 \\
\hline
\end{array}
$$
* **a -** ¿Cuál es la probabilidad de que haya exactamente un cliente en cada caja?
$$
P(X_{1}=1,X_{2}=2)=0.15
$$
* **b -** Cuál es la probabilidad de que haya exactamente el mismo número de clientes en dos líneas de espera?
$$
\sum_{i=0}^{n} P(X_{1}=i,X_{2}=i)=0.08+0.15+0.10+0.07=0,40
$$
* **c -** Sea $A$ el evento de que haya por lo menos dos clientes más en una linea de espera que en la otra. ¿Cuál es la probabilidad del evento $A$?
$$
\begin{align}
P(A)= & P(X_{1}=2,X_{2}=0)+P(X_{1}=3,X_{2}=1)+P(X_{1}=3,X_{2}=0)+ \\
 & P(X_{1}=4,X_{2}=2)+P(X_{1}=4,X_{2}=1)+P(X_{1}=4,X_{2}=0)+ \\
 & P(X_{1}=0,X_{2}=2)+P(X_{1}=0,X_{2}=3)+P(X_{1}=1,X_{2}=3) \\
 P(A)=&0.05+0.03+0.00+0.05+0.01+0.00+0.04+0.04+0.00 \\
 P(A)=&0.22 
\end{align}
$$
* **d -** ¿Cuál es la probabilidad de que el número total de clientes de las dos lineas de espera sea exactamente cuatro?¿Y por lo menos 4?
$$
\begin{array}{l}
P(Y=4)=P(X_{1}=1,X_{2}=3)+P(X_{1}=2,X_{2}=2)+P(X_{1}=3,X_{2}=1)+P(X_{1}=4,X_{2}=0)\\
P(Y=4)=0.04+0.010+0.03+0.00 \\
\boxed{P(Y=4)=0.17} \\
P(Y=5)=P(X_{1}=2,X_{2}=3)+P(X_{1}=3,X_{2}=2)+P(X_{1}=4,X_{2}=1)=0.06+0.04+0.01 \\
P(Y=5)=0.11 \\
P(Y=6)=P(X_{1}=3,X_{2}=3)+P(X_{1}=4,X_{2}=2)=0.07+0.05 \\
P(Y=6)=0.12 \\
P(Y=7)=P(X_{1}=4,X_{2}=3) \\
P(Y)=0.06 \\
P(Y\geq 4)=P(Y=4)+P(Y=5)+P(Y=6)+P(Y=7)=0.17+0.11+0.12+0.06 \\
\boxed{P(Y\geq 4)=0.46}
\end{array}
$$
* **e -** Hallar las funciones de probabilidad marginales de $X_{1}$ y $X_{2}$. ¿Son estas variables independientes? Justifique su respuesta.
$$
\begin{array}{l}
\begin{array}{|c|cccc|c|}
\hline & X_{2}=0 & X_{2}=1 & X_{2}=2 & X_{2}=3 & p_{X_{1}}  \\
\hline X_{1}=0 & 0.08 & 0.07 & 0.04 & 0.00 & 0.19 \\
X_{1}=1 & 0.06 & 0.15 &  0.05 & 0.04 & 0.30 \\
X_{1}=2 & 0.05 & 0.04 & 0.10 & 0.06 & 0.25 \\
X_{1}=3 & 0.00 & 0.03 & 0.04 & 0.07 & 0.14\\
X_{1}=4 & 0.00 & 0.01 & 0.05 & 0.06 & 0.12\\
\hline p_{X_{2}} & 0.19 & 0.30 & 0.28 & 0.23 & 1 \\
\hline
\end{array} \\
p_{X_{1}}(0)=0.19\quad p_{X_{2}}(0)=0.19 \\
P(X_{1}=0,X_{2}=0)=0.08 \\
p_{X_{1}}(0)\cdot p_{X_{2}}(0)=0.19\cdot 0.19=0,0361 \\
p_{X_{1}}(0)\cdot p_{X_{2}}(0)\neq P(X_{1}=0,X_{2}=0)=0.08\therefore\ X_{1}\ y\ X_{2}\text{ no son independientes} 
\end{array}
$$
### Ejercicio 2
Dada la siguiente función:
$$
\begin{array}{l}
f(x,y)=\begin{cases}
kxy & si & 0\leq x\leq 1\text{ y }0\leq y\leq 1\text{ y }x+y\leq 1 \\
0 & \text{en cualquier otro caso}  
\end{cases} \\
\text{con k una constante positiva}
\end{array}
$$
* **a -** Determinar el valor de la constante $k$ para que sea fdpc de $(X,Y)$.
$$
\begin{align}
\displaystyle\int_{0}^{1}\int_{0}^{1-x}kxy\ dy\ dx&=\int_{0}^{1}kx \int_{0}^{1-x}y\ dy\ dx=\int_{0}^{1}kx\left[\frac{y^{2}}{2}\right]_{0}^{1-x}dx=k\int_{0}^{1}x \frac{(1-x)^{2}}{2} \\
&=\frac{k}{2}\int_{0}^{1}(x-2x^{2}+x^{3})dx=\frac{k}{2}\left[\frac{x^{2}}{2}-\frac{2x^{3}}{3}+\frac{x^{4}}{4}\right]_{0}^{1}=\frac{k}{2}\left( \frac{1}{2}-\frac{2}{3}+\frac{1}{4}\right) \\
&=k\frac{1}{24}\Longrightarrow \boxed{k=24}
\end{align}
$$
* **b -** Hallar las funciones densidad de probabilidad marginal para $X$ y de $Y$.
$$
\begin{array}{l}
\displaystyle f_{x}(x)=\int_{0}^{1-x}24yx\ dy=24x \int_{0}^{1-x}y\ dy=24x\left[ \frac{y^{2}}{2} \right]_{0}^{1-x} \\
\boxed{f_{x}(x)=12x(1-x)^{2}} \\
\displaystyle f_{y}(y)=\int_{0}^{1-y}24yx\ dx=24y\int_{0}^{1-y}x\ dx=24y\left[ \frac{x^{2}}{2} \right]_{0}^{1-y} \\
\boxed{f_{y}(y)=12y(1-y)^{2}}
\end{array}
$$
* **c -** Hallar la esperanza y varianza de $X$ y de $Y$.
$$
\begin{array}{l}
\begin{align}
\displaystyle E(X)=&\int_{0}^{1}xf_{x}(x)\ dx=\int_{0}^{1}12x^{2}(1-x)^{2}dx=12\int_{0}^{1}(x-x^{2})^{2}dx=12\int_{0}^{1}x^{2}-2x^{3}+x^{4}\\
=& 12\left[ \frac{x^{3}}{3}-\frac{x^{4}}{2}+\frac{x^{5}}{5} \right]_{0}^{1}=12\left( \frac{1}{3}-\frac{1}{2}+\frac{1}{5} \right)=12\cdot \frac{1}{30}
\end{align} \\
\boxed{E(X)=\frac{2}{5}} \\
\text{Por simetria:} \\
\boxed{E(Y)=\frac{2}{5}} \\
V(X)=E(X^{2})-E(X)^{2} \\
\displaystyle E(X^{2})=\int_{0}^{1}x^{2}f_{x}(x)dx=12\int_{0}^{1}x^{3}(1-2x+x^{2})dx=12\int_{0}^{1}(x^{3}-2x^{4}+x^{5})dx \\
\displaystyle =12\left[ \frac{x^{4}}{4} -\frac{2x^{5}}{5}+\frac{x^{6}}{6} \right]_{0}^{1}=12\left( \frac{1}{4}-\frac{2}{5}+\frac{1}{6} \right) \\
\displaystyle E(X^{2})=\frac{1}{5} \\
\displaystyle V(X)=\frac{1}{5}-\left( \frac{2}{5} \right)^{2} \\
\displaystyle\boxed{V(X)=\frac{1}{25}} \\
\text{Por simetria} \\
\displaystyle\boxed{V(Y)=\frac{1}{25}}
\end{array}
$$
* **d -** ¿Son independientes $X$ e $Y$? Justifique su respuesta.
$$
\begin{array}{l}
f_{x}(x)f_{y}(y)\neq f(x,y) \\
\text{por lo que X e Y no son independientes}
\end{array}
$$
### Ejercicio 3
Sean $X,Y$ variables aleatorias con función de densidad de probabilidad conjunta dada por:
$$
f(x)=\begin{cases}
k(x+y) & si  & 0\leq x\leq 10\text{ y }0\leq y\leq 10 \\
0 & \text{en cualquier otro caso}
\end{cases}
$$
* **a -** ¿Cuál es el valor de $k$?
$$
\begin{array}{l}
\displaystyle 1=\int_{0}^{10}\int_{0}^{10}k(x+y)\ dy\ dx=k\int_{0}^{10}\left[ xy+\frac{y^{2}}{2} \right]_{0}^{10}dx=k\int_{0}^{10}(10x+50)dx=k[5x^{2}+50x]_{0}^{10} \\
1=1000k\iff \\
\displaystyle\boxed{k=\frac{1}{1000}}
\end{array}
$$
* **b -** Calcular $P(X+Y<5)$
$$
\begin{array}{l}
\displaystyle\int_{0}^{5}\int_{0}^{5-x}\frac{1}{1000}(x+y)\ dy\ dx= \frac{1}{1000} \int_{0}^{5}\int_{0}^{5-x}(x+y)\ dy\ dx=\frac{1}{1000}\int_{0}^{5}\left[ xy+\frac{y^{2}}{2} \right]_{0}^{5-x}dx \\
\displaystyle=\frac{1}{1000}\int_{0}^{5}\left(5x-x^{2}+\frac{x^{2}}{2}+\frac{25}{2}-5x\right)dx=\frac{1}{1000}\left[\frac{25}{2}x-\frac{x^{3}}{6}\right]_{0}^{5}=\frac{1}{1000}\cdot\left(\frac{125}{2}-\frac{125}{6}\right) \\
\displaystyle =\frac{1}{1000}\cdot \frac{125}{3}=\frac{1}{24} \\
\displaystyle\boxed{P(X+Y<5)=\frac{1}{24}}
\end{array}
$$
* **c -** ¿Cuál es la probabilidad de que el valor absoluto de la diferencia entre las variables aleatorias sea lo sumo 2?
$$
\begin{array}{l}
\begin{align}
P(|X-Y|\leq 2)&=P(-2\leq X-Y\leq 2)\\
&=P(-2\leq X-Y\leq 2) \\
&=1-P(-2>X-Y)-P(2<X-Y)  \\
P(|X-Y|\leq 2)&=1-(P(Y>X+2)+P(Y<X-2))\quad\text{Por simetría}P(Y>X+2)=P(Y<X-2) \\
P(|X-Y|\leq 2)&=1-2P(Y>X+2)
\end{align} \\
\displaystyle P(Y>X+2)=\frac{1}{1000}\int_{2}^{10}\int_{0}^{x-2}(x+y)dy\ dx = \frac{1}{1000}\int_{2}^{10}\left[ xy+\frac{y^{2}}{2} \right]_{0}^{x-2}dx \\
\displaystyle =\frac{1}{1000}\int_{2}^{10} \left(x^{2}-2x+\frac{x^{2}}{2}-2x+2\right)dx =\frac{1}{1000}\left[ \frac{x^{3}}{2}-2x^{2}+2x \right]_{2}^{10} \\
\displaystyle =\frac{1}{1000}[(500-200+20)-(4-8+4)=\frac{320}{1000} \\
P(|X-Y|\leq 2)=1-2\dfrac{320}{1000} \\
P(|X-Y|)=0.36
\end{array}
$$
* **d -** Hallar las funciones de densidad marginales de $X$ e $Y$. ¿Son estas variables independientes? Justifique su respuesta.
$$
\begin{array}{l}
\displaystyle f_{x}(x)=\int_{0}^{10} \frac{1}{1000}(x+y)dy=\frac{1}{1000}\left[ xy+\frac{y^{2}}{2}\right]_{0}^{10}=\frac{1}{1000}\left(10x+\frac{100}{2}\right) \\
\boxed{f_{x}(x)=\frac{1}{100}x+\frac{1}{20}} \\
\text{De forma analoga} \\
\boxed{f_{y}(y)=\frac{1}{100}y+\frac{1}{20}} \\
\text{Luego }f_{x}(x)\cdot f_{y}(y)= \dfrac{xy+5x+5y+25}{10000}\neq \dfrac{x+y}{1000}=f(x,y) \\
\text{Por lo que estas vriables no son independientes}
\end{array}
$$
* **e -** Calcular $Cov(X,Y)$.
$$
\begin{array}{l}
\displaystyle E(X)=\int_{0}^{10}xf_{X(x)}dx=\int_{0}^{10} \left(\frac{x^{2}}{100}+\frac{1}{20}x
\right)\ dx=\left[ \frac{x^{3}}{300}+\frac{x^{2}}{40} \right]_{0}^{10} \\
\displaystyle E(X)=\frac{70}{12} \\
\text{De forma analoga} \\
\displaystyle E(Y)=\frac{35}{6} \\
\displaystyle E(X)\cdot E(Y)=\frac{1225}{36} \\
\displaystyle E(XY)=\int_{0}^{10}\int_{0}^{10}(xy)f(x,y)dy\ dx=\frac{1}{1000}\int_{0}^{10}\int_{0}^{10}(x^{2}y+xy^{2})dy\ dx \\
\displaystyle =\frac{1}{1000}\int_{0}^{10}\left[ \frac{(xy)^{2}}{2}+\frac{xy^{3}}{3} \right]_{0}^{10} dx=\frac{1}{1000}\int_{0}^{10} \left(\frac{100x^{2}}{2}+\frac{1000x}{3}\right)dx \\
\displaystyle=\frac{1}{1000}\left[\frac{100x^{3}}{6}+\frac{1000x^{2}}{6}\right]_{0}^{10}=\frac{1}{10^{3}}\left( \frac{10^{5}}{6}+\frac{10^{5}}{6}\right)=\frac{100}{3} \\
E(XY)=\dfrac{100}{3} \\
\displaystyle Cov(X,Y)= E(XY)-(E(X)E(Y))=\frac{100}{3}-\frac{1225}{36}\\
\boxed{Cov(X,Y)=-\frac{25}{36}}
\end{array}
$$

## Aplicaciones de probabilidad conjunta
### Ejercicio 4
Un profesor entrega un artículo largo a una mecanografía y otro más corto a otra. Sea $X$ el número de errores de mecanografía del primer articulo e $Y$ el número de errores de mecanografía del segundo artículo. Suponga que $X$ e $Y$ son variables aleatorias con distribución Poisson de parámetros $\lambda_{1}$ y $\lambda_{2}$ respectivamente.
* **a -** Dar la probabilidad de masa conjunta de $(X,Y)$.
$$
\begin{align}  
&p(x,y)=P(X=x\cap Y=y)=P(X=x)\cdot P(Y=y)=\frac{\lambda_{1}^{x}e^{-\lambda_{1}}}{x!} \cdot \frac{\lambda_{2}^{y}e^{-\lambda_{2}}}{y!} \\
&p(x,y)=\frac{\lambda_{1}^{x}\lambda_{2}^{y}e^{-(\lambda_{1}+\lambda_{2})}}{x!y!}
\end{align}
$$
* **b -** ¿Cuál es la probabilidad de que a lo sumo se cometa un error entre los dos artículos?
$$
\begin{aligned}
&\text{usando el punto c}\\
&P(X+Y\leq 1)=P(X+Y=0)+P(X+Y=1)=\frac{e^{-(\lambda_{1}+\lambda_{2})}(\lambda_{1}+\lambda_{2})^{0}}{0!}+\frac{e^{-(\lambda_{1}+\lambda_{2})}(\lambda_{1}+\lambda_{2})^{1}}{1!}\\
&P(X+Y\leq 1)=e^{-(\lambda_{1}+\lambda_{2})}(1+\lambda_{1}+\lambda_{2})
\end{aligned}
$$
* **c -** Obtener una expresión general para la probabilidad de que el número total de errores entre ambos artículos sea $m$ cualquier número entero no negativo
$$
\begin{aligned}
P(X+Y=m)&=\sum_{k=0}^{m}P(X=k\cap Y=m-k)=\sum_{k=0}^{m} \left(\frac{\lambda_{1}^{k}e^{-\lambda_{1}}}{k!}\right)\cdot\left( \frac{\lambda_{2}^{m-k}e^{-\lambda_{2}}}{(m-k)!}\right)\\
&=\frac{e^{-(\lambda_{1}+\lambda_{2})}}{m!}\sum_{k=0}^{m} \frac{m!}{k!(m-k)!}\lambda_{1}^{k}\lambda_{2}^{m-k}=\frac{e^{-(\lambda_{1}+\lambda_{2})}}{m!}\sum_{k=0}^{m}\binom{m}{k}\lambda_{1}^{k}\lambda_{2}^{m-k}\\
&=\frac{e^{-(\lambda_{1}+\lambda_{2})}(\lambda_{1}+\lambda_{2})^{m}}{m!}\\
&\boxed{X+Y\thicksim Poisson(\lambda_{1}+\lambda_{2})}
\end{aligned}
$$
### Ejercicio 5
Una persona tiene dos bombillas para una lámpara en particular. Sea $X$ e $Y$ el tiempo de duración, en miles de horas, para la primera y segunda bombilla respectivamente. Suponga que $X$ e $Y$ son variables aleatorias independientes e idénticamente distribuidas, con distribución exponencial de parámetro $\lambda=1$.
* **a -** Dar la función de densidad de probabilidad conjunta de $(X,Y)$.
$$
\begin{align}
p(x,y)&=P(X=x\cap Y=y)=f_{X}(x)\cdot f_{Y}(y)=\lambda e^{-\lambda x}\cdot \lambda e^{-\lambda y} \\
&=e^{-(x+y)} \\
\end{align}
$$
* **b -** ¿Cuál es la probabilidad de que ambas bombillas duren a lo sumo mil horas?
$$
\begin{align}
P(X\leq 1\cap Y\leq 1)&=\int_{0}^{1} \int_{0}^{1}p(x,y)dy\ dx=\int_{0}^{1}\int_{0}^{1}e^{-(x+y)}dy\ dx  \\
&=\int_{0}^{1}e^{-x}\int_{0}^{1}e^{-y}\ dy\ dx=\int_{0}^{1}e^{-x}[-e^{-y}]_{0}^{1}\ dx=\int_{0}^{1}e^{-x}(-e^{-1}-(-1))\ dx \\
&=(1-e^{-1})\int_{0}^{1}e^{-x}dx=(1-e^{-1})[-e^{-x}]_{0}^{1}=(1-e^{-1})^{2}=1-\frac{2}{e}+\frac{1}{e^{2}} \\
&=0,3996
\end{align}
$$
* **c -** ¿Cuál es la probabilidad de que la duración total entre las bombillas sea a lo sumo 2000 horas?
$$
\begin{align}
P(X+Y\leq 2)&=\int_{0}^{2}\int_{0}^{2-x}e^{-x}e^{-y}dy\ dx=\int_{0}^{2}e^{-x}[-e^{-y}]_{0}^{2-x}dx=\int_{0}^{2}e^{-x}(-e^{x-2}+1)dx \\
&=\int_{0}^{2}(e^{-x}-e^{-2})\ dx=[-e^{-x}-xe^{-2}]_{0}^{2}=-e^{-2}-2e^{-2}+1=-3e^{-2}+1 \\
&=1-\frac{3}{e^{2}}\thickapprox 0,5939
\end{align}
$$
## Ejercicios MathLovers
### Ejercicio 6
Si $X$ e $Y$ son variables aleatorias independientes con $X_{i}\thicksim\mathcal B(n_{i},p)$ Para $i=1,2$, probar que $X_{1}+X_{2}\thicksim\mathcal B(n_{1}+n_{2},p)$. Ayuda: Puede utilizar la identidad de Vandermonde.
$$
\begin{align}
\binom{m+n}{r}=\sum_{k=0}^{r}\binom{m}{k}\binom{n}{r-k}
\end{align}
$$
$$
\begin{align}
X_{1}=X\quad X_{2}&=Y\\
P(X+Y=z)&=\sum_{k=0}^{z}P(X=k)\cdot P(Y=z-k)= \sum_{k=0}^{z}\binom{m}{k}p^{k}(p-1)^{m-k}\binom{n}{z-k}p^{z-k}(1-p)^{n-z+k} \\
&=p^{z}(p-1)^{n+m-z}\sum_{k=0}^{z}\binom{m}{k}\binom{n}{z-k} \\
&=p^{z}(p-1)^{n+m-z}\binom{m+n}{z} \quad\therefore QED
\end{align}
$$
### Ejercicio 7
* **a -** Demuestre que si $X$ e $Y$ son variables aleatorias independientes, entonces $E(XY)=E(X)E(Y)$. (Considere los casos en que las variables aleatorias son ambas discretas o ambas continuas).
$$
\begin{array}{l}
\text{Variables Aleatorias Discretas} \\
\begin{aligned}
E(X)E(Y)&=\sum_{i}x_{i}P(X=x_{i})\cdot \sum_{j}y_{j}P(Y=y_{j}) \\
&=\sum_{i}\sum_{j}x_{i}y_{j}P(X=x_{i},Y=y_{j}) \\
&=E(XY)\quad\therefore QED 
\end{aligned} \\
\text{Variables aleatorias Continuas} \\
\begin{aligned}
E(X)E(Y)&=\int_{-\infty}^{\infty}x\cdot f_{X}(x)\ dx\int_{-\infty}^{\infty}y\cdot f_{Y}(y)\ dy \\
&=\int_{-\infty}^{\infty}\int_{-\infty}^{\infty}xy\cdot f_{X,Y}(x,y)\ dy\ dx \\
&=E(XY)
\end{aligned}
\end{array}
$$
* **b -** Un topógrafo desea marcar en el terreno un cuadrado de longitud $L$. Sin embargo, debido a un error de medición, traza un rectángulo donde los lados norte-sur tiene una longitud $X$ y los lados este-oeste tienen longitud $Y$. Suponga que $X$ e $Y$ son independientes y que cada una tiene una distribución uniforme en el intervalo $[L-a,L+a]$(donde $0<a<L$). ¿Cuál es el área esperada del rectángulo resultante?  
$$
\begin{array}{l}
E(X)=\dfrac{L-a+L+a}{2}=L\\
E(Y)=\dfrac{L-a+L+a}{2}=L \\
E(XY)=E(X)E(Y)=L^{2} \\
\boxed{E(XY)=L^{2}}
\end{array}
$$
### Ejercicio 8
Suponga que la función de probabilidad de masa conjunta de $(X,Y)$ está dada por la siguiente tabla:
$$
\begin{array}{|c|ccc|}
\hline X/Y & -1 & 0 & 1 \\
\hline -1 & a & b & a \\
0 & b & 0 & b \\
1 & a & b & a \\
\hline
\end{array}
$$
donde se cumple que $a+b=1/4$
* **a -** Demostrar que $E(XY)=E(X)E(Y)$ y luego $\rho=0$.
$$
\begin{align}
E(X)&=(a+b+a)(-1)+(b+0+b)(0)+(a+b+a)(1)=(a+b+a)(1-1) \\
&=0 \\ \\
E(Y)&=(a+b+a)(-1)+(b+0+b)(0)+(a+b+a)(1)=(a+b+a)(1-1) \\
&=0 \\ \\
E(X)\cdot E(Y)&=0 \\ \\
E(XY)&=(-1)(-1)a+00b+(-1)1a+0(-1)b+0(-1)b+000+0(1)b+(-1)1a+1(0)b+(1)(1)a \\
&=a+0-a+0+0+0-a+0+a \\
&=0 \\ \\
&\boxed{E(XY)=E(X)\cdot E(Y)} \\  \\
Cov(X,Y)&=E(XY)-E(X)E(Y) \\
\rho&=\frac{Cov(X,Y)}{\sigma_{X}\sigma_{Y}} \\
&\boxed{\rho=0}
\end{align}
$$
* **b -** ¿Son las variables $X$ e $Y$ independientes?
$$
\begin{array}{l}
P(X=0,Y=0)=0 \\
P(X=0)=2b \\
P(Y=0)=2b \\
P(X=0)\cdot P(Y=0)=2b\cdot2b=4b^{2} \\
\text{si son independientes }4b^{2}=0\Longrightarrow b=0\Longrightarrow a=\dfrac{1}{4} \\
\text{caso contrario si } a\neq \frac{1}{4} \text{ No son independientes} \\
\text{Notar que si }b=0\Longrightarrow \text{hay puntos donde la probabilidad vale 0, por lo que la tabla se modificaria}
\end{array}
$$
### Ejercicio 9
Suponga que $Y_{1}$ e $Y_{2}$ son variables aleatorias tales que:
$$
\begin{array}{lllll}
E(Y_{1})=2\quad & E(Y_{2})=-1\quad & \rho(Y_{1},Y_{2})=\dfrac{1}{2\sqrt{6}}\quad & Var(Y_{1})=4\quad & Var(Y_{2})=6
\end{array}
$$
Obtener:
* **a -** $E(3Y_{1}-2Y_{2})$
$$
\begin{array}{l}
E(3Y_{1}-2Y_{2})=3E(Y_{1})-2E(Y_{2})=3\cdot 2-2\cdot (-1) \\
\boxed{E(3Y_{1}-2Y_{2})=8}
\end{array}
$$
* **b -** $Var(3Y_{1}-2Y_{2})$
$$
\begin{array}{l}
\rho(Y_{1},Y_{2})=\dfrac{Cov(Y_{1},Y_{2})}{\sigma_{Y_{1}}\sigma_{Y_{2}}}\iff Cov(Y_{1},Y_{2})=\rho(Y_{1},Y_{2})\sigma_{Y_{1}}\sigma_{Y_{2}} \\
Cov(Y_{1},Y_{2})=\dfrac{\sqrt{4}\sqrt{6}}{2\sqrt{ 6 }}=1 \\
Var(3Y_{1}-2Y_{2})=3^{2}Var(Y_{1})+(-2)^{2}Var(Y_{2})+2(3)(-2)Cov(Y_{1},Y_{2})=9\cdot 4+4\cdot 6 - 12\cdot 1 \\
\boxed{Var(3Y_{1}-2Y_{2})=48}
\end{array}
$$
* **c -** $Cov(3Y_{1}-2Y_{2},Y_{1})$
$$
\begin{array}{l}
Cov(3Y_{1}-2Y_{2},Y_{1})=Cov(3Y_{1},Y_{1})-Cov(2Y_{2},Y_{1})=3Cov(Y_{1},Y_{1})-2Cov(Y_{2},Y_{1})=3Var(Y_{1})-2 \\
\boxed {Cov(3Y_{1}-2Y_{2},Y_{1})=10}
\end{array}
$$
* **d -** $Cov(2Y_{1}+4Y_{2},5Y_{1}-Y_{2})$
$$
\begin{array}{l}
\begin{align}
Cov(2Y_{1}+4Y_{2},5Y_{1}-Y_{2})&=Cov(2Y_{1},5Y_{1}-Y_{2})+Cov(4Y_{2},5Y_{1}-Y_{2}) \\
&=Cov(2Y_{1},5Y_{1})+Cov(2Y_{1},-Y_{2})+Cov(4Y_{2},5Y_{1})+Cov(4Y_{2},-Y_{2}) \\
&=10Cov(Y_{1},Y_{1})-2Cov(Y_{1},Y_{2})+20Cov(Y_{2},Y_{1})-4(Y_{2},Y_{2}) \\
&=10Var(Y_{1})+18Cov(Y_{1},Y_{2})-4Var(Y_{2}) \\
&=10\cdot 4+18\cdot 1-4\cdot 6 \\
&=34
\end{align}
\end{array}
$$
* **e -** $E(3Y_{2}^{2})$
$$
\begin{array}{l}
Var(Y_{2})=E(Y_{2}^{2})-E(Y_{2})^{2}\iff E(Y^{2}_{2})=Var(Y_{2})+E(Y_{2})^{2}=6+(-1)^{2} \\
E(Y^{2}_{2})=7 \\
E(3Y^{2}_{2})=3E(Y^{2}_{2})=3\cdot 7 \\
E(EY_{2}^{2})=21
\end{array}
$$
* **f -** $E(3Y_{1}Y_{2})$
$$
\begin{array}{l}
Cov(Y_{1},Y_{2})=E(Y_{1}Y_{2})-E(Y_{1})E(Y_{2})\iff \\ E(Y_{1}Y_{2})=Cov(Y_{1},Y_{2})+E(Y_{1})E(Y_{2})=1+2(-1) \\
E(Y_{1}Y_{2})=-1 \\
E(3Y_{1}Y_{2})=3E(Y_{1}Y_{2})=3\cdot (-1) \\
\boxed{E(3Y_{1}Y_{2})=-3}
\end{array}
$$
* **g -** $Cov(2Y_{1}+4,-2Y_{2}-6)$
$$
\begin{array}{l}
Cov(2Y_{1}+4,-2Y_{2}-6)=2(-2)Cov(Y_{1},Y_{2})=-4\cdot 1 \\
\boxed{Cov(2Y_{1}+4,-2Y_{2}-6)=-4}
\end{array}
$$
## Importancia de ala Normal Estándar
### Ejercicio 10
Suponga que la densidad de sedimento $(g/cm)$ de un espécimen, seleccionado al azar de cierta región, está normalmente distribuida con una media de $2,65$ y una desviación estándar de $0,85$.
* **a -** Si se selecciona al azar una muestra aleatoria de 25 especímenes. ¿Cuál es la probabilidad de que el promedio muestral de la densidad del sedimento sea lo sumo 3? ¿Y que se encuentre entre 2,65 y 3?
* **b -** ¿Qué tan grande se requeriría el tamaño muestral para asegurar que la primera probabilidad calculada en $(a)$ sea por lo menos $0.99$?
