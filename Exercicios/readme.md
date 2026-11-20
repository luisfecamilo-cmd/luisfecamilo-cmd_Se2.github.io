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
* **Excel** (`.xlsx`)# 📊 Análise e Visualização de Dados — Campe Supply

Este repositório reúne o processo de limpeza, tratamento, análise exploratória e visualização de dados desenvolvido durante as **5 aulas de capacitação** da Empresa Júnior (EJ). O fluxo parte da base bruta (`Campe_Supply_Corrompido.xlsx`, aba `Campe Supply`), passa pela base tratada (`Campe_Supply_Limpo.xlsx`)[cite: 1, 2] e chega à construção de indicadores, rankings, tabelas dinâmicas e gráficos para apresentação ao cliente.

---

## 🗺️ Jornada das Aulas

### 🔹 Aula 01 — Inspeção Inicial e Padronização Estrutural
- Inspeção inicial da base de dados, identificação do número de linhas e diagnóstico dos tipos de dados das colunas.
- Remoção de colunas desnecessárias e de registros duplicados logo no início do tratamento.
- Padronização dos nomes das colunas com conversão para minúsculas, remoção de espaços extras, troca de espaços por `_` e substituição de caracteres acentuados (como `ã` por `a`).

### 🔹 Aula 02 — Tratamento Textual e Recuperação de Nulos por Regra de Negócio
- Identificação de erros de digitação e variações textuais em colunas categóricas (como `setor`, `produto`, `vendedor`, `regiao`, `estado` e `cliente`).
- Padronização automatizada com função de similaridade textual (`get_close_matches`) aplicando corte de **0.6 (60%)** em relação às categorias oficiais.
- Recuperação de valores nulos por meio de regras de negócio e cruzamento de atributos, preenchendo `setor` a partir de `produto` e `regiao` a partir de `estado`.

### 🔹 Aula 03 — Tipagem, Consistência Matemática e Segunda Limpeza de Duplicatas
- Conversão das colunas financeiras (`faturamento`, `margem_de_lucro`, `lucro`) para formato numérico e preparação dos demais campos.
- Correção de inconsistências matemáticas discrepantes (como registros com lucro superior ao faturamento ou margem zerada com lucro positivo).
- Recuperação de valores nulos numéricos usando a relação entre faturamento, margem de lucro e lucro, seguida de uma segunda remoção de duplicatas após a padronização e extração da coluna `mes` a partir de `data_da_venda`.

### 🔹 Aula 04 — Indicadores, Rankings e Tabelas Dinâmicas
- Consolidação dos dados limpos para o cálculo dos indicadores da empresa (como faturamento e lucro).
- Estruturação de rankings para avaliar a performance por **vendedor**, **setor** e **produto**.
- Montagem de **tabelas dinâmicas** para cruzar dimensões e facilitar a leitura comparativa dos resultados antes da etapa gráfica.


### 🔹 Aula 05 — Visualização de Dados e Apresentação ao Cliente
- Criação de visualizações com `matplotlib` e `seaborn` para transformar os resultados da análise em gráficos de leitura rápida.
- Plotagem de gráfico de linha da **evolução mensal do faturamento** (de `Jan` a `Dez`) e demais gráficos de apoio para sustentar a apresentação ao cliente[cite: 3].


---

## 🛠️ Tecnologias Utilizadas
- **Linguagem:** Python
- **Manipulação e Limpeza:** `pandas`, `numpy`, `difflib`
- **Visualização de Dados:** `matplotlib`, `seaborn`
- **Planilhas:** Excel (`.xlsx`)[cite: 1, 2]