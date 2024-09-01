# Análise de Sentimentos em Dados Olimpiadas_Paris_2024

## Descrição do Projeto

Este projeto visa realizar a análise de sentimentos em um conjunto de dados textuais, utilizando técnicas de processamento de linguagem natural (NLP) e aprendizado de máquina. O objetivo é identificar se o sentimento expresso nos textos é positivo ou negativo, implementando um modelo de classificação baseado em Random Forest, otimizado via GridSearchCV.

## Estrutura do Projeto

- **`data/`**: Diretório para armazenar os datasets utilizados no projeto.
- **`notebooks/`**: Jupyter Notebooks contendo o desenvolvimento e experimentos do projeto.
- **`scripts/`**: Scripts Python utilizados para execução do pipeline de dados e treinamento do modelo.
- **`models/`**: Diretório para salvar os modelos treinados.
- **`README.md`**: Documentação do projeto.

## Pipeline do Projeto

1. **Carregamento de Dados**: Leitura do dataset original e tratamento de eventuais inconsistências.
2. **Pré-processamento de Dados**: Limpeza dos textos, remoção de stopwords, tokenização e lematização para preparar os dados para o modelo.
3. **Criação de Features**: Transformação do texto em features numéricas usando TF-IDF (Term Frequency-Inverse Document Frequency).
4. **Divisão dos Dados**: Separação dos dados em conjuntos de treino e teste.
5. **Balanceamento das Classes**: Aplicação da técnica de SMOTE (Synthetic Minority Over-sampling Technique) para lidar com o desbalanceamento de classes.
6. **Treinamento do Modelo**: Treinamento de um modelo de Random Forest com otimização de hiperparâmetros usando GridSearchCV.
7. **Avaliação do Modelo**: Avaliação do desempenho do modelo utilizando métricas como acurácia, F1-score, matriz de confusão, e curva ROC.
8. **Análise de Resultados**: Interpretação das features mais importantes e revisão da performance do modelo em termos de discriminabilidade (AUC).

## Pré-requisitos

Certifique-se de que você tenha os seguintes pacotes instalados:

- Python 3.8 ou superior
- Pandas
- Numpy
- Scikit-learn
- Imbalanced-learn
- Matplotlib
- Seaborn
- NLTK

Você pode instalar todas as dependências necessárias executando:

```bash
pip install -r requirements.txt
