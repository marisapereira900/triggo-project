
# Projeto Técnico - Olist (Programa Trainee Triggo.ai)

Este projeto foi desenvolvido como parte do processo seletivo para o Programa de Excelência em Engenharia de Dados e DataOps da **Triggo.ai**. O objetivo foi analisar um conjunto de dados públicos de comércio eletrônico brasileiro da Olist, consistindo no tratamento dos dados, geração de insights e construção de visualizações úteis para tomada de decisão.

---

## Estrutura do Projeto

```bash
triggo-olist-project/
│
├── data/                     # Dados originais (crus)
├── data_limpa/               # Dados tratados/limpos
├── brazil_states.geojson     # Arquivo externo com o mapa do Brasil
├── notebook_parte1           # Notebook com as análises (Parte 1)
├── notebook_parte2           # Notebook com as análises (Parte 2)    
├── notebook_parte3           # Notebook com as análises (Parte 3)  
├── notebook_parte4           # Notebook com as análises (Parte 4) 
├── README.md                 # Este arquivo
```

## Como Executar o Projeto

### 1. Clone o Repositório

```bash
git clone https://github.com/marisapereira900/triggo-olist-project.git
cd triggo-olist-project
```

### 2. Crie um Ambiente Virtual

```bash
python -m venv venv
source venv/bin/activate  # No Windows: venv\Scripts\activate
```

### 3. Instale as Dependências

```bash
pip install -r requirements.txt
```

> Caso não tenha um arquivo `requirements.txt`, instale manualmente:

```bash
pip install pandas plotly dash scikit-learn
```

### 4. Execute os Notebooks

Abra os arquivos `notebooks/` com Jupyter, Google Colab ou VSCode para visualizar as análises.

### 5. Visualize o Mapa Interativo

Execute o script com Plotly (ex: `mapa_vendas.py`) que carrega o arquivo GeoJSON e os dados de vendas por estado.

---

## Principais Resultados

### **Parte 1 – Preparação dos Dados**
- Remoção de valores duplicados e nulos.
- Realizado merge de tabelas e limpeza de colunas inconsistentes.
- Arquivos tratados salvos em `data_limpa/`.

### **Parte 2 – Análises Exploratórias**
- **Estados com maior volume de vendas:** SP, RJ, MG.
- **Categorias mais vendidas:** cama_mesa_banho, beleza_saude.
- **Piores avaliações** associadas a **atrasos na entrega**.

### **Parte 3 – Machine Learning**
- **Regressão Logística** para prever atrasos:
  - Acurácia: **~88%**
- **Segmentação de Clientes** com KMeans:
  - Agrupamento em 3 perfis baseados em ticket médio e frequência.

### **Parte 4 – Visualizações Interativas**
- Visualizações com Plotly:
  - Dashboard com filtro de melhores vendedores.
  - Mapa de calor por estado (GeoJSON).
  - Gráficos de avaliação, categorias e logística.

---

##  Contato

- **Marisa Pereira de Souza**  
- 🌎 Florianópolis/SC  
- 📧 mariszprr@gmail.com  
- 🔗 [LinkedIn](https://www.linkedin.com/in/marisapereiradesouza)

---
