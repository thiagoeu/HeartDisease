# Projeto de IA: Predição de Doenças Cardíacas

## 📊 Sobre o Projeto

Este projeto utiliza algoritmos de Inteligência Artificial para prever a presença de doenças cardíacas com base em um conjunto de dados contendo variáveis clínicas dos pacientes. A análise é realizada por meio de modelos de aprendizado de máquina que classificam se um indivíduo possui ou não uma condição cardíaca.

## 📁 Estrutura do Projeto
- **`projetoIA_v2.ipynb`**: Notebook principal contendo a análise exploratória de dados, preparação do conjunto de dados e o treinamento dos modelos de IA.
- **`data/`**: Diretório (se existente) onde estão armazenados os dados brutos e processados.
- **`images/`**: Contém gráficos gerados durante a análise exploratória.
- **`models/`**: Modelos treinados salvos, caso tenha sido configurado para exportar.

## 📚 Conjunto de Dados
O conjunto de dados utilizado é relacionado a doenças cardíacas, contendo as seguintes variáveis:

| Variável  | Descrição                                     |
|-----------|-----------------------------------------------|
| age       | Idade do paciente em anos                     |
| sex       | Gênero (0 = masculino, 1 = feminino)          |
| cp        | Tipo de dor no peito (0 a 3)                  |
| trestbps  | Pressão arterial de repouso (mmHg)            |
| chol      | Colesterol sérico (mg/dl)                     |
| fbs       | Açúcar no sangue em jejum (>120mg/dl, 1 = sim, 0 = não) |
| restecg   | Resultados do ECG em repouso (0 a 2)          |
| thalach   | Frequência cardíaca máxima atingida           |
| exang     | Angina induzida por exercício (1 = sim, 0 = não) |
| oldpeak   | Depressão ST induzida por exercício           |
| slope     | Inclinação do segmento ST (0 a 2)             |
| ca        | Número de vasos principais (0 a 4)            |
| thal      | Resultado do teste de estresse (0 a 3)        |
| target    | Doença cardíaca (1 = presença, 0 = ausência)  |

## 🚀 Como Rodar o Projeto

### 1. Clone o repositório
```bash
git clone https://github.com/thiagoeu/HeartDisease.git
cd HeartDisease
```

### 2. Crie um ambiente virtual
```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

### 3. Instale as dependências
```bash
pip install -r requirements.txt
```

### 4. Execute o Jupyter Notebook
```bash
jupyter notebook
```

Abra o arquivo `projetoIA_v2.ipynb` no navegador.

## 📈 Modelos Utilizados
Os seguintes algoritmos foram testados e avaliados:
- Regressão Logística
- K-Nearest Neighbors (KNN)
- Random Forest
- Support Vector Machine (SVM)

As métricas usadas para avaliação dos modelos incluem:
- **Acurácia**
- **Precisão**
- **Recall**
- **F1-Score**

## 📊 Resultados
Os resultados finais mostraram que o modelo *[inserir modelo com melhor desempenho]* obteve a melhor performance com uma acurácia de *[inserir valor]*.

## 📌 Próximos Passos
- Melhorar a otimização de hiperparâmetros.
- Implementar técnicas de balanceamento de dados.
- Explorar redes neurais para comparação.

## 🤝 Contribuição
Fique à vontade para abrir *issues* ou enviar *pull requests* para melhorias.

## 📄 Licença
Este projeto está sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

---

💡 *Desenvolvido por [Thiago](https://github.com/thiagoeu)*

