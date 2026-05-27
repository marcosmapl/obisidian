---
disciplina: Tecnologia da Informação
tópico: Business Intelligence
created: 2026-02-12T09:30:00
updated: 2026-02-12T09:35:00
---

## Conceito

> [!note] Data Mart
> **Subconjunto temático e especializado** de um Data Warehouse, funcionando como um "mini armazém" de dados voltado para atender às necessidades específicas de um departamento ou área de negócio, como marketing, finanças ou recursos humanos.

---
## Características e Segmentação

Os Data Marts são estruturas menores e mais ágeis que o Data Warehouse corporativo (EDW). Eles podem ser segmentados por diferentes critérios:

• **Assuntos:** Como concursos, coaching ou pós-graduação.
• **Níveis de Agregação:** Dados sumarizados por períodos (semanal, mensal, anual).
• **Localização Geográfica:** Dados específicos de regiões (Norte, Sul, etc.).

---
## Tipos de Arquitetura de Data Mart

Existem três formas principais de implementar um Data Mart, dependendo da origem dos dados:

• **Dependente:** É criado a partir de um **Enterprise Data Warehouse (EDW)** centralizado. Os dados já chegam limpos e padronizados, garantindo consistência com a visão global da empresa.
• **Independente:** É construído diretamente dos sistemas operacionais (**OLTP**), sem passar por um armazém central. É mais rápido e barato de implementar, mas corre o risco de criar **"silos de informação"** (dados inconsistentes entre setores).
• **Híbrido:** Combina dados tanto do EDW quanto de fontes operacionais, oferecendo flexibilidade para uma evolução gradual.

---
## Abordagens de Construção (Kimball vs. Inmon)

O papel do Data Mart no ecossistema de dados varia conforme a estratégia adotada:

• **Abordagem de Bill Inmon (Top-Down):** Prioriza a construção de um armazém corporativo centralizado (EDW) primeiro, para só então derivar os Data Marts dependentes.
• **Abordagem de Ralph Kimball (Bottom-Up):** Defende que o processo deve começar pela implantação de Data Marts departamentais, que posteriormente são integrados por meio de **"dimensões conformadas"** (padronizadas) para compor a visão corporativa.

---
## Vantagens e Propósito

A principal finalidade do Data Mart é fornecer **acesso rápido e direto** a dados úteis para a tomada de decisão em níveis táticos e operacionais. Suas vantagens incluem o menor volume de dados (o que reduz o tempo de processamento), foco temático que facilita o uso por usuários não técnicos e maior agilidade na entrega de valor ao negócio.

---
## Tópicos Relacionados

- [[Modelagem Multidimensional]]
- [[Processo ETL]]
- [[Data Warehouse]]
- [[Data Lake]]
- [[Data Mesh]]
