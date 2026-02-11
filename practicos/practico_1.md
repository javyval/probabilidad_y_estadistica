## Probabilidad
### **Ejercicio 1**
La biblioteca de una universidad tiene cinco ejemplares de un cierto texto en reserva. Dos ejemplares (1 y 2) son primeras impresiones y los otros tres (3, 4 y 5) son segundas impresiones. Un estudiante examina estos libros en orden aleatorio, deteniéndose solo cuando selecciona una segunda impresión.
-  a - Hacer una lista de todos los resultados posibles.
-  b - Sea el evento A: solo un libro es examinado. ¿Cuales resultados están en A?. 
-  c - Sea el evento B: el libro 5 es seleccionado. ¿Cuales resultados están en B?. 
-  d - Sea el evento C: el libro 1 no se examina. ¿Cuales resultados están en C?
-  e - Expresar A ∩ B, A ∪ B y $\overline{B \cap C}$.  

*  a - $$ \begin{array}{rrr}
(1, 2, 3) & (1, 2, 4) & (1, 2, 5) \\
(2, 1, 3) & (2, 1, 4) & (2, 1, 5) \\
(1, 3) & (1, 4) & (1, 5)\\
(2, 3) & (2, 4) & (2, 5) \\
(3) & (4) & (5)
\end{array} $$
* b  - $$A= \{(3), (4), (5)\}$$
* c -$$ B = \{(1, 2, 5), (2, 1, 5), (1, 5), (2, 5), (5)\} $$
* d - $$C = \{(2, 3), (2, 4), (2, 5), (3), (4), (5)\}$$
$$A \cap B =\{(5)\}$$ $$A \cup B = \{(1, 2, 5), (2, 1, 5), (1, 5), (2, 5), (3), (4), (5)\}$$$$\overline {B \cap C} = \{(1, 2, 3), (1, 2, 4), (1, 2, 5), (2, 1, 3), (2, 1, 4), (2, 1, 5), (1, 3), (1, 4), (1, 5), (2, 3), (2, 4), (3), (4) \}$$
### **Ejercicio 2**
Demostrar que si un evento A esta contenido en otro B, entonces P (B − A) = P (B) − P (A) y P (A) ≤ P (B). En general, dados dos eventos A y B, ¿que relación existe entre P (A), P (A ∩ B) y P (A ∪ B)?.

Sea $A \subset B \implies P(B-A) = P(B) - P(A)$
![[venn_A_contenido_B|200]]

Como $A \subset B$ Entonces podemos expresar a B como el conjunto disjunto:
$B = A \cup (B-A)$ , como son disjuntos $P(B) = P(A) + P(B - A)$ . Luego $$P(B-A)=P(B)-P(A)$$
Finalmente como  $P(B-A) \geq 0$  entonces $P(B) - P(A) \geq 0$ . Sumando $P(A)$ a ambos lados queda $$P(B)\geq P(A)$$
Relación, en general $$P(A) \cap P(B) \leq P(A) \leq P(A)\cup P(B)$$
### **Ejercicio 3**

Una empresa de consultoría de computadoras ha licitado en tres proyectos. Sea $A_i = \{proyecto\ i\ otorgado\}$, para $i = 1, 2, 3$, y supongamos  que 
$$\begin{array}{lll} 
P(A_{1})=0,22 & P(A_{2})=0,25 & P(A_{3})=0,28 \\
P(A_1\cap A_{2})=0,11 & P(A_1 \cap A_{3})=0,05 & P(A_{2}\cap A_{3})=0.07\\
P(A_{1} \cap A_{2}\cap A_{3}) = 0,01
\end{array}$$   Calcule la probabilidad de los siguientes eventos:
* **a -** $P(A_{1}\cup A_{2})= P(A_{1})+P(A_{2})-P(A_{1}\cap A_{2})=0,22 + 0,25 - 0,11 = 0,36$
* **b -** $P(\overline {A_{1}} \cap \overline{A_{2}}) = P(\overline{A_{1}\cup A_{2}})= 1 - P(A_{1}\cup A_{2})= 1 -0,36 = 0,64$
* **c -** $P(A_{1}\cup A_{2} \cup A_{3})=P(A_{1}\cup A_{2}) + P(A_{3})-P((A_{1}\cup A_{2})\cap A_{3})=$
	$P(A_{1}\cup A_{2}) + P(A_{3})-P((A_{1}\cap A_{3})\cup (A_{2}\cap A_{3}))=$
	$P(A_{1}\cup A_{2}) + P(A_{3})-P(A_{1}\cap A_{3})- P(A_{2}\cap A_{3})+ P(A_{1}\cap A_{2}\cap A_{3})=$
	$0,36 + 0,28 - 0,05 - 0,07 + 0,01 = 0,53$
