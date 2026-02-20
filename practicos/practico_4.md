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
* **b -** ¿Cuál es la probabilidad de que a lo sumo se cometa un error entre los dos artículos?
* **c -** Obtener una expresión general para la probabilidad de que el número total de errores entre ambos artículos sea $m$ cualquier número entero no negativo