# 📊 Challenge TelecomX - Parte 02

## 📌 Descrição
Este projeto tem como objetivo analisar dados de clientes de uma empresa de telecomunicações e construir modelos de Machine Learning para prever **churn** (cancelamento de clientes).  
O desafio consiste em comparar diferentes algoritmos, ajustar hiperparâmetros e avaliar o desempenho dos modelos, buscando identificar o que melhor equilibra **precisão** e **recall**.

---

## 🎯 Objetivos
- Realizar análise exploratória dos dados (EDA).  
- Pré-processar as variáveis (normalização, one-hot encoding etc.).  
- Treinar e avaliar diferentes modelos de classificação:  
  - Dummy Classifier  
  - Decision Tree Classifier  
  - KNN (inicial e ajustado)  
- Comparar métricas: **Acurácia, Precisão, Recall, F1-score e Matriz de Confusão**.  
- Identificar sinais de **overfitting** e **underfitting**.  
- Sugerir próximos passos para melhoria do modelo.  

---

## ⚙️ Instalação e Dependências
Antes de executar o projeto, certifique-se de ter o Python 3.x instalado e crie um ambiente virtual.  
As principais bibliotecas utilizadas foram:


```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter


## Como Executar o Projeto

>1.Clone este repositório ou baixe os arquivos.

>2.Instale as dependências listadas acima.

>3.Abra o Notebook no Google Colab:
jupyter notebook Challenge_TelecomX_Parte02.ipynb

>4.Execute as células em ordem para reproduzir as análises e resultados.


Principais Resultados

--Dummy Classifier: Acurácia de ~0.73, não conseguiu identificar clientes churn.

--Decision Tree (max_depth=3): Melhor precisão (0.69) e boa generalização, sem sinais de overfitting.

--KNN Inicial: Recall maior que a árvore, mas apresentou overfitting.

--KNN Ajustado (n=11, distância Manhattan): Melhor F1-score (0.56) e maior recall, equilibrando precisão e recall.


Conclusão:

O Decision Tree é mais indicado se a prioridade for precisão.

O KNN Ajustado é mais indicado se a prioridade for recall (captar mais clientes em risco de churn).


Próximos Passos

>>Explorar Feature Engineering para criar novas variáveis relevantes.

>>Tratar o desbalanceamento de classes (oversampling/undersampling).

>>Testar outros algoritmos: Logistic Regression, Random Forest, Gradient Boosting.

>>Aplicar validação cruzada para obter métricas mais robustas.

>>Analisar casos de erros do modelo (falsos positivos/negativos).


Autor
jaqueline-quaresma


