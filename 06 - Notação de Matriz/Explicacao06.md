# Notações de Matriz em LaTeX

Todo o código foi formulado durante o curso de Introdução ao Latex do Professor **Aquino** onde são demostrados exemplos detalhados como definir a criar matrizes com diferentes dimensões, calcular determinantes, inversas e transpostas, resolver sistemas lineares e utilizar a simbologia correta para cada tipo de objeto matemático.

**1. Criando Matrizes:**

Para criar matrizes em LaTeX, utilize o ambiente `bmatrix`:

```latex
\begin{bmatrix}
elemento_{11} & elemento_{12} & \cdots & elemento_{1n} \\
elemento_{21} & elemento_{22} & \cdots & elemento_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
elemento_{m1} & elemento_{m2} & \cdots & elemento_{mn}
\end{bmatrix}
```

* Dentro dos colchetes, cada linha é representada por uma sequência de elementos separados por espaços.
* Utilize `\cdots` para indicar que a linha continua com mais elementos do mesmo tipo.
* O número de linhas `m` e colunas `n` da matriz é definido pelo número de linhas e colunas dentro dos colchetes, respectivamente.

**Exemplo:**

```latex
Considere a matriz
$M = \begin{bmatrix}
1 & 10 & -5 \\
6 & 7 & 8
\end{bmatrix}$
```

**2. Operações com Matrizes:**

* **Determinante:** Utilize o comando `\det` para calcular o determinante de uma matriz:

```latex
\det M
```

* **Inversa:** Utilize o comando `M^{-1}` para calcular a inversa de uma matriz:

```latex
M^{-1}
```

* **Transposta:** Utilize o comando `M^T` para calcular a transposta de uma matriz:

```latex
M^T
```

**Exemplo:**

```latex
\begin{enumerate}
\item $\det M$
\item $M^{-1}$
\item $M^T$
\end{enumerate}
```

**3. Sistemas Lineares:**

Para resolver sistemas lineares em LaTeX, utilize o ambiente `equation` e a simbologia correta para matrizes e vetores:

```latex
\begin{equation}
\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mn}
\end{bmatrix}
\begin{bmatrix}
x \\
y \\
\vdots \\
z
\end{bmatrix}
=
\begin{bmatrix}
b_1 \\
b_2 \\
\vdots \\
b_m
\end{bmatrix}
\end{equation}
```

* Dentro dos colchetes à esquerda, a matriz do sistema linear.
* O vetor de variáveis desconhecidas entre colchetes à direita e acima do sinal de igual.
* O vetor de termos independentes entre colchetes à direita do sinal de igual.

**Exemplo:**

```latex
\begin{enumerate}
\item Determine $x$, $y$ e $z$ na equação
$$\begin{bmatrix}
1 & -2 & 4 \\
5 & -2 & -2 \\
6 & 1 & 8 
\end{bmatrix}
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
=
\begin{bmatrix}
2 \\
10 \\
6
\end{bmatrix}
$$
\end{enumerate}
```

**4. Simbologia Correta:**

* **Colchetes:** Utiliza-se `\begin{bmatrix}` e `\end{bmatrix}` para representar colchetes de matrizes.
* **Parênteses:** Utiliza-se `\begin{pmatrix}` e `\end{pmatrix}` para representar parênteses de vetores.
* **Barra vertical:** Utiliza-se `|` para representar a barra vertical utilizada em determinantes.
* **Declaração de objetos lineares:** Utiliza-se `\begin{bmatrix}` e `\end{bmatrix}` para colchetes de matrizes e `\begin{pmatrix}` e `\end{pmatrix}` para parênteses de vetores, trocando a primeira letra (b, p, v) para indicar o tipo de vetor.
