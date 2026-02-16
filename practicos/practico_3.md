## Función de densidad y distribución acumulada
### Ejercicio 1
Un  libro está disponible 2 horas para la sala de lectura de la biblioteca de una universidad. Denotemos con $X$ el tiempo de préstamo solicitado por un estudiante seleccionado al azar. Supongamos que $X$ tiene la siguiente función de probabilidad.
$$
\begin{array}{l}
f(x)\begin{cases}
\dfrac {x}{2} & 0\leq x \leq 2\\[2ex]
0 & \text{en cualquier otro caso}
\end{cases} \\
\displaystyle\int\frac{x}{2}dx=\frac{1}{2}\int x\ dx=\frac{1}{2}\cdot\frac{x^{2}}{2}=\frac{x^{2}}{4}
\end{array}
$$
* **a -** Calcular las siguientes probabilidades
	* $i$ - $P(X\leq 1)$
$$
\begin{array}{l}
\displaystyle P(X\leq 1)=\int_{0}^{1} \frac{x}{2}\ dx=\frac{x^{2}}{4}\Big|_{0}^{1}=\frac{1}{4}-\frac{0}{4}=\frac{1}{4} \\
P(X\leq 1)=0,25
\end{array}
$$
	* $ii$ - $P(0,5\leq X\leq 1,5)$
$$
\begin{array}{l}
\displaystyle P(0,5\leq X\leq 1,5)=\int_{1/2}^{3/2} \frac{x}{2}dx=\frac{x^{2}}{4}\Big|_{1/2}^{3/2}=\frac{9}{16}-\frac{1}{16}=\frac{1}{2} \\
P(0,5\leq X\leq 1,5)=0,5
\end{array}
$$
	* $iii$ - $P(1,5 < X)$
$$
\begin{array}{l}
\displaystyle P(1,5<X)=\int_{1,5}^{\infty}f(x)dx=\int_{1,5}^{2} \frac{x}{2}dx
+ \int_2^{\infty}0\ dx=\frac{x^{2}}{4}\Big|_{3/2}^{2}-0=\frac{4}{4}-\frac{9}{16}=\frac{7}{16} \\
P(1,5<X)=0,4375
\end{array}
$$
* **b -** Obtener la función de distribución acumulada de $X$.
$$
\begin{array}{l}
x < 0\quad f(t)=0,\quad F(x)=0 \\
\displaystyle 0\leq x < 2\quad F(x)=\int_{0}^{x}\frac{t}{2}dt=\frac{x^{2}}{4}  \\
\displaystyle 2\leq x\quad F(x)=\int_{0}^{2} \frac{t}{2}dt+\int_{2}^{x}0dt=1 \\
F(x)\begin{cases}
0 & x\in (-\infty,0) \\
\dfrac{x^{2}}{4} & x\in[0,2) \\
1 & x\in[2,\infty)
\end{cases}
\end{array}
$$
* **c -** Calcular $E(X),\quad V(X)\quad y\quad\sigma_{X}$
$$
\begin{array}{l}
\displaystyle E(X)=\int_{-\infty}^{\infty}x\ f(x)\ dx=\int_{0}^{2}x\cdot \frac{x}{2}\ dx=\frac{1}{2}\int_{0}^{2}x^{2}dx=\frac{1}{2}\cdot\left[ \frac{x^{3}}{3} \right]_{0}^{2}=\frac{8}{6}-\frac{0}{3}=\frac{8}{6} \\
E(X)=\dfrac{4}{3}\thickapprox 1,3333 \\
E(X)^{2}=\dfrac{16}{9}\thickapprox1,7778 \\
\displaystyle E(X^{2})=\int_{0}^{2}x^{2}\frac{x}{2}dx=\frac{1}{2}\int_{0}^{2}x^{3}dx=\frac{1}{2}\left[ \frac{x^{4}}{4} \right]_{0}^{2}=\frac{16}{8}-\frac{0}{8} \\
E(X^{2})=2 \\
V(X)=\sigma_{X}^{2}=E(X^{2})-E(X)^{2}=2-\dfrac{16}{9}=\dfrac{2}{9} \\
\sigma_{X}=\dfrac{\sqrt{2}}{3}
\end{array}
$$
* **d -** Si la persona que solicita el libro se le cobra $h(X)=X^{2}$ cuando la duración del préstamo es $X$, calcule el cobro esperado $E[h(X)]$.
$$
\begin{array}{l}
E[h(X)]=E(X^{2}) \\
\displaystyle E(X^{2})=\int_{0}^{2}x^{2}\frac{x}{2}dx=\frac{1}{2}\int_{0}^{2}x^{3}dx=\frac{1}{2}\left[ \frac{x^{4}}{4} \right]_{0}^{2}=\frac{16}{8}-\frac{0}{8} \\
E[h(X)]=2 \\
\text{Cobra 2 milanesas de pollo en efecto.}
\end{array}
$$
### Ejercicio 2
Sea $X$ una variable aleatoria con función de distribución
$$
F_{X}(x)=\begin{cases}
0 & x<0 \\
x^{2} & 0\leq x\leq 1 \\
1 & x>1
\end{cases}
$$
* **a -** Calcular:
	* $i$ - $P(X<0,2)$
