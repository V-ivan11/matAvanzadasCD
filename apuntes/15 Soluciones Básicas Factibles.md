# Soluciones básicas factibles

En esta parte del curso abordaremos a los puntos extremos desde un punto de vista algebraico.

## Definición

> Considere el sistema $Ax=b$ y $x \ge 0$ donde $A$ es una matriz de dimensión $m\times n$ y b un vector de dimensión $m$. Supongamos que el $rango(A,b)=rango(A)=m$.

Después de reacomodar (posiblemente) las columnas de $A$, sea $A= [B,N]$ donde $B$ es una matriz de dimensión $m\times n$ invertible y $N$ es una matriz de dimensión $m\times (n-m)$ 
$$
\\
\\mA^n = nB^m nN^{n-(m)}
$$
 El punto 
$$
x =
\begin{bmatrix}
 x_B \\
 x_N \\
\end{bmatrix},\\\\
X_B = B^{-1}b \\
X_N = 0
$$
donde estrictamente una solución básica del sistema. Si $X_b \ge 0$
$$
Ax = [B,N]
\begin{bmatrix}
 x_B \\
 x_N \\
\end{bmatrix} = Bx_B + N X_N = BB^{-1}b + N0=b
$$
entonces $X_B$ es llamada la **solución básica factible**. En este caso $B$ es llamada la matriz básica y $N$ la matriz no básica. Las componentes de $X_B$ son llamadas variables básicas y las componentes de $X_N$ variables no básicas. Si $x_B \ge 0$, entonces $X$  es llamada **no degenerada**, si al menos una de las entradas de $X_B = 0$ entonces es llamada solución **degenerada**.

### Ejemplo

Considere el poliedro definido por las siguientes desigualdades:
$$
x_1+x_2\le 6\\
x_2\le 3\\
x_1,x_2\ge0
$$
Introduciendo variables de oleura:
$$
\begin{eqnarray*}
x_1+x_2+x_3 &=& 0\\
x_2+0+x_4 &=& 3\\
\end{eqnarray*}
$$

$$
X =
\begin{bmatrix}
 x_1 \\
 x_2 \\
 x_3\\
 x_4
\end{bmatrix}
\ge 0\\
Ax = b\\\\
\begin{bmatrix}
1 & 1 & 1 & 0\\
0 & 1 & 0 & 1
\end{bmatrix}x =\begin{bmatrix}6\\3\end{bmatrix}
\\
B \qquad N \qquad \qquad
\\
X = \begin{bmatrix}x_B\\X_N\end{bmatrix} = \begin{bmatrix}B\\0\end{bmatrix} = \begin{bmatrix}6\\3\\0\\0\end{bmatrix}
$$

Para una matriz de dimensión $m\times n$ arbitraria podemos considerar, a lo más $\binom{n}{m}$.

## Correspondencia entre soluciones factibles y puntos extremos

Veamos que un punto es una solución básica factible si y sólo si es un punto extremo.

Consideremos el siguiente problema lineal

| Minimizar | $cx$               |
| --------- | ------------------ |
| Sujeto a  | $$Ax=b \\ x\ge 0$$ |

Donde $A$ es una de la matriz de dimensión $m\times n$ con rango $m$. Sea $X$ un punto extremo de la región factible, veamos que $x$ es solución básica factible de $Ax=b, \quad x\ge 0$. Consideramos $x_1, x_2, \cdots, x_p$ las entradas de $x>0$ y $x_{p+1}, \cdots, x_n$ las entradas de $x = 0$. Veamos que $a_1, a_2, \cdots, a_p$ columnas de $A$ , son linealmente independientes.

Si estos vectores no son linealmente independientes, entonces existen escalares $\gamma_1,\gamma_2,\cdots,\gamma_p$ no todos 0 tal que
$$
\sum_{j=0}^n\gamma_ja_j = 0
$$
Exhibiremos 2 puntos de la región factible distintos tales que una de sus combinaciones lineales estricta es igual a $x$.

Defina $x',x''$ donde 
$$
x_j' = \left\lbrace
\begin{array}{ll}
x_j + \lambda \gamma_j \qquad j = 1,2,\cdots,p\\
0 \qquad j = p+1,\cdots,n 
\end{array}\right. \\ \\
x_j'' = \left\lbrace
\begin{array}{ll}
x_j - \lambda \gamma_j \qquad j = 1,2,\cdots,p\\
0 \qquad j = p+1,\cdots,n 
\end{array}\right. \\
$$

$$
\Gamma_m = \max_j \{|\gamma_j|\} > 0 \qquad \text{hint: l.i.}\\
X_{\min}=\min_j\{x_j\}\\\\
\lambda=\frac{X_{\min}}{\Gamma_m} \ge 0
$$

Luego
$$
x_j + \lambda\gamma_j \ge x_j \ge 0\\\\
x_j + \frac{x_{\min}\gamma_j}{\Gamma_m} \ge x_j-x_{\min} \qquad \gamma_j > 0 \quad\gamma\le0
$$
El aumento de precios desde la pandemia ha afectado el alza de precios de la canasta básica en la Ciudad de México para mejorar la dieta en general de los mexicanos.

