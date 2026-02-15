## Variable Aleatoria
### Ejercicio 0
Imagine que desea generar listas de longitud 5, donde cada elementos es un numero entero entre 1 y 100. un ejemplo de una lista puede ser $(87, 1, 39, 100, 56)$ 
El espacio muestral $\Omega$ está compuesto por todas las posibles listas de 5 elementos que se pueden formar con números enteros en el rango de 1 a 100. Es decir $$\Omega=\{(a_{1},a_{2},a_{3},a_{4},a_{5}): 1\leq a_{i}\leq 100,i=1,2,3,4,5\}$$
* **a -** Supongamos que cada elementos de la lista tiene la misma probabilidad de ser seleccionado. Escriba la función de probabilidad de $P$ asociada a este experimento. Es decir determine la probabilidad de generar una lista especifica en $\Omega$.$$P(a)=\dfrac{1}{100^{5}}$$
* **b -** Defina una variable aleatoria $X$ cualquiera relacionada con este experimento.$$\begin{array}{l}
X=\text{Cantidad de veces que aparece el numero 7} \\
Y=\text{Suma de los elementos} \\
Z=\text{Hay elementos Impares}
\end{array}$$

## Funciones de Probabilidad de Masa y Función de Distribución
### Ejercicio 1
Sea $X=$ número de neumáticos de un automóvil, seleccionados al azar, que tenga baja la presión.
* **a -** ¿Cuál de la siguientes tres funciones $p(.)$ es una función de probabilidad de masa para $X$? Justifique.$$\begin{array}{c}
\begin{array}{|l|ccccc|}\hline
x & 0 & 1 & 2 & 3 & 4 \\\hline
p(x) & 0,3 & 0,2 & 0,1 & 0,05 & 0,05 \\\hline
p(x) & 0,4 & 0,1 & 0,1 & 0,1 & 0,3 \\\hline
p(x) & 0,4 & 0,1 & 0,2 & 0,1 & 0,3  \\\hline
\end{array} \\\quad \\
\begin{array}{l}
\text{La segunda fila es la unica funcion de probabilidad valida porque} \\
\displaystyle\sum_{i}p(x_{i})=0,4 +0,1+0,1+0,1+0,3=1\wedge 0\leq x_{i}\leq 1 \\
\text{Ademas las funciones de la fila 1 y 3, su suma es diferente de 1.} 
\end{array}
\end{array}$$

* **b -** Con la función de probabilidad de masa obtenida en (a), calcule $P(2\leq X\leq 4), P(X\leq 2)\ y\ P(X\neq 0)$.$$\begin{array}{l}
P(2\leq X\leq 4)=P(X=2) +P(X=3)+P(X=4)=0,1+0,1+0,3\\
P(2\leq X\leq 4)=0,5\\
P(X\leq 2) =P(X=0)+P(X=1)+P(X=2)=0,4+0,1+0,1\\
P(X\leq 2) = 0,6\\
P(X\neq 0) = 1-P(X=0)=1-0,4=0,6
\end{array}$$
* **c -** Obtenga la función de distribución acumulada de $X$.$$
F(t)=\begin{cases}
0 &  \text{Si } t<0 \\
0,4 & \text{Si } 0\leq t <1 \\
0,5 &  \text{Si } 1\leq t<2\\
0,6 &  \text{Si } 2\leq t<3\\
0,7 &  \text{Si } 3\leq t<4\\
1 & \text{Si } t\geq 4

