# Inserindo tabelas usando Latex

Todo o código foi formulado durante o curso de Introdução ao Latex do Professor **Aquino** onde são demostrados exemplos detalhados como definir tabelas no Latex

## 1. Configuração da Página e Carregamento de Pacotes:

* As primeiras linhas são idênticas ao exemplo anterior, configurando o documento (tamanho A4, fonte 12pt) e carregando pacotes necessários:
    * `[a4paper, 12pt]{article}`
    * `\usepackage[top=2cm, bottom=2cm, left=2.5cm, right=2.5cm]{geometry}`
    * `\usepackage[utf8]{inputenc}`
    * `\usepackage{amsmath, amsfonts, amssymb}`
    * `\usepackage{graphicx}`
    * `\usepackage{float}`
    * `\usepackage[portuguese]{babel}`

## 3. Iniciando o Documento:

* `\begin{document}`: Marca o início do corpo do documento.

## 4. Referenciando a Tabela:

* `\begin{enumerate}`: Inicia uma lista numerada.
*  `\item A tabela \ref{minha-tabela} abaixo representa as derivadas básicas.`: Texto descritivo mencionando a tabela.
    * `\ref{minha-tabela}`: Referência cruzada à tabela identificada pela label `minha-tabela`.

## 5. Inserindo a Tabela:

* `\begin{center}`: Centraliza a tabela.
* `\begin{table}[!htb]`: Inicia a definição de uma tabela. A opção `[!htb]` indica que a tabela deve ser posicionada em qualquer lugar da página (h), no topo da página (t) ou na base da página (b).
    * `\centering`: Centraliza a tabela horizontalmente.
    * `\begin{tabular} ... \end{tabular}`: Define a estrutura da tabela com duas colunas separadas por `||`.
        * A primeira coluna (`{c}`) define o alinhamento central para o texto.
        * A segunda coluna (`{c}`) define o alinhamento central para o texto.
    * `\caption{Tabela Básica de Derivadas.}`: Define a legenda da tabela.
    * `\label{minha-tabela}`: Insere uma label `minha-tabela` para referência posterior.
* `\end{table}`: Finaliza a definição da tabela.
* `\end{center}`: Finaliza o centralizado.

### 6. Finalizando a Lista e o Documento:

* `\end{enumerate}`: Finaliza a lista numerada.
* `\end{document}`: Marca o final do corpo do documento.