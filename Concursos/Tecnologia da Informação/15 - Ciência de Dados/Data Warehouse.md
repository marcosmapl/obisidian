---
disciplina: Tecnologia da Informação
tópico: Business Intelligence
created: 2026-02-12T09:20:00
updated: 2026-02-12T09:25:00
---

## Conceito

> [!note] Data Warehouse (DW)
> Atua como um repositório centralizado, que consolida dados de múltiplas fontes (sistemas internos, planilhas, APIs externas, etc) e os organiza de forma estruturada para facilitar consultas analíticas.

Ele não é usado para registrar transações operacionais, mas sim para suportar análises, gerar relatórios gerenciais e orientar decisões estratégicas. 

Esse ambiente permite responder perguntas mais amplas e detectar padrões que o banco transacional sozinho não conseguiria mostrar com eficiência.

---
## Características Essenciais (Os Pilares de Inmon)

Para ser considerado um Data Warehouse, o repositório deve atender a quatro propriedades fundamentais definidas por Bill Inmon:

- **Orientado por Assunto:** Diferente dos sistemas operacionais organizados por funções (como "cadastro" ou "estoque"), o DW organiza os dados por **temas estratégicos** (como "Vendas", "Clientes" ou "Finanças").
- **Integrado:** Ele unifica dados de múltiplas fontes heterogêneas (ERPs, CRMs, planilhas), padronizando nomenclaturas e unidades de medida para criar uma **"fonte única da verdade"**.
- **Variável no Tempo (Histórico):** Enquanto o banco operacional foca no estado atual, o DW mantém um **acervo de meses ou décadas**, permitindo identificar tendências e comparar desempenhos ao longo do tempo.
- **Não-Volátil:** Uma vez que o dado é carregado, ele não sofre alterações ou exclusões linha a linha; ele permanece estável para garantir que relatórios gerados em momentos diferentes sejam consistentes.

----
## Data Warehouse vs. Sistemas Transacionais (OLTP)

As fontes enfatizam que o DW não substitui o banco de dados operacional, mas o complementa. A principal diferença reside na finalidade:

• **OLTP (Processamento Transacional):** Voltado para as operações do dia a dia, com transações rápidas (inserções e atualizações) e dados detalhados.

• **OLAP (Processamento Analítico):** O ambiente onde o DW reside, focado em **consultas complexas**, grandes volumes de dados históricos e suporte à gestão.

---
## Tópicos Relacionados

- [[Modelagem Multidimensional]]
- [[Processo ETL]]
- [[Data Mart]]
- [[Data Lake]]
- [[Data Mesh]]
