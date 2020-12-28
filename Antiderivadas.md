# Antiderivada y la integral indefinida

La derivada y la integral indefinida son dos operaciones que se realizan sobre funciones. En este caso, la integral indefinida toma una función y entrega como resultado otra función. La forma en cómo se define la integral indefinida, junto con sus propiedades algebraicas, hace que posea una estrecha relación con la derivada. La manera más natural de entender las integrales indefinidas es a través de la antiderivada. En esta oportunidad, sólo nos limitaremos a entender los conceptos de la manera más algebraica posible, obviando detalles relacionados a las funciones involucradas, como por ejemplo su *dominio*.

## Definición
Una **antiderivada** de una función $y=f(x)$ es una función $y=F(x)$ derivable que cumple $\displaystyle \frac{dF}{dx}=f(x)$

**Observación** Las antiderivadas no son únicas. En efecto, si $y=F(x)$ es una antiderivada de $y=f(x)$, entonces $y=G(x)=F(x)+K$ también lo es, ya que:

$$
\begin{aligned}
\frac{dG}{dx}&=\frac{d}{dx}\left( F(x)+K\right)\\
&=\frac{d}{dx}F(x)+ \frac{d}{dx}K\\
&=\frac{d}{dx}F(x)+0\\
&=\frac{d}{dx}F(x)\\
&=f(x)
\end{aligned}
$$


### Ejemplos

- **Ejemplo 1**  Si $f(x)=2x$, entonces **una** antiderivada es $F(x)=x^{2}$, porque $F'(x)=2x$.

- **Ejemplo 2**  Si $f(x)=x^3$, entonces una antiderivada es $F(x)=\frac{x^{3}}{3}$, porque:
$$F'(x)=\left(\frac{x^{3}}{3}\right)'=3\frac{x^2}{3}=x^2$$

## La integral indefinida

Si $y=F(x)$ es una antiderivada de la función $y=f(x)$, entonces la integral indefinida de $y=f(x)$ es:
$$\int f(x) \,dx=F(x)+K,$$
donde $K$ es una constante.

### Ejemplos

## Integrales de funciones elementales

#### 1. Integrales de monomios
La integral del monomio $x^n$, con respecto a la variable $x$, es:

$$\int x^{n}dx=\frac{x^{n+1}}{n+1}+K,$$

para todo $n\in \mathbb{R}$ y $n\neq 1$

#### Ejemplos.
*Ejemplo 1* 
$$\int  x^2\, dx=\frac{x^{2+1}}{2+1}+K=\frac{x^3}{3}+K$$ En este caso, $n=2$.

*Ejemplo 2.* 

 $$\int  x^{-7}\, dx=\frac{x^{-7+1}}{-7+1}+K=\frac{x^{-6}}{-6}+K=-\frac{1}{6x^6}+K$$ En este caso, $n=-7$.

#### Observaciones
* Sabemos que  $x^0=1$. En este caso, la integral indefinida queda de la siguiente manera:
$$\int 1\, dx =\int  x^{0}\, dx=\frac{x^{0+1}}{0+1}+K=x+K$$ Para evitar escribir $\int 1\, dx$ o $\int x^0\, dx$, ocupamos la notación: 
$$\int \,dx=x+K$$

* La fórmula $\int x^{n}dx=\frac{x^{n+1}}{n+1}+K$ **no sirve** para integrar $x^{-1}$, porque en este caso, $n=-1$. 
 
#### 2. Integrales de funciones trigonométricas

Las integrales de las funciones *seno* y *coseno* son las siguientes:
$$
\begin{aligned}
\int  \sin(x)\, dx &= -\cos(x)+K\\
\int  \cos(x)\, dx &= \sin(x)+K
\end{aligned}
$$

#### 3. Integral de la exponencial
Para la función exponencial en base $e$, a saber, $f(x)=e^x$, su integral indefinida es la siguiente[^1]:
$$
\begin{aligned}
\int e^x\, dx &= e^x+K
\end{aligned}$$

