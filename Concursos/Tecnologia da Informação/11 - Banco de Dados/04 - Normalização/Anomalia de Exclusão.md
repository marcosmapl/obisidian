---
disciplina: Tecnologia da Informação
tópico: Normalização
created: 2026-01-12T23:20:00
updated: 2026-01-12T23:20:00
---

## Conceito

> [!note] Anomalia de Exclusão
> Ocorre quando, ao **remover um registro**, ocorre também a **perda involuntária de outras informações relevantes**, que **não deveriam ser excluídas**.

> [!tip] Ela decorre do fato de **dados independentes estarem armazenados na mesma tabela**.

#tecnologia_informacao/banco_dados/anomalia_exclusao

---
## Causa Principal

- **Mistura de múltiplas entidades** em uma única tabela
- **Redundância de dados**
- **Dependências funcionais inadequadas**
- Falta de aplicação das **formas normais**

---
## Consequência

- **Perda de dados históricos ou estruturais**
- Comprometimento da **integridade informacional**
- Necessidade de **recadastramento** de dados
- Risco de decisões baseadas em informações incompletas

---
## Frase-chave

> [!tip] A anomalia de exclusão ocorre quando a remoção de um registro provoca a perda não intencional de outras informações relevantes.

---
## Tópicos Relacionados

- [[Anomalia de Inserção]]
- [[Anomalia de Atualização]]