$$
\begin{array}{l}
P(X<0,2)=P(0\leq X\leq 0,2)=F(0,2)-F(0)=0,2^{2}-0^{2} \\
P(X<0,2)=0,04
\end{array}
$$
	* $ii$ - $P(0,2\leq X\leq 0,8)$
$$
\begin{array}{l}
P(0,2\leq X\leq 0,8)=F(0,8)-F(0,2)=0,8^{2}-0,2^{2} \\
P(0,2\leq X\leq 0,8)=0,6
\end{array}
$$
	* $iii$ - $P(X>0,5)$
$$
\begin{array}{l}
P(X>0,5)=1-P(X\leq 0,5)=1-(F(0,5)-F(0))=1-(0,5^{2}-0^{2}) \\
P(X>0,5)=0,75
\end{array}
$$
* **b -** Hallar la función de densidad de $X$.
$$
f_{X}(x)=\begin{cases}
2x & x\in(0,1) \\
0 & \text{en cualquier otro caso}
\end{cases}
$$
### Ejercicio 3
Un profesor siempre termina su clase después de que suena el timbre y antes de que hayan transcurrido 2 minutos desde que sonó. Sea $X$ : tiempo (en minutos) que transcurre entre que suena el timbre y el término de la clase. La función de densidad de $X$ es:
$$
f(x)=\begin{cases}
kx^{2} & 0\leq x\leq 2 \\
0 & \text{en cualquier otro caso}
\end{cases}
$$
* **a -** Encuentre el valor de $k$.
$$
\begin{array}{l}
\displaystyle 1=\int_{-\infty}^{\infty}k\cdot x^{2}dx=\int_{0}^{2}k\cdot x^{2}dx=k\cdot \int_{0}^{2}x^{2}dx=k\cdot\left[ \frac{x^{3}}{3} \right]_{0}^{2}=k\cdot\frac{8}{3}\iff\\
1=\dfrac{8k}{3}\iff k=\dfrac{3}{8}
\end{array}
$$
* **b -** ¿Cuál es la probabilidad de que la clase termine antes de 1 minuto después de que suene el timbre?
$$
\begin{array}{l}
\displaystyle P(0\leq X\leq 1)=\int_{0}^{1} \frac{3x^{2}}{8}dx=\frac{3}{8}\left[ \frac{x^{3}}{3} \right]_{0}^{1}  \\
P(0\leq X\leq 1)=\dfrac{1}{8}
\end{array}
$$
* **c -** ¿Cuál es la probabilidad de que la clase continúe entre 60 y 90 segundos después de que suena el timbre?
$$
\begin{array}{l}
60s=1min;\quad 90s=1,5min \\
\displaystyle P(1\leq X\leq 1,5)=\int_{1}^{3/2} \frac{3x^{2}}{8}dx=\frac{3}{8}\left[ \frac{x^{3}}{3} \right]_{1}^{3/2}=\frac{3}{8}\cdot\left(\frac{3^{3}}{3\cdot 2^{3}}-\frac{1}{3}\right)=\frac{3}{8}\cdot\left( \frac{19}{24} \right) \\
P(1\leq X\leq 1,5)=\dfrac{19}{64}\thickapprox 0,296875
\end{array}
$$
* **d -** Obtener la función de distribución acumulada de $X$.
$$
\begin{array}{l}
x<0\quad f(t)=0\quad F(x)=0 \\
\displaystyle 0\leq x < 2\quad F(x)=\int_{0}^{x} \frac{3}{8}t^{2}dt=\frac{3}{8} \frac{x^{3}}{3}=\frac{x^{3}}{8} \\
\displaystyle 2\leq x\quad F(x)=\int_{0}^{2} \frac{3}{8}t^{2}dt+\int_{2}^{x}0\ dt=1 \\
F(x)=\begin{cases}
0 & si & x\in (-\infty,0) \\
\dfrac{x^{3}}{8} & si & x\in[0,2) \\[1ex]
1 & si & x\in[2,\infty)
\end{cases}
\end{array}
$$
* **f -** Calcular $E(X)\ y\ \sigma_{X}$.
$$
\begin{array}{l}
\displaystyle E(X)=\int_{-\infty}^{\infty}x\cdot f(x)dx=\int_{0}^{2}x\cdot \frac{3}{8}x^{2}dx=\frac{3}{8}\left[ \frac{x^{4}}{4} \right]_{0}^{2}=\frac{3}{2} \\
\displaystyle \mu=E(X)=\frac{3}{2} \\
\displaystyle E(X)^{2}=\frac{9}{4} \\ \\
\displaystyle E(X^{2})=\int_{-\infty}^{\infty}x^{2}f(x)dx=\frac{3}{8}\int_{0}^{2}x^{4}=\frac{3}{8}\left[ \frac{x^{5}}{5} \right]_{0}^{2}=\frac{12}{5} \\
\displaystyle E(X^{2})=\frac{12}{5} \\
\displaystyle \sigma^{2}=V(X)=E(X^{2})-E(X)^{2}=\frac{12}{5}-\frac{9}{4}=\frac{3}{20} \\
\displaystyle \sigma=\sqrt{ \frac{3}{20} }
\end{array}
$$
* **g -** ¿Cuál es la probabilidad de que $X$ esté a menos de 1 desviación estándar de su valor medio?
$$
\begin{array}{l}
\displaystyle P(\mu-\sigma\leq X\leq \mu+\sigma)=P\left( \frac{3}{2}-\sqrt{ \frac{3}{20} }\leq X\leq \frac{3}{2}+\sqrt{ \frac{3}{20} } \right)\thickapprox P(1,1127\leq X\leq 1,8873) \\
P(1,1127\leq X\leq 1,8873)=F(1,8873)-F(1,1127)\thickapprox 0,6681 \\
P(\mu-\sigma\leq X\leq \mu+\sigma)\thickapprox 0,6681
\end{array}
$$
## Distribución Uniforme
### Ejercicio 4
Un tiempo $X$ (en minutos) en que un asistente de laboratorio prepara el equipo para un experimento tiene una distribución uniforme en el intervalo [25, 35] $(\mathcal{U}$[25,35]).
* **a -** Dar la función de densidad y la función de distribución acumulada de $X$.
$$
\begin{array}{l}
f(x)=\begin{cases}
\dfrac{1}{10} & 25<x<35 \\[2ex]
0 & \text{en otro caso}
\end{cases} \\
F(x)=\begin{cases}
0 & x<25 \\
\dfrac{x-25}{10} & 25<x<35 \\
1 & x>35
\end{cases}
\end{array}
$$
* **b -** ¿Cuál es la probabilidad de que el tiempo de preparación exceda los 33 minutos?
$$
P(33\leq X)=1-P(X\leq 33)=1-\dfrac{33-25}{10}=\dfrac{1}{5}=0,2
$$
* **c -** Para cualquier $a$ tal que $25<a<a+2<35$ ¿Cuál es la probabilidad de que el tiempo de preparación este entre $a$ y $a+2$?
$$
\begin{array}{l}
P(a\leq X\leq a+2)=F(a+2)-F(a)=\dfrac{a+2-25}{10}-\dfrac{a-25}{10}=\dfrac{2}{10} \\
P(a\leq X\leq a+2)=0,2
\end{array}
$$
* **d -** Calcular $E(X)$ y $V(X)$.
$$
\begin{array}{l}
E(X)=\dfrac{a+b}{2}=\dfrac{25+35}{2} \\
\mu=E(X)=30 \\
V(X)=\dfrac{(b-a)^{2}}{12}=\dfrac{(35-25)^{2}}{12} \\
\sigma^{2}=V(X)=\dfrac{25}{3} \\
\sigma=\dfrac{5}{\sqrt{3}}\thickapprox 2,886751346
\end{array}
$$
* **e -** ¿Cuál es la probabilidad de que el tiempo de preparación de encuentre a 1 DE del tiempo medio de preparación? ¿Y a menos de 2 DE?.
$$
\begin{array}{l}
P(\mu-\sigma\leq X\leq \mu+\sigma)\thickapprox P(30-2,8868\leq X\leq 30+2,8868)=P(27,1132\leq X\leq 32,8868) \\
P(27,1132\leq X\leq 32,8868)=F(32,8868)-F(27,1132)=0,7887-0,2113 \\
P(\mu-\sigma\leq X\leq \mu+\sigma)\thickapprox0,5774 \\
P(\mu-2\sigma\leq X\leq \mu+2\sigma)=P\left( 30-\dfrac{10}{\sqrt{3}}\leq X\leq 30+\dfrac{10}{\sqrt{3}} \right)=F(35,7735)-F(24,2265)=1-0 \\
P(\mu-2\sigma\leq X\leq \mu+2\sigma)=1
\end{array}
$$
## Distribución Normal
### Ejercicio 5
Sea $X$ una variable aleatoria con distribución normal con media 80 y varianza 100 $(\mathcal{N}(80,100))$. 
$$
\begin{array}{l}
\sigma^{2}=100 \\
\sigma =10 \\
\mu=80 \\
Z=\dfrac{X-\mu}{\sigma}=\dfrac{X-80}{10}
\end{array}
$$
Calcular:
* **a -** $P(X\leq 100)$
$$
\begin{array}{l}
P(X\leq 100)=P\left( Z\leq \dfrac{100-80}{10} \right)=P(Z\leq 2) \\
P(X\leq 100)=0.9772
\end{array}
$$
* **b -** $P(65\leq X\leq 100)$
$$
\begin{array}{l}
P(65\leq X\leq 100)=P\left( \dfrac{65-80}{10}\leq Z\leq\dfrac{100-80}{10} \right)=P(-1,5\leq Z\leq 2) \\
P(-1,5\leq Z\leq 2)=\Phi(2)-\Phi(-1,5)=\Phi(2)+\Phi(1,5)-1=0.9772+0.9332-1 \\
P(65\leq X\leq 100)=0,9104
\end{array}
$$
* **c -** $P(70\leq X)$
$$
\begin{array}{l}
P(70\leq X)=P\left( \frac{70-80}{10}\leq Z\right)=P(-1\leq Z)=P(Z\leq 1) \\
P(70\leq X)=0.8413
\end{array}
$$
* **d -** $P(85\leq X\leq 95)$
$$
\begin{array}{l}
P(85\leq X\leq 95)=P\left( \dfrac{85-80}{10}\leq Z\leq \dfrac{95-80}{10}\right)=P( 0,5\leq Z\leq 1,5) \\
P( 0,5\leq Z\leq 1,5)=\Phi(1,5)-\Phi(0,5)=0.9332-0.6915 \\
P(85\leq X\leq 95)=0,2417
\end{array}
$$
* **e -** $P(|X-80|\leq 10)=P(-10\leq X-80\leq 10)=P(70\leq X\leq 90)$
$$
\begin{array}{l}
P(70\leq X\leq 90)=P\left(\dfrac{70-80}{10}\leq Z\leq\dfrac{90-80}{10}\right)=P(-1\leq Z\leq 1)=2\Phi(1)-1 \\
P(70\leq X\leq 90)=0,6826
\end{array}
$$
### Ejercicio 6
El diámetro de los árboles de determinado tipo, a cierta altura, se distribuye normalmente con $\mu=8,8$" y $\sigma=2,8$" Según sugiere el articulo "Simulating a Harvester-Forwarder Softwood Thinning".
* **a -** ¿Cuál es la probabilidad de que el diámetro de un árbol, seleccionado al azar, sea de a lo sumo 10"? ¿Y que sea mayor a 10"?
$$
\begin{array}{l}
P(X\leq 10)=P\left( Z\leq \dfrac{10-8,8}{2,8} \right)=P\left( Z\leq \dfrac{3}{7} \right)\thickapprox P(Z\leq 0,43) \\
P(X\leq 10)\thickapprox 0,6664 \\
P(X\geq 10)\thickapprox P(Z\geq 0,43)=1-P(Z\leq 0,43)=1-0,6664 \\
P(X\geq 10)\thickapprox 0,3336
\end{array}
$$
* **b -** ¿Cuál es la probabilidad de que el diámetro del un árbol, seleccionado al azar, esté entre 5" y 10"? 
$$
\begin{array}{l}
P(5\leq X\leq 10)=P\left( \dfrac{5-8,8}{2,8}\leq Z\leq \dfrac{10-8,8}{2,8} \right)=P\left(- \dfrac{19}{14}\leq Z\leq \dfrac{3}{7} \right)\thickapprox P(-1,36\leq Z\leq 0,43) \\
P(-1,36\leq Z\leq 0,43)=\Phi(0,43)+\Phi(1,36)-1=0,6664+0,9131-1 \\
P(5\leq X\leq 10)=0,5795
\end{array}
$$
* **c -** ¿Qué valor de $c$ es tal que el intervalo $(8,8-c;8,8+c)$ incluye el $98\%$ de todos los valores de diámetro?
$$
\begin{array}{l}
P(8,8-c\leq X\leq 8,8+c)=P(\mu-c\leq X\leq \mu+c)=0,98 \\
P(\mu-c\leq X\leq \mu+c)=P(X\leq|c|+\mu)=P\left( Z\leq \dfrac{|c|+\mu-\mu}{\sigma} \right)=P\left( Z\leq \dfrac{|c|}{\sigma} \right)=2\Phi\left( \dfrac{c}{\sigma} \right)-1\\
\Phi \left( \dfrac{c}{\sigma} \right)=\dfrac{1+0,98}{2}=0,99 \\
z_{0,99}\thickapprox 2,33\Longrightarrow \dfrac{c}{2,8}=2,33\iff c=2,33\cdot 2,8 \\
c=6,524
\end{array}
$$
* **d -** ¿Cuál es la probabilidad de que al menos 1 de 5 árboles elegidos al azar tenga diámetro entre 5" y 10"?.
$$
\begin{array}{l}
Y=\text{cantidad de arboles cuyo diametro esta entre 5" y 10"  de un total de 5} \\
\mathcal B(5;0,5795) \\
P(1\leq Y)=1-P(X\leq 0)=1-P(X=0)=1-(1-0,5795)^{5} \\
P(1\leq Y)=0,9869
\end{array}
$$
### Ejercicio 7
La distribución de resistencia para resistores de cierto tipo es normal, el $10\%$ de todos los resistores tienen una resistencia que excede los 10,256 ohm y el $5\%$ una resistencia menor que 9,671 ohm ¿Cuáles son los valores de la media y la desviación estándar de la distribución de la resistencia?
$$
\begin{array}{l}
P(X> 10,256)=0,10\iff P(X \leq 10,256)=0,90 \Longrightarrow z_{1}=1,28 \\
P(X\leq 9,671)=0,05\Longrightarrow z_{2}=-1,64 \\
z=\dfrac{x-\mu}{\sigma}\Longrightarrow x=\mu+z\sigma \\
\begin{array}{l}
\begin{cases}
10,256=\mu+1,28\sigma \\
9,671=\mu-1,64\sigma
\end{cases}\iff &
\left[\begin{array}{cc|c}
1 & 1,28 & 10,256 \\
1 & -1,64 & 9,671
\end{array}\right]\iff &
\left[\begin{array}{cc|c}
1 & 1,28 & 10,256 \\
0 & -2,92 & −0,585
\end{array}\right]\iff \\[2ex]
\left[\begin{array}{cc|c}
1 & 1,28 & 10,256 \\
0 & 1 & 0,2003
\end{array}\right]\iff &
\left[\begin{array}{cc|c}
1 & 0 & 9,9996 \\
0 & 1 & 0,2003
\end{array}\right]\iff &
\begin{cases}
\mu=9,9996 \\
\sigma=0,2003
\end{cases}
\end{array}
\end{array}
$$

