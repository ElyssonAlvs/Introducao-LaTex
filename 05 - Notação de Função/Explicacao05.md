# Notações de Função em LaTeX

Todo o código foi formulado durante o curso de Introdução ao Latex do Professor **Aquino** onde são demostrados exemplos detalhados como definir funções, especificar seus domínios e contradomínios, e utilizar a estrutura de casos para funções piecewise (definidas por partes).

**1. Definição de Função:**

Para definir uma função `f`, utiliza-se a seguinte estrutura:

```latex
f : \mathbb{R} \to \mathbb{R} \quad \text{onde } f(x) = \text{expressão}
```

* `f`: nome da função
* `\mathbb{R} \to \mathbb{R}`: indica o domínio (conjunto de valores de entrada) e o contradomínio (conjunto de valores de saída) da função, ambos os reais neste caso.
* `f(x)`: representa o valor da função `f` para uma entrada `x`.
* `\text{expressão}`: representa a regra de correspondência da função (fórmula que define o valor de saída para cada entrada).

**Exemplo:**

```latex
Seja a função $f : \mathbb{R} \to \mathbb{R}$ definida por $f(x) = \dfrac{1}{2}x^2 - 2x + 1.
```

**2. Funções Piecewise (Definidas por Partes):**

Para funções definidas por partes, utiliza-se a estrutura `\begin{cases} ... \end{cases}`:

```latex
f : \mathbb{R} \to \mathbb{R} \quad \text{onde } f(x) =
\begin{cases}
\text{expressão 1}; \quad \text{condição 1} \\
\text{expressão 2}; \quad \text{condição 2} \\
\text{ ... }
\end{cases}
```

* Cada linha dentro do `cases` define uma regra para um determinado intervalo de entrada.
* As condições determinam em quais valores de `x` cada expressão se aplica.

**Exemplos:**

```latex
$$f : \mathbb{R} \to \mathbb{R}$$
$$f(x) = 
\begin{cases}
x^2 - 1; \, x \geq 1 \\
x - 3 ; \, x < 1 \\
2x + 1; \, x < -1
\end{cases}
$$

$$f : \mathbb{R} \to \mathbb{R}$$
$$f(x) = 
\begin{cases}
x^2 - 1; \,\textrm{se } x \geq 1 \\
x - 3 ; \,\textrm{se } x < 1 \\
2x + 1; \,\textrm{se } x < -1
\end{cases}
$$
```

**3. Funções Comuns:**

Para funções predefinidas como exponencial, logarítmica, trigonométricas e outras, utiliza-se os comandos específicos:

* Função exponencial: `f(x) = 2^{x-1}` ou `f(x) = \exp(x-1)`
* Função logarítmica: `f(x) = \log_2 x` (logaritmo na base 2) ou `f(x) = \ln x` (logaritmo natural)
* Funções trigonométricas: `f(x) = \cos x`, `f(x) = \sin x`, `f(x) = \tan x`

**Exemplo:**

```latex
$$f : \mathbb{R} \to \mathbb{R}$$
$$f(x) = \cos x
$$
```
**4. Observações sobre Sintaxe:**

* Utiliza-se espaços para melhorar a legibilidade entre variáveis, operadores e símbolos matemáticos.
* Para funções trigonométricas com deslocamentos, você pode utilizar `\sin \left(x - \frac{\pi}{2}\right)`, `\sen \left[x - \frac{\pi}{2}\right]`, ou `\sen \left\{x - \frac{\pi}{2}\right\}`. Os colchetes e chaves são equivalentes neste caso.
