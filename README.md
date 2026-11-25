Tarefa 01 -  📊 Módulo 06 - Visualização de Dados com Matplotlib e Seaborn (DataSUS)

Repositório dedicado aos estudos e exercícios práticos do **Módulo 06** do curso **Profissão: Cientista de Dados (EBAC)**, focado na construção de gráficos de frequência, análises comparativas e painéis visuais (*subplots*) utilizando **Matplotlib** e **Seaborn** sobre a base de nascidos vivos do **DataSUS** (`SINASC_RO_2019.csv`).

## 💡 Como elaborei este projeto

Desenvolvi a análise visual em Jupyter Notebook, estruturando o código desde o tratamento textual dos rótulos até a composição de múltiplos painéis exploratórios:

1. **Carregamento e Inspeção da Base:** Importei o dataset `SINASC_RO_2019.csv` com **Pandas** (`pd.read_csv`) e mapeei suas 69 variáveis clínicas e demográficas para orientar as visualizações.
2. **Limpeza de Rótulos para Visualização:** Realizei um pré-tratamento textual na coluna `GESTACAO` (`.str.replace('semanas', '')`) para remover textos redundantes e evitar sobreposição nos eixos dos gráficos.
3. **Análise Univariada em Grade (`plt.subplots`):** Estruturei uma grade de **3x2** com `sns.countplot()` para visualizar simultaneamente a distribuição de `APGAR1`, `APGAR5`, `SEXO`, `GESTACAO` e `ESTCIVMAE`, utilizando `fig.delaxes()` para remover o espaço vazio e manter o layout limpo.
4. **Análise Bivariada de Desfecho Clínico:** Construí um gráfico de barras comparativo com `sns.barplot()` cruzando o número de consultas pré-natal (`CONSULTAS`) com a média da nota de vitalidade no 5º minuto (`APGAR5`).
5. **Painel Consolidado (Dashboard Exploratório):** Montei um painel **2x2** reunindo as frequências das principais variáveis demográficas e de acompanhamento gestacional (`SEXO`, `GESTACAO`, `CONSULTAS` e `ESTCIVMAE`) para facilitar a leitura comparativa em uma única visualização.

## 🛠️ Tecnologias Utilizadas
* **Python 3**
* **Pandas** (carregamento e tratamento de strings nos rótulos)
* **Matplotlib** (controle de figuras, grades e eixos via `plt.subplots`)
* **Seaborn** (visualização estatística com `countplot` e `barplot`)
* **Jupyter Notebook / Google Colab**


TAREFA 02 - # 📊 Módulo 06 - Visualização de Dados com Matplotlib e Seaborn (DataSUS)

Repositório dedicado aos estudos e exercícios práticos do **Módulo 06** do curso **Profissão: Cientista de Dados (EBAC)**, focado na exploração visual de variáveis categóricas e contínuas sobre a base de nascidos vivos do **DataSUS** (`SINASC_RO_2019.csv`) utilizando **Matplotlib** e **Seaborn**.

## 💡 Como elaborei este projeto

Estruturei o trabalho em dois notebooks, avançando da visualização de frequências categóricas até a análise de distribuição e dispersão de variáveis numéricas:

### 1. Variáveis Categóricas e Painéis Exploratórios (`Tarefa 01`)
* **Tratamento de Rótulos:** Limpei textos redundantes na coluna `GESTACAO` (`.str.replace('semanas', '')`) para evitar sobreposição visual nos eixos.
* **Gráficos em Grade (`plt.subplots`):** Construí uma grade **3x2** com `sns.countplot()` para avaliar a distribuição de `APGAR1`, `APGAR5`, `SEXO`, `GESTACAO` e `ESTCIVMAE`, removendo o eixo excedente com `fig.delaxes()` para manter o layout limpo.
* **Análise Bivariada:** Utilize `sns.barplot()` para comparar a média da nota de vitalidade (`APGAR5`) conforme o número de consultas pré-natal (`CONSULTAS`).
* **Painel Consolidado (2x2):** Reuni as frequências de `SEXO`, `GESTACAO`, `CONSULTAS` e `ESTCIVMAE` em um único dashboard comparativo.

### 2. Distribuição e Dispersão de Variáveis Contínuas (`Tarefa 02`)
* **Detecção de Outliers e Quartis (`sns.boxplot`):** Construí diagramas de caixa (*boxplots*) para avaliar a mediana, amplitude interquartil e valores extremos das variáveis contínuas **`IDADEMAE`** (idade da mãe) e **`PESO`** (peso do recém-nascido).
* **Histogramas e Densidade (`sns.histplot`):** Plotei histogramas com curva de densidade estimada (`kde=True`) e ajuste de transparência (`alpha=0.15`) para analisar o formato das distribuições de idade materna e peso ao nascer.

## 🛠️ Tecnologias Utilizadas
* **Python 3**
* **Pandas** (carregamento de dados e tratamento de strings nos rótulos)
* **Matplotlib** (controle de figuras, grades e eixos via `plt.subplots`)
* **Seaborn** (`countplot`, `barplot`, `boxplot` e `histplot` com curva KDE)
* **Jupyter Notebook / Google Colab**




TAREFA 03 - 
