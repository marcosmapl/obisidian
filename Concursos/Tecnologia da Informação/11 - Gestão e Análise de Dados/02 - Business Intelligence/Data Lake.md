---
disciplina: Tecnologia da Informação
tópico: Business Intelligence
created: 2026-02-12T11:45:00
updated: 2026-02-12T11:50:00
---

## Conceito

> [!note] Data Lake
> Repositório centralizado capaz de armazenar grandes volumes de dados em seu **formato bruto (raw data)**, sejam eles estruturados, semiestruturados ou totalmente não estruturados.

---
## A Filosofia Schema-on-Read (Esquema na Leitura)

A principal distinção técnica entre um Data Lake e um Data Warehouse reside no momento em que a estrutura do dado é definida:

- **Data Lake (Schema-on-read):** Adota a filosofia de que o dado deve ser ingerido rapidamente sem transformação inicial. O formato e a organização só são aplicados quando alguém precisa ler ou analisar a informação, o que garante uma flexibilidade enorme para diferentes usos futuros.
- **Data Warehouse (Schema-on-write):** Exige que o esquema seja definido rigidamente antes do armazenamento, o que requer um processo de limpeza e organização prévia (ETL).

---
## Tópicos Relacionados

- [[Modelagem Multidimensional]]
- [[Processo ETL]]
- [[Data Warehouse]]
- [[Data Mart]]
- [[Data Mesh]]
