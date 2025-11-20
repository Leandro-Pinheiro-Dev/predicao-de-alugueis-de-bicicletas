
 **Predição de Aluguel de Bicicletas**

## 📌 **Descrição do Projeto**

Este projeto tem como objetivo desenvolver um modelo de Machine Learning capaz de **prever a quantidade diária de aluguéis de bicicletas** com base em variáveis meteorológicas e informações de calendário.

O trabalho aplica boas práticas de análise de dados, modelagem, validação e documentação — conectando diretamente com princípios de **Quality Assurance (QA)**.

---

## 📁 **Estrutura do Projeto**

```
📂 Projeto-P2
 ├── Leandro_P2.ipynb        # Notebook com todo o processamento, análises e modelos
 ├── Relatorio P2.docx       # Relatório final estruturado
 ├── README.md               # Documento atual
```

---

## 🔍 **1. Exploração e Análise dos Dados**

A primeira etapa consiste em entender a base:

* Verificação dos tipos de dados
* Procura por valores ausentes
* Estatísticas descritivas
* Distribuições e padrões iniciais

**Principais variáveis presentes:**

* Data (dia, mês, ano)
* Estação
* Indicador de feriado e dia útil
* Temperatura e sensação térmica
* Umidade
* Velocidade do vento
* Situação do tempo
* *Rentals* (variável alvo)

---

## 📊 **2. Análises Visuais**

Foram gerados gráficos que permitem interpretar o comportamento dos dados:

* **Histograma de rentals** → mostra distribuição da demanda
* **Matriz de correlação** → identifica variáveis que influenciam positivamente ou negativamente os aluguéis

**Insights principais:**

* Temperatura e sensação térmica têm correlação positiva com *rentals*
* Umidade e clima chuvoso reduzem o número de aluguéis

---

## 🧹 **3. Preparação dos Dados**

Etapas realizadas:

* Separação em variáveis independentes (X) e alvo (y)
* Divisão entre treino (80%) e teste (20%)
* Padronização e organização da base para modelagem

Essa etapa garante qualidade, consistência e evita viés nas previsões.

---

## 🤖 **4. Modelagem**

Dois modelos foram testados:

### **1️⃣ Regressão Linear**

* Simples e interpretável
* Serve como baseline

### **2️⃣ Árvore de Decisão**

* Capaz de capturar relações não lineares
* Ajuste de profundidade para evitar overfitting

---

## 📈 **5. Avaliação dos Modelos**

As seguintes métricas foram utilizadas:

* **R²** – Variabilidade explicada
* **MAE** – Erro absoluto médio
* **RMSE** – Desvio médio das previsões

**Resultado:**
A **Árvore de Decisão** teve melhor desempenho em todas as métricas, sendo considerada o modelo ideal para esta base.

---

## 📌 **6. Conexão com Quality Assurance (QA)**

Este projeto aplica vários princípios importantes de QA:

* **Validação da qualidade dos dados**
* **Testes comparativos entre modelos**
* **Análise sistemática de métricas**
* **Documentação clara e rastreável (notebook + relatório)**
* **Reprodutibilidade do processo**

Embora seja um projeto de dados, segue práticas fundamentais de garantia de qualidade.

---

## 🏁 **7. Conclusões**

* A Árvore de Decisão apresentou o melhor desempenho na predição dos aluguéis.
* Temperatura tem forte influência positiva na demanda.
* Umidade e clima desfavorável reduzem o número de bicicletas alugadas.

**Próximos passos sugeridos:**

* Testar modelos ensemble (Random Forest, XGBoost)
* Otimizar hiperparâmetros
* Ampliar análise para sazonalidade anual

---

## 🚀 **Como Executar o Notebook**

1. Instale as dependências necessárias:

```bash
pip install pandas numpy matplotlib scikit-learn
```

2. Abra o notebook:

```bash
jupyter notebook Leandro_P2.ipynb
```
