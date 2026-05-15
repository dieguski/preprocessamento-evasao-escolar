# Pré-processamento de Dados — Evasão Escolar

Pipeline completo de pré-processamento de um dataset educacional bruto,
preparando-o para uso em modelos de machine learning.

## Contexto

Dataset com 153 registros de estudantes de ensino superior, contendo
informações socioeconômicas e acadêmicas em estado bruto — com duplicatas,
valores nulos, outliers e inconsistências de texto.

## Objetivo

Transformar o dataset bruto em um dataset limpo, padronizado e codificado,
pronto para ser utilizado como input em um modelo preditivo de evasão escolar.

## Tecnologias utilizadas

- Python
- pandas

## Etapas do pipeline

1. Carregamento e análise inicial do dataset
2. Remoção de coluna duplicada e linhas duplicadas
3. Tratamento de valores nulos com estratégia adequada por coluna
4. Identificação e substituição de outliers pela mediana
5. Padronização de valores categóricos inconsistentes
6. Criação de variáveis derivadas (Faixa Etária, Renda Normalizada)
7. Encoding: mapeamento ordinal para Faixa Etária, OHE para demais categóricas
8. Definição da variável target (Status → binário)
9. Exportação do dataset tratado em CSV

## Arquivos

| Arquivo | Descrição |
|---|---|
| `pre_processamento_evasao_escolar.ipynb` | Pipeline completo de pré-processamento |
| `base_aed_evasao_pre_processamento.xlsx` | Dataset bruto de entrada |
| `base_aed_evasao_pre_processamento_tratada.csv` | Dataset tratado exportado |
