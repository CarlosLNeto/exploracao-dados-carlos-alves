# Análise de Pontualidade de Voos no Brasil - Dezembro/2024

Este repositório contém uma análise exploratória de dados (EDA) sobre a pontualidade e regularidade dos voos da aviação civil no Brasil, utilizando dados públicos fornecidos pela Agência Nacional de Aviação Civil (ANAC).

## 🌟 Destaques da Análise

#### O que motivou a escolha do dataset?
O tema de atrasos e cancelamentos de voos é de grande interesse público e de fácil compreensão. Os dados da ANAC são uma fonte confiável, pública e granular, permitindo uma análise prática e relevante sobre a eficiência de um setor crítico para a infraestrutura do país.

#### As análises mais relevantes realizadas:
1.  **Análise de Distribuição com Histogramas:** Para visualizar a frequência dos percentuais de atraso e cancelamento, entendendo o que é "normal" versus o que é "raro".
2.  **Detecção de Outliers com Boxplots:** Para identificar rapidamente os voos com desempenho significativamente pior que a média, que representam os casos mais críticos.
3.  **Análise de Correlação com Gráfico de Dispersão:** Para investigar a relação entre atrasos moderados (> 30 min) e atrasos severos (> 60 min).

#### Os principais insights obtidos:
* **A Pontualidade é a Norma:** A grande maioria dos voos opera com um índice de problemas muito baixo (próximo de 0%). A operação padrão da aviação no período foi marcadamente eficiente.
* **O Problema está nos Outliers:** Os problemas de desempenho não são generalizados. Em vez disso, são **concentrados em um número específico de voos problemáticos** que falham de forma consistente e representam os principais pontos de atenção para as companhias.
* **Atrasos Tendem a Escalar:** Voos que são propensos a atrasos moderados (> 30 min) também são os que têm maior probabilidade de sofrer atrasos extremos (> 60 min), indicando que as causas dos atrasos, quando não mitigadas, tendem a se agravar.

---

## 1. Sobre o Projeto

O objetivo principal é entender os padrões de atrasos e cancelamentos de voos, identificar irregularidades e extrair insights sobre o desempenho operacional das companhias aéreas em um período específico (Dezembro de 2024).

A análise foi conduzida em um ambiente SageMaker Studio Lab, utilizando Python e as principais bibliotecas de Data Science.

## 2. Fonte dos Dados

* **Nome do Dataset:** Percentuais de Atrasos e Cancelamentos de Voos (Voo Regular)
* **Órgão Responsável:** Agência Nacional de Aviação Civil (ANAC)
* **Link para o Conjunto de Dados:** [Portal Brasileiro de Dados Abertos - ANAC](https://www.gov.br/anac/pt-br/dadosabertos/Voos-e-operacoes-aereas/Percentuais-de-atrasos-e-cancelamentos/)
* **Arquivo Utilizado:** `Anexo I.csv`, que contém os dados mais granulares, detalhando a performance por número de voo.

## 3. Como Executar a Análise

Para replicar este projeto, siga os passos abaixo:

### Pré-requisitos

É necessário ter Python 3 instalado, juntamente com as seguintes bibliotecas:
* pandas
* numpy
* matplotlib
* seaborn

Você pode instalar todas as dependências com o seguinte comando:
```bash
pip install pandas numpy matplotlib seaborn