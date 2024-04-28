# Notações de Conjunto em LaTeX

Todo o código foi formulado durante o curso de Introdução ao Latex do Professor **Aquino** onde são demostrados exemplos detalhados como representar conjuntos, realizar operações como intersecção, união e diferença, classificar proposições como verdadeiro ou falso, e utilizar quantificadores universais e existenciais.

**1. Representação de Conjuntos:**

Para representar conjuntos em LaTeX, utiliza-se os colchetes `\{` e `\}` para listar os elementos entre vírgulas. Utilize `\in` para indicar que um elemento pertence ao conjunto e `\notin` para indicar que não pertence.

**Exemplo:**

```latex
Sejam os conjuntos $A = \{1;\, 2;\, 3;\, 4\}$, $B = \{x \in \mathbb{Z} \, |\, -2 \leq x < 4\}$ e $C = \{x \in \mathbb{N} \, |\, x \geq 2\}$.
```

**2. Operações com Conjuntos:**

* **Intersecção:** Utiliza-se o símbolo `\cap` para representar a intersecção de conjuntos (elementos que pertencem a ambos os conjuntos).

```latex
$A \cap B$
```

* **União:** Utiliza-se o símbolo `\cup` para representar a união de conjuntos (elementos que pertencem a pelo menos um dos conjuntos).

```latex
$B \cup C$
```

* **Diferença:** Utiliza-se o símbolo `-` para representar a diferença de conjuntos (elementos que pertencem ao primeiro conjunto, mas não ao segundo).

```latex
$A - C$
```

* **Diferença Simétrica:** Utiliza-se o símbolo `\setminus` para representar a diferença simétrica de conjuntos (elementos que pertencem a apenas um dos conjuntos).

```latex
$C \setminus B$
```

**3. Classificando Proposições:**

Para classificar proposições como verdadeiro ou falso em LaTeX, utilize a estrutura a seguir:

```latex
\begin{enumerate}
\item Classifique em verdadeiro ou falso:
\begin{enumerate}
\item ... (proposição 1)
\item ... (proposição 2)
\item ... (proposição n)
\end{enumerate}
\end{enumerate}
```

**Exemplo:**

```latex
\begin{enumerate}
\item Classifique em verdadeiro ou falso:
\begin{enumerate}
\item $\mathbb{Z} \subset \mathbb{N}$
\item $\mathbb{R} \supset \mathbb{Q}$
\item $\mathbb{Z} \not\subset \mathbb{N}$
\item $\mathbb{R} \not\supset \mathbb{Q}$
\item $0 \not\in \mathbb{R} \setminus\mathbb{Q}$
\item $\forall z \in \mathbb{N}$, temos $x \geq 0$
\item $\exists x \in \mathbb{R}$, tal que $\sqrt{x} \not\in\mathbb{R}$
\item $7 \not\in \{x\in \mathbb{N} \,|\, x \textrm{ par}\}$
\item $-5 \in \mathbb{R}^*_+$
\item $0 \in \varnothing$
\end{enumerate}
\end{enumerate}
```

**4. Quantificadores:**

* **Quantificador Universal (∀):** Utiliza-se o símbolo `\forall` para representar o quantificador universal "para todo".

```latex
$\forall z \in \mathbb{N}$, temos $x \geq 0$
```

* **Quantificador Existencial (∃):** Utiliza-se o símbolo `\exists` para representar o quantificador existencial "existe pelo menos um".

```latex
$\exists x \in \mathbb{R}$, tal que $\sqrt{x} \not\in\mathbb{R}$
```

**Observações:**

* Utiliza-se o pacote `amsmath` para ter acesso aos símbolos matemáticos e comandos específicos para conjuntos e operações matemáticas.
* Para formatar equações complexas, utiliza-se o ambiente `equation`.
* Seja consistente na utilização da formatação para manter a clareza e organização do seu documento.
