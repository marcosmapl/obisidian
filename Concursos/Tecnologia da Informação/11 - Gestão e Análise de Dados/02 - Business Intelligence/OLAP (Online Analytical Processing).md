---
disciplina: Tecnologia da Informação
tópico: Business Intelligence
created: 2026-02-26T15:50:00
updated: 2026-02-26T15:55:00
---


## Conceito

Ambiente voltado à **análise de dados históricos para suporte à decisão estratégica**.

---
## Finalidade

Permitir **análises complexas e multidimensionais** para apoiar gestores.

Exemplos:
- Data Warehouse
- Business Intelligence (BI)
- Dashboards gerenciais

---
## Características Técnicas

- 📊 Processamento **analítico**
- 🎯 Foco **estratégico**
- 🧊 Estrutura **multidimensional** (modelos estrela ou snowflake)
- 📦 Orientado a **cubos de dados / estruturas multidimensionais**
- 🔎 Consultas **ad-hoc e complexas**
- 🧬 Dados **desnormalizados** (redundância controlada para ganho de desempenho)
- ⏳ Tempo de resposta **maior (segundos ou mais)** devido ao alto volume de processamento
- 📅 Atualizações por **cargas periódicas (ETL/ELT)**
- 📉 **Baixa granularidade** (dados agregados/sumarizados)
- 🗄 Dados **não voláteis** (históricos, estáveis)

## Objetivo Central

Suporte à tomada de decisão por meio de análise histórica e consolidada.

---
## Objetivo Central

Eficiência operacional e confiabilidade nas transações.

---
## Comparação

|Característica|OLTP|OLAP|
|---|---|---|
|Finalidade|Operacional|Estratégica|
|Tipo de processamento|Transacional|Analítico|
|Modelo de dados|Relacional normalizado|Multidimensional desnormalizado|
|Consultas|Simples e pré-definidas|Complexas e ad-hoc|
|Granularidade|Alta (detalhada)|Baixa (agregada)|
|Atualização|Contínua|Periódica|
|Volatilidade|Alta|Baixa|
|Tempo de resposta|Milissegundos|Segundos|

---
## Resumo para Memorização Rápida

- **OLTP = Operação + Transação + Tabelas + Tempo Real**
- **OLAP = Análise + Agregação + Histórico + Estratégia**

---
## Tópicos Relacionados

- [[OLTP (Online Transaction Processing)]]