### Ejercicio 8
* **a -** Demuestre que si $X$ tiene una distribución normal con parámetros $\mu$ y $\sigma$, entonces $Y=aX+b$ con $a\neq 0$, también tiene una distribución normal. ¿Cuáles con los parámetros de la distribución $Y$ (Es decir $E(Y)$ y $V(Y)$)?
$$
\begin{array}{l} 
Y \sim N(\mu,\sigma^{2}) \\
Y=aX+b \iff X=\dfrac{Y-b}{a}\Longrightarrow \dfrac{dx}{dy}=\dfrac{1}{a}\\
f_{x}(x)=\dfrac{1}{\sigma\sqrt{2\pi}}e^{-(x-\mu)/2\sigma^{2}}=\dfrac{1}{\sigma}\varphi\left(\dfrac{x-\mu}{\sigma}\right) \\
f_{y}(y)=f_{x}\left(\dfrac{y-b}{a}\right)\dfrac{dx}{dy} \\
f_{y}(y)=\dfrac{1}{|a|\sigma}\varphi\left(\dfrac{y-(\mu a+b)}{\sigma |a|}\right) \\
Y \sim N(\mu a+b,(\sigma|a|)^{2})
\end{array}
$$
* **b -** Si la temperatura medida en $°C$ está normalmente distribuida con media 115 y desviación estándar 2, ¿qué se puede decir acerca de la distribución de la temperatura medida en $°F$?.
$$
\begin{array}{l}
C\sim N(\mu_{C},\sigma_{C}^{2}) \\
\mu_{C}=115 \\
\sigma_{C}=2 \\
F=C\dfrac{9}{5}+32 \\
F\sim N\left(115\cdot\dfrac{9}{5},\left( 2\cdot\dfrac{9}{5}\right)^{2}\right) \\
F\sim N(207,12.96) \\
\sigma=3,6
\end{array}
$$
### Ejercicio 9