* **d -** $P(\overline {A_{1}}\cap\overline{A_{2}}\cap\overline{A_{3}})=P(\overline{A_{1}\cup A_{2}\cup A_{3}})=1-P(A_{1}\cup A_{2}\cup A_{3}) = 1-0,53=0,47$
* **e -**   $P(\overline{A_{1}}\cap\overline{A_{2}}\cap A_{3})= P(A_{1}\cup A_{2}\cup\overline{A_{3}})=$
* **f -** $P((\overline{A_{1}}\cup\overline{A_{2}}\cup{A_{3}}))$

### **Ejercicio 4**

Cinco empresas $F_{1},F_{2},\dots F_{5}$ hacen propuestas con respecto a tres contratos separados $C_{1},\ C{2}, y \ C_{3}$. Una empresas solo puede obtener a lo sumo un contrato. Los contratos son diferentes, de tal forma que la asignación de $C_{1} \ a \ F_{1}$ se debe diferenciar de la asignación $C_{2} \ a \ F_{1}$.
* **a -** ¿Cuantos puntos muestrales hay en total en este experimento que trata de la asignación de contratos a las empresas? (No hay necesidad de listar todos los puntos). $$\frac{5!}{(5-3)!}=\frac{5!}{2!}=60$$
* **b -** Encuentre la probabilidad de que se conceda un contrato a la empresa $F_{3}$, bajo el supuesto de que los puntos muestrales son equiparables. $$\begin{array}{l}
Cantidad\ de\ elementos =3\ Perm(4,2)=3 \dfrac{4!}{2!}=3*12=36 \\[2ex]
\text{Elijo uno de los 3 posibles contratos y ubico 4 de las empresas en los 2 contratos restantes.} \\[2ex]
P(A)=\dfrac{36}{60}=0,6\quad\text{(Probabilidad de Laplace)}
\end{array}$$ 
### Ejercicio 5 
Al poco tiempo de se puestos en servicio, algunos colectivos fabricados por cierta compañía presentan grietas en su parte inferior. Una ciudad tiene 25 de estos colectivos  y han aparecido grietas en 8 de ellos. Se seleccionan aleatoriamente 5 colectivos para hacer una inspección.
* **a -** ¿Cual es la la probabilidad de que 4 de los 5 colectivos tengan grietas?
$$\begin{array}{l}
 Formas\ de\ elegir\ 5\ colectivos = C(25, 5)= \dfrac{25!}{5!(25-5)!}\\[2ex]
 4\ de\ los\ 5\ tienen\ grietas = C(17,1)*C(8,4)=\dfrac{17!}{1(16)!} \dfrac{8!}{4!(8-4)!} \\[2ex]
P(A)=\dfrac{C(17,1)*C(8,4)}{C(25,5)}=\dfrac{70*17}{53130}= 0, 0224

\end{array}$$
* **b -** ¿Cual es la probabilidad de que al menos 4 de los seleccionados tengan grietas?$$\begin{array}{l}
P(B)=P(4\ tienen\ grietas)+P(5\ tienen\ grietas) \\[2ex]
P(B)=\dfrac{C(17,1)*C(8,4)}{C(25,5)}+\dfrac{C(17,0)*C(8,5)}{C(25,5)}=\dfrac{70*17}{53130} + \dfrac{1*56}{53130}=0,023
\end{array}$$
### Ejercicio 6
Un departamento académico con cinco miembros de la facultad: Anderson, Box, Cox, Cramer y Fisher, debe seleccionar a dos de sus miembros ara prestar servicio en una comisión de revisión de personal. debido a que el trabajo sera lento, nadie desea prestar ese servicio, así que deciden que el representante ser seleccionado por el método de colocar cinco boletas de papel en una caja, mesclarlas y seleccionar dos.
* **a -** ¿Cual es la probabilidad de que Box y Anderson sean seleccionados?
$$ \begin{array}{l}
Formas\ de\ elegir\ 2\ personas\ = C(5,2) = \dfrac{5!}{2!(5-2)!} = 10 \\[2ex]
P(A)=\dfrac{1}{10}=0,1
\end{array} $$

