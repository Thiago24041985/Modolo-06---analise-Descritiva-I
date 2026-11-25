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
