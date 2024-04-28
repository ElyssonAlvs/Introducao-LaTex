# Notações de Geometria Analítica em LaTeX: Um Tutorial

Todo o código foi formulado durante o curso de Introdução ao Latex do Professor **Aquino** onde são demostrados exemplos detalhados como definir representar segmentos de reta, vetores, planos, produto escalar, produto vetorial, ângulo entre vetores e norma de um vetor.

**1. Segmentos de Reta e Vetores:**

* Segmento de reta $\overline{AB}$: utiliza-se a barra sobre a letra.
* Vetor orientado $\overrightarrow{AB}$: utiliza-se a seta sobre a letra maiúscula.
* Vetor não-orientado $\vec{u}$: utiliza-se a seta sobre a letra minúscula.

**Exemplo:**

```latex
Seja o segmento $\overline{AB}$. A partir dele podemos definir os segmentos orientados $\overrightarrow{AB}$ e $\overrightarrow{AB}$. Seja $\vec{u}$ e $\vec{v}$.
```

**2. Ortogonalidade de Vetores:**

Para verificar se dois vetores $\vec{u}$ e $\vec{v}$ são ortogonais (perpendiculares), utilize o símbolo $\vec{u} \perp \vec{v}$.

**Exemplo:**

```latex
Sejam os vetores $\vec{u} = (1;\, -1;\, 2)$ e $\vec{v} = (2;\, 5;\, -4)$. Verifique se $\vec{u} \perp \vec{v}$.
```

**3. Planos:**

Para representar um plano, utiliza-se a equação geral:

```latex
ax + by + cz + d = 0
```

onde `a`, `b`, `c` e `d` são constantes reais e representam os coeficientes do plano.

**Exemplo:**

```latex
Sejam os planos $\alpha : x - 2y + 6z - 3 = 0$ e $\beta : x - 2y + 6z - 3 = 0$.
```

**4. Produto Escalar e Vetorial:**

* **Produto Escalar:** representado por $\vec{u} \cdot \vec{v}$ (escalar).
* **Produto Vetorial:** representado por $\vec{u} \times \vec{v}$ (vetor).

Para o produto vetorial, utilize o determinante de terceira ordem com base matricial:

```latex
\vec{u} \times \vec{v} = 
\begin{vmatrix}
\vec{i} & \vec{j} & \vec{k} \\
x_0 & y_0 & z_0 \\
x_1 & y_1 & z_1
\end{vmatrix}
```

onde:

* $\vec{i}$, $\vec{j}$, $\vec{k}$ são os vetores unitários ortogonais representando os eixos cartesianos.
* $(x_0, y_0, z_0)$ e $(x_1, y_1, z_1)$ são as componentes dos vetores $\vec{u}$ e $\vec{v}$, respectivamente.

**5. Outras Operações Vetoriais:**

* Produto interno: utilize `< \vec{u},\, \vec{v} >` ou $<\langle\vec{u},\, \vec{v}\rangle>$.
* Norma de um vetor: utilize $||\vec{u}||$, $\|\vec{u}\|$, ou $\left\|\overrightarrow{AB}\right\|$.

**Observações:**

* Utiliza-se o pacote `amsmath` para ter acesso aos símbolos matemáticos específicos.
* Para formatação de matrizes e determinantes, consulte a documentação do pacote `amsmath`.
* Seja consistente na utilização da formatação para manter a clareza e organização do seu documento.
