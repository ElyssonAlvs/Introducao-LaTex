# Inserindo Figuras e Referenciando-as com Latex

Todo o código foi formulado durante o curso de Introdução ao Latex do Professor **Aquino** onde são demostrados exemplos detalhados como inserir imagens e referenciar elas no Latex.

## 1. Configuração da Página

* `\documentclass[a4paper, 12pt]{article}`: Define o tipo de documento como artigo e configura o tamanho do papel para A4 com fonte de 12pt.
* `\usepackage[top=2cm, bottom=2cm, left=2.5cm, right=2.5cm]{geometry}`: Ajusta as margens do documento (superior, inferior, esquerda e direita) para 2.5cm cada.

## 2. Carregando Pacotes:

Pacotes que são utilizado para escrever o documento:

* `\usepackage[utf8]{inputenc}`: Permite a utilização de caracteres UTF-8 para acentuação e caracteres especiais.
* `\usepackage{amsmath, amsfonts, amssymb}`: Carrega pacotes essenciais para notações matemáticas (amsmath), fontes matemáticas (amsfonts) e símbolos matemáticos (amssymb).
* `\usepackage{graphicx}`: Permite a inclusão de imagens no documento.
* `\usepackage{float}`: Auxilia no posicionamento de figuras e tabelas.
* `\usepackage[portuguese]{babel}`: Configura o idioma do documento para português.

## 3. Iniciando o Documento:

* `\begin{document}`: Marca o início do corpo do documento.

## 4. Inserindo e Referenciando Figuras:

Explicando cada parte do código, temos:

* `\begin{enumerate}`: Inicia uma lista numerada.
    * `\item Calcule o valor de $x$ na Figura \ref{rotulo}.`: Texto descritivo da questão.
    * `\ref{rotulo}`: Referência cruzada à figura identificada pela label `rotulo`.
        *  `\begin{figure}[H]`: Inicia a definição de uma figura. A opção `[H]` indica que a figura deve ser posicionada o mais alto possível na página.
            * `\centering`: Centraliza a figura horizontalmente.
            * `\includegraphics[scale=0.5]{imagem.png}`: Inclui a imagem `imagem.png` e ajusta seu tamanho para 50% do tamanho original (`scale=0.5`).
            * `\caption{Gráfico .}`: Define a legenda da figura.
            * `\label{rotulo}`: Insere uma label `rotulo` para posterior referência.
        * `\end{figure}`: Finaliza a definição da figura.
    * O mesmo procedimento é repetido para a segunda figura, substituindo `rotulo` por `meu-rotulo`.
* `\end{enumerate}`: Finaliza a lista numerada.

## 5. Finalizando o Documento

* `\end{document}`: Marca o final do corpo do documento.

**Observações:**

* Substitua `imagem.png` pelo nome real do arquivo de imagem que você deseja incluir.
* Certifique-se de que o arquivo de imagem está na mesma pasta que o seu código Latex ou em uma pasta acessível pelo Latex.
* Você pode alterar o posicionamento das figuras usando outras opções dentro do comando `[H]`, como `[t]` para o topo da página ou `[b]` para a base.
* É possível ajustar o tamanho da figura alterando o valor de `scale` no comando `\includegraphics`.