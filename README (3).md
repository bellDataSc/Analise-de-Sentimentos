# Análise de sentimentos com os roteiros de Rick and Morty

Comecei este estudo no Kaggle para explorar o vocabulário dos diálogos de Rick and Morty com três léxicos: AFINN, Bing e NRC. Ao preparar o case para o **Portfolio Night 2026, em São Paulo**, retomei essa exploração para comunicar melhor o método, os resultados e seus limites.

Este repositório preserva o estudo original e registra essa evolução. Os notebooks usam o mesmo corpus, com objetivos diferentes: exploração inicial e apresentação revisada do case.

## Notebooks

| Arquivo | Papel |
|---|---|
| [Análise_de_Sentimentos.ipynb](Análise_de_Sentimentos.ipynb) | Exploração original, preservada como início do estudo. |
| [Portfolio_Night_2026.ipynb](Portfolio_Night_2026.ipynb) | Atualização do case para o Portfolio Night, com código autônomo, análise revisada e resultados no próprio notebook. |

## O que evoluiu para o Portfolio Night

- Inventário das falas e dos episódios, deixando explícito o recorte disponível.
- Tokenização consistente, com normalização de apóstrofos e preservação de contrações.
- Comparação dos léxicos nas palavras realmente observadas, distinguindo concordância e acurácia.
- Associações emocionais por personagem normalizadas pelo volume de tokens.
- Inspeção das palavras que mais contribuem para as emoções e das divergências entre métodos.
- Teste de sensibilidade às contribuições de `god` e `time`, mantendo o denominador original.
- Demonstração didática do limite da abordagem diante da negação, separada dos resultados do corpus.

## O que os resultados permitem dizer

A versão revisada trabalha com **1.905 falas e 25.371 tokens**, distribuídos por **11 episódios representados no arquivo**. A cobertura lexical varia de **7,2% a 9,1%** das ocorrências de tokens. As tabelas e os cálculos correspondentes estão no notebook atualizado.

Esses números descrevem o corpus disponível. O arquivo contém quantidades desiguais de falas por episódio; um deles tem apenas oito. As associações dos dicionários ajudam a investigar o vocabulário, mas não medem o estado emocional dos personagens nem validam ironia e intenção narrativa.

## Executar o notebook atualizado

O arquivo `Portfolio_Night_2026.ipynb` contém o código necessário para a análise. No Kaggle, use os dois datasets abaixo e execute as células em ordem. Em um ambiente local ou no Colab com Python 3.11 ou posterior, o notebook instala dependências ausentes e baixa automaticamente os dados públicos, conferindo a versão pelos hashes. Os resultados também ficam visíveis no próprio arquivo.

- [Roteiros de Rick and Morty](https://www.kaggle.com/datasets/isabelgonalves/roteiros-de-rick-and-morty)
- [Léxicos utilizados](https://www.kaggle.com/datasets/isabelgonalves/categorizao-de-sentimentos)

## Origem no Kaggle

- [Estudo original — Análise de Sentimentos](https://www.kaggle.com/code/isabelgonalves/an-lise-de-sentimentos)
- [Case — Portfolio Night 2026 — São Paulo](https://www.kaggle.com/code/isabelgonalves/case-portfolio-night-2026-s-o-paulo)

O Kaggle registra a exploração e a apresentação do estudo. O GitHub reúne sua trajetória e a versão revisada para consulta e execução. A revisão entregue neste repositório pode evoluir em relação às versões publicadas no Kaggle.

**Próximos experimentos:** regra de negação, avaliação com falas rotuladas manualmente e comparação com um modelo contextual. Essas etapas ainda não foram realizadas.

**Autora:** Isabel Gonçalves Cruz · [Kaggle](https://www.kaggle.com/isabelgonalves) · [GitHub](https://github.com/bellDataSc)
