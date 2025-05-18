# README - Análise de Dados de Clientes da Olist

Este código realiza uma análise inicial e limpeza básica do conjunto de dados `olist_customers_dataset.csv`, que contém informações sobre clientes da Olist.

## Objetivo
O objetivo deste script é:
1. Carregar e explorar os dados de clientes
2. Realizar limpeza e pré-processamento básico dos dados
3. Preparar os dados para análises mais avançadas

## Funcionalidades

### 1. Carregamento e Exploração Inicial
- Carrega o dataset usando pandas
- Mostra as primeiras linhas do dataframe (`head()`)
- Exibe informações sobre a estrutura dos dados (`info()`)
- Apresenta estatísticas descritivas (`describe()`)

### 2. Limpeza de Dados
- Verifica e remove valores nulos (`isnull().sum()`)
- Identifica e remove duplicatas (`duplicated().sum()`)
- Verifica se há IDs de clientes duplicados (que deveriam ser únicos)

### 3. Padronização de Dados
- Normaliza nomes de cidades e estados para maiúsculas
- Padroniza códigos postais para strings com 5 dígitos (preenchendo com zeros à esquerda se necessário)

## Como Usar
1. Certifique-se de ter o arquivo `olist_customers_dataset.csv` no mesmo diretório
2. Instale as dependências necessárias: pandas e numpy
3. Execute o script

## Dependências
- Python 3.x
- pandas
- numpy

## Saída
O script imprime no console:
- Uma amostra dos dados
- Informações sobre a estrutura dos dados
- Estatísticas descritivas
- Verificação de valores nulos
- Verificação de duplicatas
- Valores únicos de estados

O dataframe resultante terá:
- Dados limpos e padronizados
- Sem duplicatas
- Formatos consistentes para cidades, estados e códigos postais

## Próximos Passos
Este script prepara os dados para análises mais avançadas, como:
- Análise geográfica de clientes
- Segmentação de clientes
- Integração com outros datasets da Olist