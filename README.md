# 🛍️ Segmentação de Clientes com Clusterização K-Means

Projeto de machine learning não supervisionado para identificar perfis distintos de clientes e viabilizar estratégias de marketing personalizadas com base em dados comportamentais e financeiros.

---

## 🎯 Objetivo de Negócio

Equipes de varejo e e-commerce frequentemente tratam toda a base de clientes como um único público, resultando em baixo ROI nas campanhas de marketing. Este projeto resolve esse problema agrupando os clientes em segmentos homogêneos, permitindo que o negócio adapte a comunicação, as ofertas e as estratégias de retenção a cada perfil.

---

## 🗂️ Metodologia

### 1. Análise Exploratória de Dados (EDA)
- Análise da distribuição de renda e spending score na base de clientes
- Identificação de correlações entre variáveis demográficas e comportamento de compra

### 2. Pré-processamento de Dados
- Normalização das features com `StandardScaler` para evitar viés de escala no algoritmo baseado em distância
- Seleção das variáveis mais discriminantes para a clusterização: **Renda Anual** e **Spending Score**

### 3. Número Ótimo de Clusters
Duas técnicas complementares foram aplicadas para definir o número ideal de grupos:

- **Método do Cotovelo (Elbow Method)**: Identificou o ponto de retornos decrescentes na redução da inércia
- **Silhouette Score**: Validou a coesão dos clusters; o modelo final com **5 clusters** atingiu um score de **0.272**

### 4. Modelo K-Means
- Treinamento de um modelo K-Means com `k=5`
- Mapeamento dos centros dos clusters para personas de negócio, permitindo interpretação estratégica

---

## 📊 Resultados — As 5 Personas de Clientes

| Cluster | Perfil | Estratégia |
|---|---|---|
| 0 — Estáveis | Clientes mais velhos, renda estável, gasto moderado | Programas de fidelidade |
| 1 — Poupadores | Renda alta, baixa frequência de gasto | Campanhas de exclusividade e premium |
| 2 — Engajados | Jovens, renda média, alto volume de compra | Eventos e experiências |
| 3 — Premium | Renda alta e gasto recorrente elevado | Serviços VIP e networking |
| 4 — Antenados | Jovens, renda mais baixa, orientados a compras | Descontos e conteúdo de tendências |

---

## 🛠️ Stack Técnica

| Categoria | Ferramentas |
|---|---|
| Linguagem | Python |
| Manipulação de Dados | Pandas, NumPy |
| Visualização | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn (K-Means, StandardScaler, Silhouette Score) |
| Ambiente | Jupyter Notebook |

---

## ▶️ Como Executar

```bash
# Clone o repositório
git clone https://github.com/oporaxuao/customer-segmentation-kmeans.git
cd customer-segmentation-kmeans

# Instale as dependências
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

# Inicie o notebook
jupyter notebook
```

---

## 👤 Autor

**João Alfredo de Sousa Siqueira**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-oporaxuao-blue)](https://linkedin.com/in/oporaxuao)
[![GitHub](https://img.shields.io/badge/GitHub-oporaxuao-black)](https://github.com/oporaxuao)
