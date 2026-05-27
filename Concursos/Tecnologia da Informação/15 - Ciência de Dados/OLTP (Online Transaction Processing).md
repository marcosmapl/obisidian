---
disciplina: Tecnologia da Informação
tópico: Business Intelligence
created: 2026-02-26T15:26:00
updated: 2026-02-26T15:30:00
---

## Conceito

Ambiente voltado ao **processamento de transações operacionais em tempo real**, garantindo integridade, consistência e alta disponibilidade.

---
## Finalidade

Suportar as **operações do dia a dia da organização**.

Exemplos:

- Sistemas bancários
- Sistemas de vendas (PDV)
- ERPs
- Sistemas de cadastro

---
## Características Técnicas

- 🔁 Processamento de **transações ACID** (Atomicidade, Consistência, Isolamento e Durabilidade)
- 🎯 Foco **operacional**
- 🗂 Estrutura de dados **relacional bidimensional (tabelas)**
- 📌 Orientado a **registros (tuplas)**
- 📋 Consultas geralmente **pré-definidas e simples**
- 🧱 Dados **altamente normalizados** (redundância mínima)
- ⚡ Tempo de resposta **muito rápido (milissegundos)**
- 🔄 Atualizações **frequentes e contínuas**
- 🔍 **Alta granularidade** (dados detalhados)
- 🌊 Dados **voláteis** (sofrem alterações constantes)

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

- [[OLAP (Online Analytical Processing)]]