En una fábrica se fabrican tornillos cuyo diámetro es una variable aleatoria normal. Se pueden usar dos máquinas de distintas marcas para cortarlos. Si se cortan con la maquina $A$, el diámetro del tornillo (medido en cm) es una variable con distribución $N(1,0.4)$. Si se cortan con la máquina $B$ (cuyo costo de mantenimiento es mucho menor) el diámetro (también medido en cm) resulta una variable con distribución $N(1.1,0.4)$. la maquina $A$ se usa el $40\%$ de las veces y la $B$ el $60\%$ de las veces. Para que un tornillo de considere aceptable, su diámetro debe de estar entre 0,9 y 1,1 cm.
* **a -** ¿Cuál es la probabilidad de que un tornillo elegido al azar cumpla el requerimiento deseado?
$$
\begin{array}{l}
\mu_{A}=1 \\
\sigma_{A}=\sqrt\frac{4}{10}\thickapprox 0,4472 \\
P(E|A)=P(0,9\leq X_{A}\leq 1,1)=P\left(\dfrac{0,9-1}{0,4472}\leq Z\leq\dfrac{1,1-1}{0,4472}\right) \\
P(−0,2236\leq Z\leq 0,2236)=2\Phi(0,2236)-1=2\cdot0.5871-1 \\
P(E|A)=0,1742 \\
P(A)=0,40 \\
\mu_{B}=1,1 \\
\sigma_{B}\thickapprox 0,4472 \\
P(E|B)= P(0,9\leq X_{B}\leq 1,1)=P\left(\frac{0,9-11}{0,4472}\leq Z \leq \frac{1,1-1,1}{0,4472}\right)=P(-0,4472\leq Z\leq 0)\\
P(-0,4472\leq Z\leq 0)=\Phi(0)-\Phi(-0,4472)=\Phi(0)+\Phi(0,4472)-1=0,5 + 0,6700-1\\
P(E|B)=0,17 \\
P(B)=0,60 \\
P(A\cap B)=0\\
P(E)=P(E|A)P(A)+P(E|B)P(B) \\
P(E)=0,1742\cdot 0,40+0,17\cdot 0,6 \\
P(E)=0,17168
\end{array}
$$
* **b -** Se ha logrado estabilizar la máquina $B$ para producir tornillos con diámetro medio de 1 cm. Su desvío estándar $\sigma$ todavía debe ser regulado. ¿Que valor debería tomar $\sigma$ para cumplir los requerimientos de calidad con probabilidad mayor o igual que 0,90?