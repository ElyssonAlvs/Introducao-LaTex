# Listas e Operações Básicas em LaTeX

Todo o código foi formulado durante o curso de Introdução ao Latex do Professor **Aquino** onde são demostrados exemplos detalhados para numerar itens sequencialmente, criar subitens, inserir marcadores, realizar operações matemáticas simples como adição, subtração, multiplicação, divisão e potenciação, além de representar raízes quadradas, cúbicas e de qualquer ordem, e formatar índices.

**1. Listas Numeradas:**

Para criar listas numeradas, utiliza-se o ambiente `enumerate`:

```latex
\begin{enumerate}
    itens
    \item mais outro texto.
    \begin{enumerate}
        subitens
        \item{aqui vem o texto}
        \item{aqui vem o texto}
            \begin{enumerate}
                  \item{outro texto}
                \end{enumerate}
    \end{enumerate}
    \item vem o texto.
    \item vem o texto.
    \item outro texto.
\end{enumerate}
```

**Exemplo:**

1. itens
   1. mais outro texto.
      1. aqui vem o texto
      2. aqui vem o texto
         1. outro texto
   2. vem o texto.
   3. vem o texto.
   4. outro texto.

**2. Listas com Marcadores:**

Para criar listas com marcadores, utiliza-se o ambiente `itemize`:

```latex
\begin{itemize}
    bolinha
    \item isso aqui é um item.
    \item isso aqui é outro item.
        \begin{itemize}
            \item não sei oque.
            \item ainda não sei.
            \item sei lá.
        \end{itemize}
    \item mais outro item.
\end{itemize}
```

**Exemplo:**

* bolinha
  * isso aqui é um item.
  * isso aqui é outro item.
    * não sei oque.
    * ainda não sei.
    * sei lá.
  * mais outro item.

**3. Operações Matemáticas Básicas:**

As operações matemáticas básicas podem ser representadas diretamente no texto utilizando os símbolos matemáticos correspondentes:

* Adição: `a + b`
* Subtração: `a - b`
* Multiplicação: `a \cdot b` ou `a \times b`
* Divisão: `a \div b`
* Fração: `\frac{a}{b}` ou `\dfrac{a}{b}`
* Potência: `a^b`

**Exemplo:**

$a + b$

$a - b$

$a\cdot b$

$a \times b$

$a \div b$

isso é uma fração $\frac{a}{b}$

uma linha de tsta para ver como fica

isso é uma fração $\dfrac{a}{b}$

**4. Raízes e Potências:**

As raízes e potências podem ser representadas utilizando os comandos específicos:

* Raíz quadrada: `\sqrt{a}`
* Raíz cúbica: `\sqrt[3]{a}`
* Raíz de qualquer ordem: `\sqrt[n]{a}`

**Exemplo:**

$\sqrt{a}{b}$

$\sqrt[3]{a}$

$\sqrt[8]{a}$

**5. Índices:**

Os índices podem ser representados utilizando a notação `a_i`, onde `i` é o índice desejado.

**Exemplo:**

$a_1$, $a_2$, $a_3$ e $a_4$

$a_{10}$, $a_{20}$

**Observações:**

* Utiliza-se o espaço antes e depois dos símbolos matemáticos para melhor legibilidade.
* Para operações mais complexas, utiliza-se o ambiente `equation` para formatar a equação em uma linha separada.
* Explore os pacotes `amsmath`, `amsfonts` e `amssymb` para obter mais símbolos matemáticos e recursos avançados de formatação.
