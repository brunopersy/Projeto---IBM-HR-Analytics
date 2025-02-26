# Análise de Desempenho e Rotatividade de Funcionários - IBM HR Analytics

## Visão Geral

Este projeto aborda a análise da rotatividade de funcionários ( *churn* ) utilizando um conjunto de dados de RH. A rotatividade de funcionários é um problema relevante para organizações, e esta análise visa identificar os principais fatores que contribuem para essa rotatividade. O objetivo é obter *insights* que possam ajudar a organização a reduzir a rotatividade e melhorar a retenção de funcionários.

## Bibliotecas Utilizadas

Esta análise utiliza as seguintes bibliotecas Python:

*   **pandas**: Para manipulação e análise de dados, especialmente trabalhando com DataFrames.
*   **seaborn**: Para visualização de dados estatísticos.
*   **matplotlib**: Para criar gráficos estáticos, interativos e animados.
*   **numpy**: Para computação numérica e operações com *arrays*.
*   **hvplot**: Para visualização interativa de dados.

## Fonte de Dados

O conjunto de dados usado nesta análise é o `WA_Fn-UseC_-HR-Employee-Attrition.csv`. Ele contém informações sobre diversos atributos de funcionários, incluindo dados demográficos, informações relacionadas ao trabalho e detalhes sobre o ambiente de trabalho.

## Etapas da Análise

A análise é conduzida em um *notebook* Jupyter, e as principais etapas são as seguintes:

1.  **Carregamento de Dados e Configuração**: Carregamento das bibliotecas necessárias, configuração de estilos de gráficos, formatos numéricos e carregamento do conjunto de dados em um DataFrame do `pandas`.

2.  **Análise Exploratória de Dados (EDA)**:
    *   Verificação do formato do conjunto de dados.
    *   Verificação de dados ausentes.
    *   Exploração de tipos de dados e estatísticas descritivas.
    *   Identificação e análise de *outliers* (valores discrepantes) usando o método do Intervalo Interquartil (IQR).
    *   Visualização de *outliers* usando *boxplots*.
    *   Análise de valores únicos em cada coluna.
    *   Remoção de colunas desnecessárias.

3.  **Engenharia de Atributos e Pré-processamento**:
    *   Separação de colunas categóricas e numéricas.
    *   Codificação da variável alvo `Attrition` em valores numéricos.

4.  **Visualização de Dados**:
    *   Visualização da distribuição de atributos-chave em relação à rotatividade de funcionários usando histogramas interativos.
    *   Criação de uma matriz de correlação para entender as relações entre atributos numéricos usando um mapa de calor.

5.  **Principais Descobertas**:
    A análise identifica vários fatores que influenciam a rotatividade:
    *   **Nível do Cargo, Renda Mensal, Anos na Empresa, Total de Anos de Trabalho**: Funcionários com níveis de cargo mais baixos, renda mensal menor e menos tempo de trabalho têm maior probabilidade de sair.
    *   **Viagens a Trabalho**: Funcionários que viajam frequentemente têm maior probabilidade de rotatividade.
    *   **Departamento**: Funcionários do setor de Pesquisa e Desenvolvimento têm maior probabilidade de permanecer na empresa.
    *   **Área de Formação**: Funcionários com formação em Recursos Humanos e áreas Técnicas apresentam maiores taxas de rotatividade.
    *   **Gênero**: Homens têm maior probabilidade de sair.
    *   **Função**: Técnicos de Laboratório, Representantes de Vendas e funcionários de RH apresentam maiores taxas de rotatividade.
    *   **Estado Civil**: Funcionários solteiros têm maior probabilidade de sair.
    *   **Horas Extras**: Funcionários que trabalham horas extras têm maior probabilidade de sair.
    *   **Observação**: A análise constatou que *Satisfação com o Ambiente, Satisfação com o Trabalho, Avaliação de Desempenho* e *Satisfação com Relacionamentos* não parecem ter um impacto significativo na rotatividade de funcionários.

## Conclusões

A análise sugere que fatores como remuneração mais baixa, oportunidades de crescimento limitadas, equilíbrio entre vida pessoal e profissional e determinadas funções contribuem significativamente para a rotatividade de funcionários. A organização deve considerar estratégias para lidar com essas questões, a fim de melhorar a retenção de funcionários.

## Como Utilizar

1.  Certifique-se de ter o Python 3.6+ instalado.
2.  Instale as bibliotecas necessárias usando:
3.  Execute o *notebook* Jupyter `seu_notebook.ipynb` para reproduzir a análise.

## Trabalhos Futuros

Trabalhos adicionais poderiam incluir:

*   Construção de modelos preditivos para rotatividade de funcionários.
*   Investigação do impacto de fatores adicionais, como equilíbrio entre vida pessoal e profissional, níveis de estresse e funções mais específicas.
*   Implementação de um painel para monitorar a rotatividade de funcionários em tempo real.
*   Aplicar técnicas de redução de dimensionalidade para otimizar ainda mais a análise e melhorar o tempo de treinamento do modelo.

## Autor

Bruno Eduardo p. da Silva
