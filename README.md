# Desigualdade nas notas do ENEM por raça e gênero

Trabalho de conclusão de curso que analisa os microdados do ENEM para medir as diferenças de desempenho entre grupos raciais e de gênero e como elas mudaram ao longo do tempo.

## Pergunta

Como as notas do ENEM, principalmente em Matemática, variam entre grupos de raça/cor e sexo, e qual o peso de fatores socioeconômicos (renda familiar, escolaridade dos pais e acesso à internet) nessas diferenças?

## Dados

- **Fonte:** [Microdados do ENEM, INEP](https://www.gov.br/inep/pt-br/acesso-a-informacao/dados-abertos/microdados/enem)
- **Edições analisadas:** 2011, 2018 e 2020
- **Volume:** mais de 5 milhões de inscritos por edição
- **Variáveis principais:** notas das quatro áreas (`NU_NOTA_MT`, `NU_NOTA_LC`, `NU_NOTA_CH`, `NU_NOTA_CN`), sexo (`TP_SEXO`), raça/cor (`TP_COR_RACA`) e questionário socioeconômico (`Q001`, `Q002`, `Q006`, `Q025`)

Os arquivos originais não estão no repositório por causa do tamanho. Para rodar, baixe os microdados no site do INEP.

## Método

1. Leitura seletiva das colunas necessárias, para lidar com arquivos de vários GB
2. Limpeza, tratamento de ausentes e codificação de variáveis categóricas (one-hot)
3. Comparação de médias e medianas por grupo de raça e sexo em cada edição
4. Diferença de notas em relação a um grupo de referência e evolução entre 2011, 2018 e 2020
5. Regressão linear para estimar a relação entre fatores socioeconômicos e a nota de Matemática em cada grupo
6. Teste exploratório com rede neural (Keras)

## Tecnologias

Python · Pandas · NumPy · scikit-learn · TensorFlow/Keras · Matplotlib · Seaborn · Google Colab

## Estrutura

```
analise_desigualdade_enem.ipynb   notebook principal com a análise consolidada
rascunhos/                        versões exploratórias usadas durante o desenvolvimento
```

## Autora

Rita Farias · [LinkedIn](https://www.linkedin.com/in/rita-farias-b24a33232/)
