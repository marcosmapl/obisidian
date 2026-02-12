---
disciplina: Tecnologia da Informação
tópico: Business Intelligence
created: 2026-02-12T09:30:00
updated: 2026-02-12T09:35:00
---

## Conceito

> [!note] Processo ETL
> Descrito nas fontes como o conjunto de etapas fundamentais para transformar dados brutos em informações valiosas que suportam a gestão corporativa e a tomada de decisão. No ecossistema de **Business Intelligence (BI)** e **Data Warehouse (DW)**, ele funciona como a "espinha dorsal" que integra sistemas heterogêneos, garantindo que os dados sejam padronizados e higienizados antes de serem disponibilizados para análise.

---
## Etapas do ETL

- **Extração (Extract):** É a fase de coleta de dados de diversas fontes, como sistemas **ERP**, **CRM**, bancos de dados legados, planilhas e APIs externas. Estima-se que cerca de **60% do esforço de um projeto de ETL** esteja concentrado apenas na extração, devido à diversidade de formatos e origens.
- **Transformação (Transform):** Considerada a etapa mais crítica e complexa, é onde os dados são "limpos", padronizados e enriquecidos. Exemplos de atividades nesta fase incluem a **deduplicação** (remoção de duplicatas), correção de erros, cálculos, conformidade de chaves e a padronização de campos (como converter "São Paulo" e "SP" para um formato único).
- **Carga (Load):** É a inserção final dos dados já tratados no repositório de destino, como um **Data Warehouse** ou **Data Mart**. A carga pode ser **inicial** (todo o histórico) ou **incremental** (apenas o que mudou desde a última atualização).

---
## Ambientes Intermediários

### Staging Area (Área de Preparação)

- Um **ambiente técnico temporário** usado para **armazenar dados brutos** enquanto eles são **processados e limpos**. 
- É um **espaço de trabalho** que não é acessado pelos usuários finais.
### Operational Data Store (ODS)

- Um repositório integrado que fornece uma **visão operacional em tempo quase real**
- Útil para **decisões táticas de curto prazo** antes de os dados serem consolidados **historicamente** no DW.