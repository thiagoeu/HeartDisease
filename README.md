# Heart Disease Prediction

Este repositório contém um projeto de machine learning para prever a ocorrência de doenças cardíacas com base em um conjunto de dados fornecido. O objetivo é criar um modelo preditivo que possa auxiliar na identificação precoce de problemas cardíacos.

## Conjunto de Dados

Os dados utilizados neste projeto foram obtidos a partir de uma planilha disponível no Google Sheets. O link para exportação dos dados em formato CSV é:

[Link para o conjunto de dados](#)

## Descrição das Variáveis

O conjunto de dados contém as seguintes variáveis:

- **Idade:** Idade do paciente.
- **Sexo:** Sexo do paciente (Masculino/Feminino).
- **Tipo de dor no peito:** Tipo de dor no peito relatada (1 a 4).
- **Pressão arterial em repouso:** Pressão arterial em repouso (em mm Hg).
- **Colesterol:** Nível de colesterol sérico (em mg/dl).
- **Açúcar no sangue em jejum:** Nível de açúcar no sangue em jejum (> 120 mg/dl = 1; < 120 mg/dl = 0).
- **Eletrocardiograma em repouso:** Resultados do eletrocardiograma em repouso (0 a 2).
- **Frequência cardíaca máxima:** Frequência cardíaca máxima alcançada.
- **Angina induzida por exercício:** Presença de angina induzida por exercício (1 = sim; 0 = não).
- **Depressão de ST:** Depressão de ST induzida por exercício em relação ao repouso.
- **Inclinação do segmento ST:** Inclinação do segmento ST no pico do exercício (1 a 3).
- **Número de vasos principais:** Número de vasos principais coloridos por fluoroscopia (0 a 3).
- **Talassemia:** Resultado da talassemia (3 = normal; 6 = defeito fixo; 7 = defeito reversível).
- **Doença cardíaca:** Presença de doença cardíaca (1 = sim; 0 = não).

## Metodologia

### Pré-processamento dos dados:

- Tratamento de valores ausentes.
- Normalização ou padronização das variáveis.
- Codificação de variáveis categóricas.

### Análise exploratória de dados (EDA):

- Visualização de distribuições e correlações.
- Identificação de outliers.

### Modelagem:

- Divisão dos dados em conjuntos de treino e teste.
- Aplicação de algoritmos de machine learning (ex: Regressão Logística, Random Forest, XGBoost).
- Avaliação dos modelos com métricas como acurácia, precisão, recall e F1-score.

### Seleção do modelo:

- Escolha do modelo com melhor desempenho.
- Ajuste de hiperparâmetros com validação cruzada.

### Deploy (opcional):

- Implementação do modelo em produção (ex: API com Flask ou FastAPI).

## Como Executar o Projeto

Clone este repositório:

```bash
git clone https://github.com/thiagoeu/HeartDisease.git
```

Instale as dependências necessárias:

```bash
pip install -r requirements.txt
```

Execute o notebook ou script principal:

```bash
jupyter notebook HeartDisease.ipynb
```

## Resultados dos Modelos

### 1. Regressão Logística

**Acurácia no Treino:** 87.77%

**Acurácia no Teste:** 82.98%

Matriz de Confusão:

```
[[15  5]
 [ 3 24]]
```

### 2. SVM (Support Vector Machine)

**Acurácia no Treino:** 92.02%

**Acurácia no Teste:** 85.11%

Matriz de Confusão:

```
[[15  5]
 [ 2 25]]
```

### 3. Random Forest

**Acurácia no Treino:** 100.00%

**Acurácia no Teste:** 82.98%

Matriz de Confusão:

```
[[15  5]
 [ 3 24]]
```

### 4. Árvore de Decisão

**Acurácia no Treino:** 100.00%

**Acurácia no Teste:** 82.98%

Matriz de Confusão:

```
[[15  5]
 [ 3 24]]
```

### 5. Rede Neural (MLP)

**Acurácia no Treino:** 100.00%

**Acurácia no Teste:** 89.36%

Matriz de Confusão:

```
[[16  4]
 [ 1 26]]
```

## Análise dos Resultados

O modelo de **Rede Neural (MLP)** obteve a maior acurácia no conjunto de teste (89.36%), seguido pelo **SVM (85.11%)**.

Os modelos **Regressão Logística, Random Forest e Árvore de Decisão** tiveram desempenho semelhante, com acurácia de teste em torno de **82.98%**.

A Rede Neural também apresentou o melhor equilíbrio entre **precisão** e **recall**, especialmente para a classe 1 (doença cardíaca presente).

## Contribuições

Contribuições são bem-vindas! Siga os passos abaixo:

1. Faça um fork do repositório.
2. Crie uma branch para sua feature:
   ```bash
   git checkout -b feature/nova-feature
   ```
3. Commit suas mudanças:
   ```bash
   git commit -m 'Adiciona nova feature'
   ```
4. Push para a branch:
   ```bash
   git push origin feature/nova-feature
   ```
5. Abra um Pull Request.

## Licença

Este projeto está licenciado sob a licença MIT. Consulte o arquivo LICENSE para mais detalhes.