* **b -** ¿Cual es la probabilidad de que se seleccione por lo menos a uno de los dos miembros cuyos apellidos comienzan con C?$$\begin{array}{l} 
P(B)=\dfrac{C(2,2)}{C(5,2)}+\dfrac{C(2,1)*C(3,1)}{C(5,2)}=\dfrac{1}{10}+\dfrac{6}{10}=\dfrac{7}{10} \\
\text{El primer termino refleja seleccioanr a los dos que empiezan con C.} \\
\text{El segundo termino refleja uno empieza con C, el segundo no empieza con C}
\end{array}$$
* **c -** Si los cinco miembros de la facultad han dado clase en la universidad durante 3, 6 , 7, 10 y 14 años respectivamente, ¿Cual es la probabilidad de que entre los dos representantes seleccionados tengan por lo menos 15 años de experiencia en la enseñanza?.
	$$\begin{array}{l}
Para\ 14 = 4\ posibilidades &
Para\ 10 = 2\ posibilidades &
Para\ 7 = 0\ posibilidades  \\
Para\ 6 = 0\ posibilidades  &
Para\ 3 = 0\ posibilidades  \\[2ex]
P(C)=\dfrac{6}{10}
\end{array}$$
### Ejercicio 7 
Una profesora desea programar una reunión con cada uno de sus ocho ayudantes, cuatro hombres y cuatro mujeres, para analizar su curso. Se supone que todos los ordenamientos posibles de las reuniones tienen la misma probabilidad de ser elegidos.
* **a -** ¿Cuál es la probabilidad de que por lo menos una asistente mujer este ente los tres primeros con quien se reúne la profesora?$$\begin{array}{l}  \\
P(Solo\ hombres\ selccionados)=\frac{\dbinom{4}{3}}{\dbinom{8}{3}}=\dfrac{4}{56}=0,071 \\
P(Al\ menos\ una\ mujer)= 1- P(Solo\ hombres\ selccionados)= 0,929

\end{array}$$