#### 4. Integral de la función $f(x)=\frac{1}{x}$

La integral de la función racional $f(x)=\frac{1}{x}$ es:

$$\int \frac{1}{x}\, dx=\ln |x|+K$$

donde $\ln$ es el *logaritmo natural en base* $e$[^2].
## Propieades algebraicas de las integrales

Al igual que las derivadas, las integrales indefinidas tienen propiedades algebraicas con respecto a la suma y al producto, que permiten calcular integrales más complejas:

**Teorema** Sean $f,\, g$ funciones con variables independiente $x$ y sea $k\in \mathbb{R}$ una constante:
$$		
\begin{aligned}
\int (f(x)\pm g(x))\, dx &= \int f(x)\,dx\pm \int g(x)\, dx , \\
\int k\cdot f(x)\, dx &= k\cdot \int f(x)\, dx.
\end{aligned}
$$
En un lenguaje más formal, al cumplirse las igualdades de arriba, se dice que la integral posee la propiedad de *linealidad*. 

### Ejemplos

* **Ejemplo 1** Calcular la integral indefinida de la función $f( x) =3x^{3} +2x^{2} -x+5$

  **Desarrollo**
$$
\begin{aligned}
	\int f(x) \, dx &= \int 3x^{3} +2x^{2} -x+5 \, dx \\
			 &= \int 3x^{3}\, dx +\int 2x^{2}\, dx -\int  x\, dx+\int 5 \, dx \\
			  &= 3\int x^{3}\, dx +2\int x^{2}\, dx -\int  x\, dx+5\int  \, dx \\
			  &= 3\cdot \frac{x^{4}}{4} +2\cdot  \frac{x^{3}}{3} -  \frac{x^2}{2}+5x+K \\
			  &=  \frac{3x^{4}}{4} + \frac{2x^{3}}{3} -  \frac{x^2}{2}+5x+K \\
\end{aligned}
$$

* **Ejemplo 2**  Calcular la integral indefinida de la función $g(x)=3\sin(x)-2e^x$

  **Desarrollo**
  $$
  \begin{aligned}
	\int g(x) \, dx &= \int 3\sin(x)-2e^x\, dx \\
			 &= \int 3\sin(x)\, dx -\int 2e^x\, dx  \\
			  &= 3\int \sin(x)\, dx -2\int e^x\, dx  \\
			  &= -3\cos(x)-2e^x+K \\
\end{aligned}
$$




## Relación entre la integral indefinida y la derivada

Por como es definida la integral indefinida, las siguientes consecuencias son *inmediatas*:

1. La antiderivada de la derivada de una función es la misma función más la constante de integración. En otras palabras: $$\int f'(x)\, dx=f(x)+K.$$

2. La derivada de la antiderivada de una función es la misma función. En otras palabras: $$\frac{d}{dx}\int f(x)\, dx=f(x).$$

Observación importante En resumen, la derivada y la integral indefinida son operaciones inversas una de la otra.

## Problemas propuestos 

**Problema 1** Calcular la integral indefinida de las siguientes funciones:
1. $\int (3x^4-8x^2+2x)\, dx$
2. $\int (10x^{3/4}-4x^{-2/5})\, dx$
3. 

**Problema 2** 

**Problema 3** 

**Problema 4** 

[^1]: $e$ es el número de Euler $e=2.71828...$
[^2]: También llamado logaritmo neperiano.


> Written with [StackEdit](https://stackedit.io/).



<!--stackedit_data:
eyJoaXN0b3J5IjpbNjg2MzM5OTgyLC0zNjkyNDk3MTEsLTUxMj
k3NTI0NywtNDIyMjY3NTA4LDYzODIxMDg3MiwtMTE5NzMyMjQ1
Myw5ODUzNzMzMDIsMTk0NTE3NDg3OCwtMjA3OTk1OTc1LC0xND
Q1NTgzMDczLC0yMTQ0MDQ3ODE4XX0=
-->