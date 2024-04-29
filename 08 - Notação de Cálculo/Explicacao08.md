# Notações de Cálculo Diferencial e Integral em LaTeX

Todo o código foi formulado durante o curso de Introdução ao Latex do Professor **Aquino** onde são demostrados exemplos detalhados como definir Limites, Derivadas, Integrais e Somatórios, conceitos básicos no estudo de Cálculo.

**1. Limites:**

* Utiliza-se `\lim_{x \to a}` para representar o limite quando $x$ tende a $a$.
* Vários comandos como `\displaystyle` e `\limits` podem ser usados para ajustar o espaçamento e posicionamento do limite.

**Exemplo:**

```latex
\begin{enumerate}
  \item $\lim_{x \to 1} \dfrac{x^2 - 1}{x - 1}$
  \item $$\lim_{x \to 1} \dfrac{x^2 - 1}{x - 1}$$
  \item $\displaystyle\lim_{x \to 1} \dfrac{x^2 - 1}{x - 1}$
  \item $\limite_{x \to 1} \dfrac{x^2 - 1}{x - 1}$
\end{enumerate}
```

**2. Derivadas:**

* Derivadas representadas por `f'(x)`, `f''(x)`, `f^{(n)}(x)`, ou `\dfrac{df}{dx}`, `\dfrac{d^2f}{dx^2}`, `\dfrac{d^nf}{dx^n}`.

**Exemplo:**

```latex
Seja a função definida por $f(x) = x^2 - \sqrt{x}$. Calcule as derivadas abaixo (clássica).
\begin{enumerate}
  \item $f'$
  \item $f''$
  \item $f'''$
  \item $f^{(iv)}$
  \item $f^{(v)}$
  \item $\dfrac{df}{dx}$
  \item $\dfrac{d^2f}{dx^2}$
  \item $\dfrac{d^3f}{dx^3}$
  \item $\dfrac{d^4f}{dx^4}$
  \item $\dfrac{d^5f}{dx^5}$
\end{enumerate}
```

**3. Derivadas Parciais:**

* Derivadas parciais representadas por `\dfrac{\partial f}{\partial x}`, `\dfrac{\partial^2f}{\partial x^2}`, etc.

**Exemplo:**

```latex
Seja a função definida por $f(x,y) = yx^2 - \sqrt{x} + y^3$. Calcule as derivadas abaixo (Letras gregas).
\begin{enumerate}
  \item $\dfrac{\partial f}{\partial x}$
  \item $\dfrac{\partial ^2f}{\partial x^2}$
  \item $\dfrac{\partial ^3f}{\partial y^3}$
  \item $\dfrac{\partial ^4f}{\partial x^4}$
  \item $\dfrac{\partial ^5f}{\partial y^5}$
  \item $\dfrac{\partial }{\partial x} \left(\dfrac{\partial f}{\partial y}\right) $
\end{enumerate}
```

**4. Integrais:**

* Utiliza-se `\int_a^b f(x) dx` para representar a integral definida de $f$ de $a$ até $b$.
* `\displaystyle` e `\limits` podem ser usados para ajustar o espaçamento e posicionamento.

**Exemplo:**

```latex
\begin{enumerate}
  \item $\int_l^5 x^2\cos x dx$
  \item $$\int_l^5 x^2\cos x \, dx$$
  \item $$\displaystyle\int x^2 \sin x \, dx$$
  \item $$\integral x \cos x^2$$
\end{enumerate}
```

**5. Somação:**

* Utilize `\sum_{i=1}^n a_i` para representar a somatória de $a_i$ de $i = 1$ até $n$.

**Exemplo:**

```latex
\begin{enumerate}
  \item $\int_l^5 x^2\cos x dx$
  \item $$\sum_{i=1}^n a_i$$
\end{enumerate}
```

**Observações:**

* Utilize o pacote `amsmath` para ter acesso aos símbolos matemáticos específicos.
* Para formatação de limites e integrais, consulte a documentação do pacote `amsmath`.