* **b -** ¿Cuál es la probabilidad de que después de las cinco primera reuniones, la profesora se haya reunido con el total de las asistentes?$$P(B)=\dfrac{\dbinom{4}{4}\dbinom{4}{1}}{\dbinom{8}{5}}=\dfrac{4}{56}=0,071$$
## Probabilidad Condicional
### Ejercicio 8
Una caja contiene 6 cubos rojos y 4 verdes y una segunda caja contiene 7 cubos rojos y 3 verdes. Se elije al azar un cubo de la primera caja y se pone en la segunda caja. Luego se selecciona al azar un cubo de la segunda caja y se pone en la primer caja.
* **a -** ¿Cual es la probabilidad de que se seleccione un cubo rojo de la primera caja y un cubo rojo de la segunda caja?$$\begin{array}{l}
P(R_{1})=\dfrac{6}{10}=0,6 \\
P(R_{2}/R_{1})=\dfrac{7+1}{11}=0,727 \\
P(R_{2}/R_{1})=\dfrac{P(R_{1}\cap R_{2})}{P(R_{1})}\Longrightarrow P(R_{1}\cap R_{2})=P(R_{2}/R_{1})*P(R_{1}) \\
P(A)=P(R_{1}\cap R_{2})=\dfrac{6}{10}* \dfrac{8}{11}=0,436
\end{array}$$
* **b -** Al finalizar el proceso de selección ¿Cuál es la probabilidad de que los números de los cubos rojos y vedes de la primera caja sean idénticos a los que había al comienzo?.$$\begin{array}{l} 
P(V_{1})=\dfrac{4}{10}=0,4 \\
P(V_{2}/V_{1})=\dfrac{3+1}{11}=0,364 \\
P(B)=P(V_{1}\cap V_{2})=\dfrac{4}{10} * \dfrac{4}{11}=0,145 \\
P(C)=P(A)+P(B)=\dfrac{24}{55} + \dfrac{8}{55}=0,582 \\
\text{La probabilidad de que los cubos rojos y verdes sean identicos al final es si seleccione} \\
\text{primero un cubo rojo de la primera y un rojo de la segunda, ó} \\
\text{primero un cubo verde de la primera y un verde de la segunda.} \\
P(C)=0,582
\end{array}$$
### Ejercicio 9
Una gran tienda de departamentos vende camisas deportivas en tres talles (pequeño, mediano y grande), en tres modelos (a cuadros, estampados y de franjas) y con dos largos de mangas (corta y larga). Las siguientes tablas presentan las proporciones de camisas vendidas que caben en varias combinaciones de categorías.
$$\begin{array}{|lccc|} \hline
\text{Manga corta}  \\ \hline
&& \text{Modelo} \\ \hline
\text{Talle} & \text{Cuadros} & \text{Estampada} & \text{Franjas} \\ \hline
\text{Pequeño} & 0,04 & 0,02 & 0,05 \\
\text{Mediano} & 0,08 & 0,07 & 0,12 \\
\text{Grande} & 0,03 & 0,07 & 0,08 \\\hline
\text{Manga larga} \\\hline
&&\text{Modelo} \\\hline
\text{Talle} & \text{Cuadros} & \text{Estampada} & \text{Franjas} \\ \hline
\text{Pequeño} & 0,03 & 0,02 & 0,03 \\
\text{Mediano} & 0,10 & 0,05 & 0,07 \\
\text{Grande} & 0,04 & 0,02 & 0,08 \\ \hline
\end{array}$$
* **a -** ¿Cuál es la probabilidad de que la camisa que se venda sea una mediana, de manga larga y estampada?$$P(A)=0,05$$
* **b -** ¿Cuál es la probabilidad de que la camisa que se venda sea mediana y estampada?$$P(B)=0,05+0,07=0,12$$
* **c -** ¿Cuál es la probabilidad de que la camisa que se venda sea de manga corta?. ¿Y de manga larga?$$\begin{array}{l}
P(C_{1})=0,04+0,02+0,05+0,08+0,07+0,12+0,03+0,07+0,08 \\
P(C_{1})=0,56 \\
P(C_{2})=0,03+0,02+0,03+0,10+0,05+0,07+0,04+0,02+0,08 \\
P(C_{2})=0,44
\end{array}$$
* **d -** ¿Cuál es la probabilidad de que el talle de la camisa que se venda sea mediano?. ¿Y que el modelo sea estampado?$$\begin{array}{l}
P(D_{1})=0,08+0,07+0,12+0,10+0,05+0,07 \\
P(D_{1})=0,49 \\
P(D_{2})=0,02+0,07+0,07+0,02+0,05+0,02 \\
P(D_{2})=0,25
\end{array}$$
* **e -** Dado que la camisa que se vendió era a cuadros y de manga corta, ¿Cuál es la probabilidad de que su talle sea mediano?.$$\begin{array}{l}
P(E)=\dfrac{0,08}{0,04+0,08+0,03}=0,53
\end{array}$$
* **f -** Dado que la camisa que se vendió era a cuadros y mediana, ¿Cuál es la probabilidad de que sea de manga corta?  ¿Y de manga larga?$$\begin{array}{l}
P(F_{1})=\dfrac{0,08}{0,08+0,10}=\dfrac{4}{9}=0,44 \\
P(F_{2})=\dfrac{0,10}{0,08+0,10}=\dfrac{5}{9}=0,56
\end{array}$$
### Ejercicio 10
* **a -** Dados los eventos $A$ y $B$  $con P(B) > 0$, demuestre que $P(A|B) + P(\overline{A}|B)=1$ $$\begin{array} {l}
P(A|B)=\dfrac{P(A\cap B)}{P(B)} \\
P(\overline{A}|B)=\dfrac{P(\overline{A}\cap B)}{P(B)} \\
P(A|B) + P(\overline{A}|B)=\dfrac{P(A\cap B)+P(\overline{A}\cap B)}{P(B)} \quad //A\cap B\ y\ \overline{A}\cap B\ \ \text{Son disjuntas} \\
P(A|B) + P(\overline{A}|B)=\dfrac{P((A\cap B)\cup(\overline{A}\cap B))}{P(B)}\quad//(A\cap B)\cup(\overline{A}\cap B)=B \\
P(A|B) + P(\overline{A}|B)=\dfrac{P(B)}{P(B)}=1 \quad\therefore QED
\end{array}$$![[practico1_ej10|300]]

