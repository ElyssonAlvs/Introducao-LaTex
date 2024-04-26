# Formatação Básica de Texto em LaTeX

Todo o código foi formulado durante o curso de Introdução ao Latex do Professor **Aquino** onde são demostrados exemplos detalhados, como centralizar, alinhar à esquerda e à direita, aplicar negrito, itálico e sublinhado, e até mesmo combinar as formatações para criar efeitos visuais mais complexos.

**1. Estrutura do Documento LaTeX:**

O código LaTeX inicia com a declaração `\documentclass`, que define o tipo de documento (artigo neste caso) e o tamanho da fonte. Em seguida, o pacote `geometry` é importado para configurar as margens da página. O pacote `inputec` garante a codificação correta do texto em português.

```latex
\documentclass[a4paper, 12pt]{article}
\usepackage[top=2cm, bottom=2cm, left=2.5cm, right=2.5cm]{geometry}
\usepackage[utf8]{inputec}
```

**2. Formatação de Parágrafos:**

O texto principal do documento é iniciado com o comando `\begin{document}` e finalizado com `\end{document}`. O comando `\par` indica o início de um novo parágrafo.

**3. Centralização de Texto:**

Para centralizar um parágrafo ou elemento de texto, utiliza-se o ambiente `center`:

```latex
\begin{center}
Texto a ser centralizado
\end{center}
```

**Exemplo:**

```latex
\begin{center}
**Equação polinomial do 2° grau.**
\end{center}
```

**4. Alinhamento à Esquerda e à Direita:**

Os ambientes `flushleft` e `flushright` alinham o texto à esquerda e à direita, respectivamente:

```latex
\begin{flushleft}
Texto alinhado à esquerda
\end{flushleft}

\begin{flushright}
Texto alinhado à direita
\end{flushright}
```

**5. Formatação de Caracteres:**

Para formatar caracteres individuais ou palavras, utiliza-se os comandos específicos para cada estilo:

* **Negrito:** `\textbf{texto em negrito}`
* **Itálico:** `\textit{texto em itálico}`
* **Sublinhado:** `\underline{texto sublinhado}`

**Exemplo:**

```latex
\textbf{\textit{\underline{Equação polinomial do 2° grau.}}}
```

**6. Combinação de Formatações:**

É possível combinar as formatações de caracteres para criar efeitos visuais mais complexos:

```latex
\textbf{\textit{\underline{Equação polinomial do 2° grau.}}}
```

**7. Apresentação de Equações:**

Para apresentar equações matemáticas no LaTeX, utiliza-se o ambiente `equation`:

```latex
\begin{equation}
ax^2 + bx + c = 0
\end{equation}
```

**Exemplo:**

```latex
Uma equação da forma $$ax^2 + bx + c = 0,$$ $a \neq 0$ será chamada de equação
polinomial do 2° grau.
```

**8. Solução da Equação Polinomial do 2° Grau:**

A solução da equação polinomial do 2° grau é apresentada utilizando o ambiente `equation`:

```latex
$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2ac} $$
```

**Observações:**

* O símbolo `\pm` indica "mais ou menos".
* O símbolo `\sqrt{}` representa a raiz quadrada.
* O símbolo `\frac{}{}` é utilizado para frações.
