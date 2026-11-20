# 📊 Análise e Visualização de Dados — Campe Supply

Este repositório reúne a evolução do projeto desenvolvido durante as **5 aulas de capacitação** da Empresa Júnior (EJ), cobrindo desde a inspeção e limpeza de uma base de dados bruta (`Campe_Supply_Corrompido.xlsx`) até a geração de indicadores, tabelas dinâmicas e visualizações para apresentação ao cliente.

---

## 🗺️ Jornada das Aulas

### 🔹 Aula 01 — Inspeção Inicial e Padronização Estrutural
* Inspeção da base de dados e identificação do número de linhas.
* Diagnóstico dos tipos de dados das colunas.
* Remoção de colunas e registros duplicados.
* Padronização dos nomes das colunas (conversão para minúsculas, substituição de espaços por `_` e remoção de acentos).

### 🔹 Aula 02 — Tratamento Textual e Recuperação de Nulos por Regra de Negócio
* Identificação de inconsistências e erros de digitação nas variáveis categóricas.
* Criação de função de similaridade textual para padronizar termos com correspondência superior a **60%**.
* Recuperação de valores nulos por meio do cruzamento inteligente de dados (ex.: associando cada estado à sua respectiva região e cada produto ao seu setor).

### 🔹 Aula 03 — Tipagem, Consistência Matemática e Segunda Limpeza de Duplicatas
* Conversão das colunas para seus tipos adequados (numéricos e *strings*).
* Correção de inconsistências matemáticas discrepantes (ex.: cenários em que o lucro superava o faturamento).
* Preenchimento de valores nulos numéricos utilizando a relação matemática entre faturamento, margem de lucro e lucro.
* Execução de uma segunda etapa de remoção de duplicatas após a correção ortográfica e o preenchimento de nulos.

### 🔹 Aula 04 — Indicadores, Rankings e Tabelas Dinâmicas
* Cálculo dos principais indicadores financeiros e operacionais da empresa (como faturamento, lucro e margem).
* Construção de rankings de **melhores vendedores**, **setores de maior desempenho** e **produtos mais vendidos**.
* Elaboração de **tabelas dinâmicas** para o cruzamento multidimensional dos dados.

### 🔹 Aula 05 — Visualização de Dados e Apresentação ao Cliente
* Transformação dos rankings e análises em gráficos (como a evolução mensal do faturamento) para facilitar a leitura executiva e a apresentação dos resultados ao cliente.

---

## 🛠️ Tecnologias Utilizadas
* **Python** (`pandas`, `numpy`, `difflib`)
* **Visualização de Dados** (`matplotlib`, `seaborn`)
* **Excel** (`.xlsx`)