* **b -** Si $P(B|A) > P(B)$, demuestre que $P(\overline{B}|A) < P(\overline{B})$.$$\begin{array}{l}
P(B|A) + P(\overline{B}|A)=1 \Longrightarrow P(\overline{B}|A)=1 - P(B|A) \\
P(B|A) > P(B) \\
-P(B|A) < -P(B) \quad\quad\quad\text{|| Multiplica (-1)}\\
1-P(B|A) < 1-P(B) \quad\text{||Suma 1}\\
P(\overline{B}|A) < P(\overline{B})\quad\therefore QED
\end{array}$$
* **c -** Dados los eventos $A, B, C$ con $P(C) > 0$, demuestre que $P(A\cup B|C)=P(A|C)+P(B|C)-P(A\cap B|C)$. $$\begin{array}{l}
P(A\cup B|C)=\dfrac{P((A\cup B)\cap C)}{P(C)}=\dfrac{P((A\cap C)\cup(B\cap C))}{P(C)} \\
P(A\cup B|C)=\dfrac{P(A\cap C)+P(B\cap C)-P((A\cap C)\cap(B\cap C))}{P(C)} \\
P(A\cup B|C)=\dfrac{P(A\cap C)}{P(C)}+\dfrac{P(B\cap C)}{P(C)}-\dfrac{P((A\cap B)\cap C)}{P(C)} \\
P(A\cup B|C)=P(A|C)+P(B|C)-P(A\cap B|C)\quad\therefore QED
\end{array}$$
### Ejercicio 11
Uno de cada 25 adultos está afectado de cierta enfermedad para la cual se ah desarrollado una prueba de diagnóstico. La prueba es tal que, cuando un individuo padece la enfermedad, el resultado de la prueba es positivo en un 99% de las veces. Mientras que un individuo sin la enfermedad mostrara un resultado positivo solo el 2% de las veces.
* **a -** ¿Cuál es la probabilidad de que un resultado de la prueba sea positivo?.$$P(Pp)=P(S)\cdot P(P|S)+P(E)\cdot P(P|E)=\dfrac{24}{25}\cdot0,02+\dfrac{1}{25}\cdot 0,99=0,0588$$
* **b -** Dado que el resultado de a prueba es positivo, ¿Cuál es la probabilidad de que el individuo tenga la enfermedad?$$P(E|Pp)=\dfrac{P(Pp|E)\cdot P(E)}{P(Pp)}=\dfrac{0,99\cdot\dfrac{1}{25}}{0,0588}=0,6735$$
* **c -** Dado que el resultado de la prueba es negativo, ¿Cuál es la probabilidad de que el individuo no tenga la enfermedad?$$\begin{array}{l}
P(Pn)=1-P(Pp)=1-0,0588=0,9412 \\
P(Pn|S)=\dfrac{P(Pn|S)\cdot P(S)}{P(Pn)}=\dfrac{0,2\cdot\dfrac{24}{25}}{0,9412}=0,0204
\end{array}$$
## Independencia
### Ejercicio 12 
Sean $A$ y $B$ eventos independientes, demostrar que $\overline{A}$ y $B$, $A$ y $\overline{B}$   y $\quad\overline{A}$ y $\overline{B}$ son independientes.$$\begin{array}{l}
P(A)\cdot P(B)=P(A\cap B) \quad\text{|| Hipotesis}\\ \\
B=(A\cap B)\cup (\overline{A}\cap B) \quad\text{|| Disjuntos} \\
P(B)=P(A\cap B)+ P(\overline{A}\cap B)\Longrightarrow \\
P(\overline{A}\cap B)=P(A\cap B)-P(B)\quad\text{|| Usando la Hipotesis} \\
P(\overline{A}\cap B)=P(A)\cdot P(B)-P(B) \\
P(\overline{A}\cap B)=(P(A)-1)\cdot P(B) \\
P(\overline{A}\cap B)=P(\overline{A})\cdot P(B)\Longrightarrow \overline {A}\ y\ B \text{ Son independientes}  \quad\therefore QED
\end{array}$$
$$\begin{array}{l}
P(A)\cdot P(B)=P(A\cap B) \quad\text{|| Hipotesis}\\ \\
A=(A\cap B)\cup(A\cap\overline{B}) \quad\text{|| Disjuntos}\\
P(A)=P(A\cap B)+P(A\cap\overline{B})\iff \\
P(A\cap\overline{B})=P(A\cap B)-P(A) \quad\text{|| Usando la Hipotesis}\\
P(A\cap\overline{B})=P(A)P(B)-P(A) \\
P(A\cap\overline{B})=(1-P(B))\cdot P(A) \\
P(A\cap\overline{B})=P(\overline{B})\cdot P(A) \iff\overline{B}\ y\ A \text{ son independientes}\quad\therefore QED
\end{array}$$
$$\begin{array}{l}
P(A)\cdot P(B)=P(A\cap B) \quad\text{|| Hipotesis}\\ \\
\overline{A}\cap\overline{B}=\overline{A\cup B} \\
P(\overline{A}\cap\overline{B})=1-P(A\cup B)=1-P(A)+P(B)-P(A\cap B) \\
P(\overline{A}\cap\overline{B})=1-P(A)+P(B)-P(A)\cdot P(B) \\
P(\overline{A}\cap\overline{B})=(1-P(A))\cdot (1-P(B)) \\
P(\overline{A}\cap\overline{B})=P(\overline{A})\cdot P(\overline{B})\iff \overline{A}\ y\ \overline{B}\text{ son indepentiendes}\quad\therefore QED
\end{array}$$
### Ejercicio 13
En un lote de 10 tablas de madera, dos están demasiado verdes para ser usadas en construcción de primera calidad. Se seleccionan 2 tablas al azar, una después de otra.
Sea $A = {\text{La primera tabla está verde}}$ y $B={\text{La segunda tabla está verde}}$. Calcule $P(A), P(B)\ y\ P(A\cap B)$.¿Son $A$ y $B$ independientes?.$$\begin{array}{l}
P(A)=\dfrac{2}{10} \\
P(B)=\dfrac{2}{10} \\
P(A)\cdot P(B)=\dfrac{1}{25} \\
P(A\cap B)=\dfrac{2}{10} \cdot\dfrac{1}{9}=\dfrac{1}{45} \\
\text{Dado que }P(A)\cdot P(B)\neq P(A\cap B), \text{ enconces A y B no son independientes}
\end{array}$$
### Ejercicio 14
Un mazo de 52 cartas es mezclado y se reparten 13 cartas a cada uno de los 4 jugadores $A, B, C, y\ D$. Calcular la probabilidad de los siguientes eventos.
* **a -** A tiene todos los corazones, B tiene todos los diamantes, C tiene todos los tréboles, y D tiene todas las picas.$$\begin{array}{l}
\#\text{Casos totales}= \dfrac{52!}{13!13!13!13!} \\
\#Ac=\dbinom{13}{13}=1 \\
P(Ac)=\dfrac{\#Ac}{\#\text{Casos totales}}=\dfrac{13!13!13!13!}{52!}\quad\text{|| Numero muy pequeño} \\
P(Ac)=P(Bd)=P(Ct)=P(Dp)
\end{array}$$
* **b -** Cada jugador tiene cartas de un solo palo.$$\begin{array}{l}
\#\text{Formas de elegir un palo para 4 personas}= 4! \\
P(E)=\dfrac{\#\text{Formas de elegir un palo para 4 personas}}{\#\text{Casos totales}}=\dfrac{4!\cdot 13!13!13!13!}{52!}
\end{array}$$
* **c -** El Jugador A no tiene Ases.$$\begin{array}{l}
\#Ana=\dbinom{48}{13}=\dfrac{48!}{13!\cdot35!} \\
\#\text{Casos totales para un jugador}=\dbinom{52}{13}=\dfrac{52!}{13!\cdot39!} \\
P(Ana)=\dfrac{\#Ana}{\#\text{Casos totales para un jugador}}=\dfrac{48!\cdot 13!\cdot 39!}{13!\cdot 35!\cdot 52!}\thickapprox0,3038
\end{array}$$
* **d -** Cada jugador recibe un As.$$\begin{array}{l}
\#\text{Casos Favorables}=4!\cdot\dfrac{48!}{12!\cdot 12!\cdot 12!\cdot 12!} \\
\#\text{Casos totales}= \dfrac{52!}{13!13!13!13!} \\
P(Ja)=\dfrac{\#\text{Casos Favorables}}{\#\text{Casos totales}}=\dfrac{4!\cdot 48!\cdot 13!\cdot 13! \cdot 13\cdot 13!}{52!\cdot 12!\cdot 12!\cdot 12!\cdot 12!}=\dfrac{4!\cdot 48!\cdot 13^{4}}{52!}\thickapprox0,1055
\end{array}$$
### Ejercicio 15
Se realizó una investigación en personas que sufren leucoplasia oral. El 85% de ellas fuman o consume alcohol, el 45% consume alcohol y el 60% fuma.
* **a -** ¿Cuál es la probabilidad de que una persona elegida al azar de esta población consuma alcohol y no fume?$$\begin{array}{l}
P(A)=0,45 \\
P(F)=0,6 \\
P(A\cup F)=0,85 \\
P(A\cup F)=P(A)+P(F)-P(A\cap F)\Longrightarrow P(A\cap F)=0,2 \\
P(A\cap F)=0,2 \\ \\
A=(A\cap F)\cup (A\cap\overline{F})\\
P(A)= P(A\cap F)+ P(A\cap\overline{F})\Longrightarrow\\
P(A\cap\overline{F})=P(A)-P(A\cap F)=0,45-0,2 \\
P(A\cap\overline{F})=0,25
\end{array}$$
* **b -** SI se elije al azar un individuo fumador, ¿Cuál es la probabilidad de que consuma alcohol?.$$\begin{array}{l}
P(A|F)=\dfrac{P(A\cap F)}{P(F)}=\dfrac{0,2}{0,6}=\dfrac{1}{3}=0,3333
\end{array}$$
* **c -** ¿Son independientes los eventos de fumar y consumir alcohol?$$\begin{array}{l}
P(A)\cdot P(F)= 0,45\cdot 0,6=0,27\neq 0,2 \\
P(A)\cdot P(F)\neq P(A\cap F)\Longrightarrow A\ y\ F \text{ no son independientes}
\end{array}$$
### Ejercicio 16
Una compañía realiza el 50% de sus envíos a través de la empresa de correos 1, el 40% a través de la empresa 2 y el resto por la empresa 3. De los paquetes enviados por la empresa 1, el 2% llega tarde a su destino, el 1% de los paquetes enviados por la empresa 2 llega tarde y, de aquellos enviados por la empresa 3, el 5% llega tarde.
* **a -** ¿Cuál es la probabilidad de que un paquete elegido al azar llegue tarde a su destino?. $$\begin{array}{l}
P(Pf)=P(E_{1})\cdot P(Pf|E_{1})+P(E_{2})\cdot P(Pf|E_{2})+P(E_{3})\cdot P(Pf|E_{3})\quad\text{|| Probabilidad total} \\
P(Pf)=0,5\cdot 0,02+0,4\cdot 0,01+0,1\cdot 0,05 \\
P(Pf)=0,019
\end{array}$$
* **b -** Si un paquete elegido al azar llega a tiempo, ¿Cuál es la probabilidad de que haya sido enviada por la empresa 1?$$\begin{array}{l}
P(Pe)=P(\overline {Pf})=1-P(Pf)=1-0,019 \\
P(Pe)=0,981 \\
P(E_{1}|Pe)=\dfrac{E_{1}\cap Pe}{Pe}=\dfrac{0,98\cdot 0,5}{0,981}=0,4995
\end{array}$$
* **c -** Si se sabe que un paquete no fue enviado por la empresa 3, ¿Cuál es la probabilidad de que llegue a tiempo a su destino?$$\begin{array}{l}
\overline{E_{3}}=E_{1}\cup E_{2} \\
P(Pe|\overline{E_{3}})=\dfrac{P(Pe\cap\overline{E_{3}})}{P(\overline{E_{3}})}=\dfrac{P(Pe\cap E_{1})+P(Pe\cap E_{2})}{P(\overline{E_{3}})}=\dfrac{0,98\cdot 0,5+0,99\cdot 0,4}{0,9} \\
{P(\overline{E_{3}})}=0,9844
\end{array}$$
* **d -** Si se eligen 10 paquetes al azar de los enviados por esta compañía, ¿Cuál es la probabilidad de que ninguno llegue tarde?.$$\begin{array}{l}
P(Pe|E_{3})=\dfrac{P(Pe\cap E_{3})}{P(E_{3})}=\dfrac{0,95\cdot 0,10}{0,10}=0,95 \\
P(Pe|E_{3})^{10}=0,5987
\end{array}$$
### Ejercicio 17
Una costura echa en un avión necesita 25 remaches. La costura tendrá que volver a realizarse si al menos uno de los remaches está defectuoso. Suponga que los remaches están defectuosos independientemente, unos de otros, cada uno con la misma probabilidad.
* **a -** Si el 14% de todas las costuras necesitan volver a efectuarse, ¿Cuál es la probabilidad de que un remache esté defectuoso?.$$\begin{array}{l}
P(Rd)=p \\
R(Rb)= 1- p\quad\quad\text{|| Probabilidad de que un remache este bien} \\
P(Ce)= 0,86 \\
P(Ce)=(1-p)^{25}=0,86\Longrightarrow p=1-\displaystyle\sqrt [ 25 ] { 0,86 } \\
P(Rd)=0,006014754
\end{array}$$
* **b -** Si se quiere que sólo el 10% de las costuras necesiten volver a ejecutarse , ¿Cuál es la probabilidad de que un remache sea defectuoso?.$$\begin{array}{l}
P(Rd)=1-\sqrt[25]{0,9}=0,004205552
\end{array}$$
### Ejercicio 18
En una carrera de caballos participan 6 caballos numerados del 1 al 6. Todos los resultados posibles de la carrera son igualmente probables. Hacen podio los tres de los primeros caballos en terminar la carrera.
* **a -** ¿Cuál es la probabilidad de que el caballo numero 2 salga en primer lugar?$$P(A)=P(C_{2}|P_{1})=\dfrac{1}{6}$$
* **b -** ¿Cuál es la probabilidad de que el caballo numero 1 haga podio?$$P(B)=P(C_{1}|P)=\frac{1}{6}\cdot 3=\frac{1}{2}$$
* **c -** ¿Cuál es la probabilidad de que ocurra al menos uno de los ítems anteriores?.$$\begin{array}{l}
P(A\cap B)=P(A)\cdot P(B|A)=\dfrac{1}{6}\cdot\dfrac{2}{5}=\dfrac{1}{15} \\
P(A\cup B)=P(A)+P(B)-P(A\cap B)=\dfrac{1}{6}+\dfrac{1}{2}-\dfrac{1}{15} \\
P(A\cup B)=\dfrac{3}{5} \\

\end{array}$$
* **d -** Una persona hace apuestas sobre el resultado de la carrera. Apuesta que los caballo numerados con 1, 2 y 3 hacen podio. ¿Cual es la probabilidad de que esta persona gane su apuesta?$$\begin{array}{l}
P(P_{1,2,3})=\dfrac{1}{\dbinom{6}{3}}=\dfrac{1}{\dfrac{6!}{3!3!}}=\dfrac{1}{20}
\end{array}$$