\end{cases}$$
* **d -** Si $P(x)=k(5-x)$ para $X=0 ,1, 2,3, 4, 5$. ¿Cuál debe ser el valor de la constante $k$ para que p sea una función de probabilidad de masa.$$\begin{array}{l}
\sum_{i}P(x_{i})=1 \\
1=P(X=0)+P(X=1)+P(X=2)+P(X=3)+P(X=4)+P(X=5) \\
1=k(5-0)+k(5-1)+k(5-2)+k(5-3)+k(5-4)+k(5-5)=5k+4k+3k+2k+1k+0k \\
1=15k\iff k=\dfrac{1}{15}
\end{array}$$
### Ejercicio 2
Un negocio de computadoras que atiende pedidos por correo tiene seis líneas telefónica. Denotemos por $X$ el número de líneas en uso en un momento específico. Supongamos que la función de probabilidad de masa de $X$ está dada en la siguiente tabla:$$\begin{array}{|c|cccccc|}
\hline x & 0 & 1 & 2 & 3 & 4 & 5 & 6 \\
\hline p(x) & 0,10 & 0,15 & 0,20 & 0,25 & 0,20 & 0,06 & 0,04 \\
\hline
\end{array}$$
Calcule la probabilidad de cada uno de los siguientes eventos:
* **a -** $A=\text{A lo sumo tres líneas están en uso.}$ $$\begin{array}{l}
P(A)=P(X\leq 3)=P(X=3)+P(X=2)+P(X=1)+P(X=0) \\
P(A)=0,25+0,20+0.15+0,10 \\
P(A)=0,70
\end{array}$$
* **b -** $B=\text{Menos de tres líneas están en uso.}$ $$\begin{array}{l}
P(B)=P(X<3)=P(X=2)+P(X=1)+P(X=0)  \\
P(B)=0,20+0,15+0,10 \\
P(B)=0,45
\end{array}$$
* **c -** $C=\text{Por lo menos tres líneas están en uso.}$ $$\begin{array}{l}
P(C)=P(X\geq 3)=P(X=6)+P(X=5)+P(X=4)+P(X=3) \\
P(C)=0,04+0,06+0,20+0,25 \\
P(C)=0,55
\end{array}$$
* **d -** $D=\text{Entre 2 y 5 líneas están en uso.}$ $$\begin{array}{l}
P(D)=P(2\leq X\leq 5)=P(X=2)+P(X=3)+P(X=4)+P(X=5) \\
P(D)= 0,20+0,25+0,20+0,06 \\
P(D)=0,71
\end{array}$$
* **e -** $E=\text{Entre 2 y 4 líneas no están en uso.}$ $$\begin{array}{l}
E=\overline{D} \\
P(E)=P(\overline{D})=1-P(D) \\
P(E)=0,29
\end{array}$$
* **f -** $F=\text{Por lo menos 4 líneas no están en uso.}$ $$\begin{array}{l}
P(\overline{F})=P(X\geq 4)\iff \\
P(F)=1-P(X\geq 4)=1-(P(X=4)+P(X=5)+P(X=6) \\
P(F)=1-(0,20+0,06+0,04) \\
P(F)=0,7
\end{array}$$
* **g -** Obtenga la función de distribución acumulada de $X$.$$F(t)\begin{cases}
0  & si & t<0 \\
0,1 & si & 0\leq t<1 \\
0,25 & si & 1\leq t<2 \\
0,45 & si & 2\leq t<3 \\
0,7 & si & 3\leq t<4  \\
0,9 & si & 4\leq t<5 \\
0,96 & si & 5\leq t<6 \\
1 & si & t\geq 6
\end{cases}$$
### Ejercicio 3
Una compañía de seguros ofrece a sus tenedores de pólizas varias opciones diferentes para el pago de primas. Para un tenedor seleccionado al azar, sea $X=\text{número de meses entre pagos sucsivos}$. La función de distribución acumulada de $X$ es como sigue:  $$F(x)=\begin{cases}
0 & x<1 \\
0,30 &  1\leq x <3 \\
0,40 & 3\leq x<4 \\
0,45 & 4\leq x<6 \\
0,60 & 6\leq x<12 \\
1 & 12\leq x
\end{cases}$$
* **a -** ¿Cual es la función de probabilidad de masa de $X$? $$\begin{array}{|c|ccccc|}
\hline x & 1 & 3 & 4 & 6 & 12  \\
\hline p(x) & 0,30 & 0,10 & 0,05 & 0,15 & 0,4 \\
\hline\end{array}$$
* **b -** Sólo con el uso de la función de distribución acumulada, calcule $P(3\leq X\leq 6)\ y\ P(4\leq X)$ $$\begin{array}{l}
P(3\leq X\leq 6)=F(6)-F(3^{-})=0,60-0,30 \\
P(3\leq X\leq 6)=0,30 \\
 \\
P(4\leq X)=P(4\leq X\leq\infty)=(\displaystyle\lim_{ x \to \infty }F(x))-F(4^{-})=1-0,40  \\
P(4\leq X)=0,60
\end{array}$$
### Ejercicio 4
Considere un grupo de cinco personas $A ,B, C, D\ y\ E$, que son potenciales donantes de sangre. Se necesita un donante de sangre tipo $O+$ y, de estas personas , sólo $A$ y $B$ tienen dicho grupo sanguíneo. Un laboratorio tomará una muestra de sangre de cada persona y determinará en orden aleatorio el grupo sanguíneo, hasta encontrar la primera muestra $O+$. Considere la variable aleatoria $X$, que cuenta el número de determinaciones necesarias.
* **a -** Encuentre la función de probabilidad de masa de $X$.$$\begin{array}{l}
\begin{array}{|c|ccccc|}
\hline x  & 1 & 2 & 3 & 4 & 5 \\
\hline p(x) & \dfrac{2}{5} & \dfrac{3\cdot {2}}{4\cdot 5} & \dfrac{3\cdot 2\cdot 2}{5\cdot 4\cdot 3} & \dfrac{3\cdot 2}{5\cdot 4\cdot {3}} & 0 \\
\hline
\end{array}\iff \\ \\
\begin{array}{|c|ccccc|}
\hline x  & 1 & 2 & 3 & 4 & 5 \\
\hline p(x) & \dfrac{2}{5} & \dfrac{3}{10} & \dfrac{1}{5} & \dfrac{1}{10} & 0 \\
\hline
\end{array}
\end{array}$$
* **b -** Usando la función de probabilidad de masa obtenida en el ítem **a-**. Calcule la probabilidad de que el grupo sanguíneo $O+$ no sea encontrado en las dos primeras determinaciones.$$P(X\geq 3)=P(X=3)+P(X=4)+P(X=5)=0,2+0,1+0=0,3$$
### Ejercicio 5
Silvina vive en el punto $O$ del siguiente diagrama y decide salir a correr. En su recorrido, tiene cuatro posibles destinos que son $A,B,C\ y\ D$. Para decidir cual de estos lugares ir primero , lanza dos veces una moneda, y de acuerdo con el resultado , elije uno de os cuatro destinos. Una vez que Silvina llega a un lugar puede decidir entre regresar a su casa , continuar hacia uno de los dos caminos adyacentes, Cada una de estas opciones tiene una probabilidad de $1/3$. Silvina continúa corriendo entre los destinos hasta que finalmente decide regresar a su casa.
![[practico_2_ejercicio_4.excalidraw|200]]
* **a -** Sea $X=\text{número de destinos que recorre.}$ Obtenga la función de masa de $X$.
$$
p(X=x)=\left(\frac{2}{3}\right)^{x-1}\frac{1}{3}\quad\text{para }x=1,2,3,4,\dots
$$

* **b -** Obtenga la función de distribución acumulada de $X$.$$\begin{array}{l}
F(x)=\sum_{k=0}^{x-1}\frac{1}{3}\cdot\left(\frac{2}{3}\right)^{k}\iff \\
F(x)=\frac{1}{3}\sum_{k=0}^{x-1}\left(\frac{2}{3}\right)^{k}\iff \\
F(x)=\frac{1}{3}\cdot \frac{1-\left( \frac{2}{3} \right)^{{x}}}{1-\frac{2}{3}}\iff \\
F(x)=1-\left(\frac{2}{3}\right)^{x}
\end{array}$$
* **c -** Sea $Y=\text{número de segmentos que transita Silvina.}$ Obtenga la función de la probabilidad de masa de $Y$.$$\begin{array}{l}
Y=X+1 \\
P(Y=y)=P(X= y-1) \\
p(Y=y)=\left(\frac{2}{3}\right)^{y-2}\frac{1}{3}\quad\text{para }x=2,3,4,5,\dots
 \\
\end{array}$$
## Medidas características de una v. a.
### Ejercicio 6
Sea $X = \text{resultado cuando un dado honesto se hace rodar una vez.}$
* **a -** Calcule la esperanza de $X$ y de $1/X$.
$$\begin{array}{l}
p(x)=\dfrac{1}{6}\quad\text{para }x=1,2,3,4,5,6 \\
\displaystyle E(X)=\sum_{i=1}^{6}x_{i}\cdot p(x_{i})=\sum_{i=1}^{6}i\cdot\frac{1}{6} \\
\displaystyle E(X)=\frac{1}{6}\cdot \sum_{i=1}^{6}i=\frac{1}{6}\cdot\frac{6\cdot 7}{2} \\
\displaystyle E(X)=\frac{7}{2} \\\\ 
\displaystyle E\left( \frac{1}{X} \right)=\sum_{i=1}^6 \frac{1}{x_{i}}\cdot p(x_{i})=\frac{1}{6}\cdot\left( 1+\frac{1}{2}+\frac{1}{3}+\frac{1}{4}+\frac{1}{5}+\frac{1}{6} \right)=\frac{1}{6}\cdot \frac{49}{20}=\frac{49}{120} \\
\displaystyle E\left( \frac{1}{X} \right)=0,408333333
\end{array}$$
* **b -** Si antes de arrojar el dado de ofrece al tirador retirarse con $\frac{1}{3,5}$ dólares  o jugar obteniendo $h(X)=1/X$ dólares. Le conviene retirarse o jugar? Justifique. 
$$
\begin{array}{l}
\displaystyle\text{Le conviene seguir jugando, debido a que la esperanza de } h(X) = \frac{49}{120} > \frac{10}{35} \\
\text{Si sigue jugando es esperable que gane mas}
\end{array}
$$
### Ejercicio 7
Un distribuidor de aparatos electrodomésticos vende tres modelos de diferentes congeladores verticales con capacidad de 13,5; 15,9 y 19,1 pies cúbicos de espacio de almacenaje, respectivamente. Sea $X=\text{la cantidad de espacio de almacenaje comprado por un cliente que va a comprar un congelador.}$ Supongamos  que $X$ tiene la siguiente función de probabilidad de masa:
$$
\begin{array}{|c|ccc|}
\hline x & 13,5 & 15,9 & 19,1 \\
\hline p(x) & 0,2 & 0,5 & 0,3 \\
\hline
\end{array}
$$
* **a -** Calcule $E(X), E(X^{2})\ y\ V(X)$
$$
\begin{array}{l}
\displaystyle E(X)=\sum_{i=1}^{n}x_{i}\cdot p(x_{i})=13,5\cdot 0,2+15,9\cdot 0,5+ 19,1\cdot 0,3 \\
E(X)=16,38 \\
\displaystyle E(X^2)=\sum_{i=1}^{n}x_{i}^2\cdot p(x_{i})=13,5^2\cdot 0,2+15,9^2\cdot 0,5+19,1^2\cdot 0,3 \\
E(X^2)=272,298 \\
V(X)= E(X^2)-E(X)^{2}=3,9936
\end{array}
$$
* **b -** Si el precio de un congelador que tiene una capacidad de $X$ pies cúbicos es de $25X-8,5$. ¿Cuál es la esperanza y varianza del precio pagado por un cliente que va a comprar un congelador?
$$
\begin{array}{l}
Y=25X-8,5 \\
E(Y)=E(25X-8,5)=25\cdot E(X)-8,5 \\
E(Y)=401 \\
V(Y)=V(25X-8,5)=25^2\cdot V(X) \\
V(Y)=2496
\end{array}
$$
* **c -** Suponga que mientras la capacidad nominal de un congelador es $X$. La capacidad real es $h(X)=X-0,01X^{2}$. ¿Cuál es la capacidad real esperada del congelador comprada por un cliente?
$$\begin{array}{l}
E(h(X))=E(X-0,01X^2)=E(X)-0,01\cdot E(X^2)=16,38-0,01\cdot 272,298 \\
E(h(X))=13,65702
\end{array}
$$
### Ejercicio 8 
Considere la variable aleatoria de $X$ del ejercicio 4.
* **a -** Encuentre la esperanza y la desviación estándar de $X$.
$$
\begin{array}{l}
\displaystyle E(X)=\sum_{i=1}^5 x_{i}\cdot p(x_{i})=1\cdot \frac{2}{5}+2 \cdot \frac{3}{10}+3\cdot \frac{1}{5}+4\cdot \frac{1}{10}+5\cdot 0 \\
E(X)=2 \\
\displaystyle E(X^2)=\sum_{i=1}^{5}x_{i}^2\cdot p(x_{i})=1^2\cdot \frac{2}{5}+2^2 \cdot \frac{3}{10}+3^2\cdot \frac{1}{5}+4^2\cdot \frac{1}{10}+5^2\cdot 0 \\
E(X^2)=5 \\
V(X)=E(X^2)-E(X)^2=5-4 \\
V(X)=1 \\
\sigma^2=V(X) \\
\sigma=\sqrt{ V(X) }=\sqrt{ 1 } \\
\sigma = 1
\end{array}
$$
* **b -** Si la determinación del grupo sanguíneo de cada muestra le cuesta al laboratorio 200$. ¿Cual es el costo esperado para realizar las determinaciones necesarias hasta encontrar el donante?. ¿Y la varianza del costo?.
$$
\begin{array}{l}
Y =200X \\
E(Y)=E(200X)=200\cdot E(X) \\
E(Y)=400 \\ \\
V(Y)=V(200X)=200^2\cdot V(X) \\
V(Y)=40000
\end{array}
$$
## Distribuciones de una variable aleatoria discreta  
### Ejercicio 9
Suponga que sólo el $20\%$ de los automovilistas se detiene por completo en un cruce donde hay un semáforo con la luz intermitente en todas las direcciones, cuando no haya otros automóviles visibles.
* **a -** ¿Cuál es la probabilidad de que 20 automovilistas , seleccionados ala azar, que lleguen al cruce en estas condiciones:
$$
\begin{array}{l}
\displaystyle P(X=x)=\binom{n}{x}\cdot p^x\cdot (1-p)^{n-x} \\
\displaystyle P(X=x)=\binom{20}{x}\cdot 0,2^x\cdot 0,8^{20-x}
\end{array}
$$
	* **$i$ -** a lo sumo 5 se detengan por completo.
$$\begin{array}{l}
\displaystyle P(X\leq 5)=\sum_{k=0}^{5}\binom{20}{k}\cdot 0,2^k\cdot 0,8^{20-k} \\
P(X\leq 5)=0.80420
\end{array}$$
	* **$ii$ -** exactamente 5 se detengan por completo.
$$
\begin{array}{l}
\displaystyle P(X=5)=\binom{20}{5}\cdot 0,2^5\cdot 0,8^{20-5} \\
P(X=5)=0,17456
\end{array}
$$
	* **$iii$ -** por lo menos 5 se detengan por completo.
$$
\begin{array}{l}
P(X\geq 5)=1-P(X\leq 4) \\
\displaystyle P(X\leq 4)=\sum_{k=0}^{4}\binom{20}{k}0,2^{k}0,8^{20-k} \\ \\
P(X\geq 5)=0,37036 \\
\end{array}
$$
* **b -** ¿Cuántos, de los siguientes 20 automovilistas, espera el lector que se detengan por completo? 
$$
\begin{array}{l}
E(X)=n\cdot p=20\cdot 0,2 \\
E(X)=4 
\end{array}
$$
### Ejercicio 10
Un tipo particular de raqueta de tenis se fabrica en tamaños mediano y extragrande. El $60\%$ de todos los clientes, de cierta tienda, buscan el tamaño extragrande.
* **a -** Entre los 10 clientes seleccionados al azar que desean ese tipo de raqueta, ¿Cuál es la probabilidad de que por lo menos 6 busquen el tamaño extragrande?.
$$
\begin{array}{l}
\displaystyle P(X=x)=\binom{10}{x}0,6^{x}\cdot 0,4^{10-x} \\
\displaystyle P(X\geq 6)=1-P(X\leq 5)=1-\sum_{k=0}^{5}\binom{10}{k}0,6^k\cdot 0,4^{10-k} \\
P(X\geq 6)=0.633103
\end{array}
$$
* **b -** Entre los 10 clientes seleccionados al azar que desean ese tipo de raqueta, ¿Cuál es la probabilidad de que el número de clientes que buscan el tamaño extragrande esté dentro de una desviación estándar del valor medio?.
$$
\begin{array}{l} \\
\mu=n\cdot p=10\cdot 0,6= \\
\mu= 6 \\
\sigma^{2}=V(X)=n\cdot p \cdot q=10\cdot 0,6\cdot 0,4=2,4 \\
\sigma\thickapprox1,549193338 \\
[\mu-\sigma,\mu+\sigma]\thickapprox[4,45;7,55] \\
P(4,45\leq X\leq 7,55)=P(5\leq X\leq 7) \\
\displaystyle P(5\leq X\leq 7)=\sum_{k=5}^7\binom{10}{k}\cdot0,6^{k}\cdot 0,4^{10-k} \\
P(5\leq X\leq 7)=0, 6664716288
\end{array}
$$
* **c -** La tienda tiene actualmente 6 raquetas de cada modelo. ¿Cual es la probabilidad de que los siguientes diez clientes que buscan esta raqueta puedan comprar el modelo que buscan, de entre la existencia actual?.
$$
\begin{array}{l}
\displaystyle P(4\leq X\leq 6)=\sum_{k=4}^{6}\binom{10}{k}\cdot0,6^{k}\cdot 0,4^{10-k} \\
P(4\leq X\leq 6)=0, 5629575168 \\ \\
\bullet\text{ Solo hay 6 extragrandes por lo que }X\leq 6 \\
\bullet\text{ Si se eligen menos de 4 extragrandes significa que se eligieron mas de 6 medianas } 4\leq X
\end{array}
$$
### Ejercicio 11
De todas las reparaciones hechas en aparatos de TV en cierta tienda, el $80\%$ se hace en aparatos que ya no tienen garantía. 
* **a -** Entre 20 aparatos llevados a reparación. ¿Cuál es el número esperado de aparatos que ya no tengan su garantía?
$$
\begin{array}{l}
X=\text{número de aparatos que ya no tienen garantia en 20 aparatos} \\
E(X)=n\cdot p=20\cdot 0,8 \\
E(X)=16
\end{array}
$$
* **b -** Entre 20 aparatos llevados a reparación.¿Cual es el numero esperado que tengan garantía?
$$
\begin{array}{l}
X=\text{número de aparaos que tienen garantia entre 20 aparatos} \\
E(X)=n\cdot p=20\cdot 0,2 \\
E(X)=4
\end{array}
$$
* **c -** Entre 20 aparatos llevados a reparación. ¿Cuál es la probabilidad de que al menos el $75\%$ ya no tenga garantía?
$$
\begin{array}{l}
0,75\cdot 20=15 \\
\displaystyle P(X\geq 15)=\sum_{k=15}^{20}\binom{20}{k}0,8^{k}\cdot 0,2^{20-k} \\
P(X\geq 15)\thickapprox 0,8042
\end{array}
$$
* **d -** Suponga que hay 12 aparatos ahora en la tienda, de los cuales 4 tienen garantía. Si 5 de los 12 son llevados a reparación en orden aleatorio y se reparan en el mismo orden. ¿Cuál es la función de distribución de probabilidad de $X=\text{número de aparatos con garantía entre los 5 reparados}$?¿Cuánto vale $E(X)\ y\ V(X)$
$$
\begin{array}{l}
r_{1}=4 \\
r=12 \\
n=5 \\
p_{x}=P(X=x)=\dfrac{\dbinom{4}{x}\cdot\dbinom{8}{5-x}}{\dbinom{12}{5}}\quad x=0,1,2,3,4 \\
E(X)=\dfrac{n\cdot r_{1}}{r}=\dfrac{5\cdot 4}{12} \\
E(X)\thickapprox1,666666667 \\
V(X)=\dfrac{r_{1}\cdot n\cdot (r-r_{1})\cdot(r-n) }{r^2\cdot(r-1)}=\dfrac{4\cdot 5\cdot 8\cdot 7}{12^2\cdot 11} \\
V(X)\thickapprox 0,707070707
\end{array}
$$
### Ejercicio 12
Cada uno de los refrigeradores de cierto tipo ha sido devuelto a un distribuidor debido a la presencia de cierto ruido oscilante agudo , cuando esta funcionando. Supongamos que de 4 de esos 12 tienen compresores defectuosos y los otros 8 tienen problemas menos serios. Si se examina 6 refrigeradores al azar, sea $X=\text{número de de refrigeradores que tienen el compresor defectuoso entre los 6 examinados.}$
$$
\begin{array}{l}
r=12,\quad r_{1}=4\quad n=6 \\
P(X=x)=\dfrac{\dbinom{4}{x}\cdot\dbinom{8}{6-x}}{\dbinom{12}{6}}\quad x=0,1,2,3,4
\end{array}
$$
* **a -** Calcule
	* $i$ - $P(X=1)$
$$
P(X=1)=\dfrac{\dbinom{4}{1}\cdot\dbinom{8}{5}}{\dbinom{12}{6}}=\dfrac{8}{33}\thickapprox 0,2424
$$
	* $ii$ - $P(X\geq 4)$
$$
P(X\geq 4)=\dfrac{\dbinom{4}{4}\cdot\dbinom{8}{2}}{\dbinom{12}{6}}=\frac{1}{33}\thickapprox 0,0303
$$
	* $iii$ - $P(1\leq X\leq 3)$
$$
\displaystyle P(1\leq X\leq 3)=\sum _{k=1}^{3}\dfrac{\dbinom{4}{k}\cdot\dbinom{8}{6-k}}{\dbinom{12}{6}}=\frac{31}{33}\thickapprox 0,9393
$$
* **b -** ¿Cuanto vale $E(X$) y $V(X)$?
$$
\begin{array}{l}
E(X)=\dfrac{r_{1}\cdot n}{r}=\dfrac{4\cdot 6}{12} \\
E(X)=2 \\
V(X)=\dfrac{r_{1}\cdot n\cdot(r-r_{1})\cdot(r-n)}{r²\cdot(r-1)}=\dfrac{4\cdot 6\cdot 8\cdot 6}{12^2\cdot(12-1)} \\
V(X)=\dfrac{8}{11}\thickapprox 0,727272727
\end{array}
$$
### Ejercicio 13
Boca y River hacen una serie de partidos en los que si hay empate se define por penales. Suponga que $p=P(\text{gana Boca})=0,5$. Jugaran hasta que Boca gane dos partidos.
* **a -** ¿Cuál es la probabilidad de que River gane $x$ partidos?.
$$
\begin{array}{l}
P(K=k)=\dbinom{k-1}{r-1}\cdot q^{k-r}\cdot p^{r}\quad k=r,r+1,r+2,\dots\\
k=x+r \quad x:\text{cantidad de partidos ganados por river}\\
r=2 \\
p=0,5 \\
q=0,5 \\
P(X=x)=\dbinom{x+1}{1}\cdot 0,5^{x}\cdot 0,5^{2}\quad x=0,1,2,3,\dots
\end{array}
$$
* **b -** ¿Cuál es la probabilidad de que se jueguen 4 partidos?.
$$
\begin{array}{l}
P(K=k)=\dbinom{k-1}{1}\cdot0,5^{k-2}\cdot0,5^{2}\quad k=2,3,4,\dots\\
P(K=k)=(k-1)\cdot0,5^{k}\quad k=2,3,4,\dots \\
P(K=4)=(4-1)\cdot 0,5^{4}\\
P(K=4)=0,1875
\end{array}
$$
* **c -** ¿Cuál es la probabilidad de que de jueguen a lo sumo 4 partidos?.
$$
\begin{array}{l}
\displaystyle P(K\leq 4)=\sum_{k=2}^{4}(k-1)\cdot0,5^{k-2}\cdot0,5^{2}\\
P(K\leq 4)=\dfrac{11}{16}=0,6875 
\end{array}
$$
* **d -** ¿Cuántos partidos se esperaría que gane River?. ¿Cuántos partidos se esperaría que se jueguen? .
$$
\begin{array}{l}
E(K)=\dfrac{r}{p}=\dfrac{2}{0,5}=4 \\
K=X+r\iff X=K-r \\
E(X)=E(K-r)=E(K)-r=4-2 \\
E(X)=2
\end{array}
$$
### Ejercicio 14
Suponga que $X=$ números de tornados observados, en una región particular, durante un periodo de un año tiene una distribución Poisson con $\lambda=8$.
* **a -** Calcule: 
	* **$i$ -** $P(X\leq5)$
$$
\begin{array}{l}
\displaystyle P(X\leq5)=\sum_{k=0}^{5}\frac{e^{-\lambda}\cdot \lambda^{k}}{k!} \\
P(X\leq5)=0.1912
\end{array}
$$
	* $ii$ - $P(6\leq X\leq 9)$
$$
\begin{array}{l}
\displaystyle P(6\leq X\leq 9)=\sum_{k=6}^{9}\frac{e^{-\lambda}\cdot \lambda^{k}}{k!} \\
P(6\leq X\leq 9)=0.52539
\end{array}
$$
	* $iii$ - $P(10\leq X)$
$$
\begin{array}{l}
\displaystyle P(10\leq X)=1-P(X\leq 9)=1-\sum_{k=0}^{9}\frac{e^{-\lambda}\cdot \lambda^{k}}{k!}  \\
P(10\leq X)=0.28337
\end{array}
$$
	* $iv$ - $P(X\geq 1)$
$$
\begin{array}{l}
\displaystyle P(X\geq 1)=1-P(X=0)=1-\frac{e^{-8}\cdot \lambda^{0}}{0!}=1-\frac{1}{e^{8}} \\
P(X\geq 1)\thickapprox0,9997
\end{array}
$$

* **b -** ¿Cuántos tornados se puede esperar que se observen durante un periodo de un año? ¿Cuál es la desviación estándar de $X$?
$$
\begin{array}{l}
E(X)=\lambda=8 \\
\sigma^{2}=V(x)=\lambda \\
\sigma=\sqrt{\lambda}=\sqrt{ 8 }=2\cdot \sqrt{2} \\
\sigma \thickapprox2,8284
\end{array}
$$
### Ejercicio 15
Un establecimiento tiene dos entradas. Los coches llegan por hora a la entrada $I$ de acuerdo con una distribución Poisson de parámetro $\lambda=3$ y a la entrada $II$ de acuerdo con una distribución Poisson con parámetro $\lambda=4$. ¿Cuál es la probabilidad de que 3 coches lleguen al estacionamiento durante una hora dada? (Se supone que los números de coches que llegan a las dos entradas son independientes).
$$
\begin{array}{l}
X=X_{I}+X_{II} \\
\lambda=\lambda_{I}+\lambda_{II} \\
\lambda=7 \\
P(X=x)=\dfrac{e^{-\lambda}\cdot\lambda^{x}}{x!} \\
P(X=3)=\dfrac{e^{-7}\cdot7^{3}}{3!} \\
P(X=3)=0,052129252
\end{array}
$$
### Ejercicio 16
Se supone que el número de defectos Y (por cm) de la producción diaria de cierto tipo de soga tiene una distribución de Poisson con una media de 2. Cuando se vende la soga, la ganancia por cm está dada por $X=50-2Y-2Y^{2}$. Dé la ganancia esperada por cm.
$$
\begin{array}{l}
E(Y)=2:\quad V(Y)=2 \\
V(Y)=E(Y^{2})-E(Y)^{2}\iff \\
E(Y)^{2}=V(Y)+E(Y)^{2} \\
E(Y)^{2}=2+2^{2} \\
E(Y)^{2}=6 \\
E(X)=E(50-2Y-2Y^{2})=50-2E(Y)-2E(Y^{2})=50-2\cdot 2-2\cdot 6 \\
E(X)=34
\end{array}
$$
### Ejercicio 17
* **a -** Halle la esperanza y varianza para una variable aleatoria con distribución Hipergeométrica.
$$
\begin{array}{l}
\displaystyle E(X)=\sum_{i=1}^{n}x\cdot p(x)=\sum_{i=1}^{n}x\cdot\frac{\dbinom{r_{1}}{x}\cdot\dbinom{r-r_{1}}{n-x}}{\dbinom{r}{n}}=\sum_{i=1}^{n}x\dfrac{\dfrac{r_{1}!}{x!(r_{1}-x)}\cdot\dfrac{(r-r_{1})!}{(n-x)!\cdot((r-r_{1})-(n-x))}}{\dfrac{r!}{n!\cdot(r-n)!}} \\
\end{array}
$$
* **b -** Halle la esperanza y varianza para una variable aleatoria con distribución Binomial Negativa.
