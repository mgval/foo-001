# Antiderivada y la integral indefinida


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

*Ejemplo 2* 
$$\int  x^{-7}\, dx=\frac{x^{-7+1}}{-7+1}+K=\frac{x^{-6}}{-6}+K=\frac{1}{6x^6}+K$$ En este caso, $n=-7$.


#### Observaciones
*Observación 1.* Cuando $n=0$, la integral del monomio $x^0=1$ 
#### Integrales de funciones trigonométricas

#### Integral del logaritmo y la exponencial

## Propieades algebraicas de las integrales

Al igual que las derivadas, las integrales indefinidas tienen propiedades algebraicas con respecto a la suma y al producto, que permiten calcular integrales más complejas:

**Teorema** Sean $f,\, g$ funciones con variables independiente $x$ y sea $k\in \mathbb{R}$ una constante:
$$		
\begin{aligned}
\int (f(x)\pm g(x))\, dx &= \int f(x)\,dx\pm \int g(x)\, dx , \\
\int k\cdot f(x)\, dx &= k\cdot \int f(x)\, dx.
\end{aligned}
$$
En un lenguaje más formal, al cumplirse las igualdades de arriba, se dice que la integral posee la propiedad de *linealidad* 

## Relación entre la integral indefinida y la derivada

Por como es definida la integral indefinida, tenemos las siguientes consecuencias:

1. La antiderivada de la derivada de una función es la misma función más la constante de integración. En otras palabras: $$\int f'(x)dx=f(x)+C.$$

2. La derivada de la antiderivada de una función es la misma función. En otras palabras: $$\frac{d}{dx}\int f(x)dx=f(x).$$

Observación importante En resumen, la derivada y la integral indefinida son operaciones inversas una de la otra.

## El problema del valor inicial

##
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMzIwMzMyMDc4LC0xNDQ1NTgzMDczLC0yMT
Q0MDQ3ODE4XX0=
-->