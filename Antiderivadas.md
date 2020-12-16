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

- Integrales de monomios

- Integrales de funciones trigonométricas

- Integral del logaritmo y la exponencial

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

## El problema del valor inicial

##
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTIxNDQwNDc4MThdfQ==
-->