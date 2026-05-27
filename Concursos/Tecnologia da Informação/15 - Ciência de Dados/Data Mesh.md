---
disciplina: Tecnologia da Informação
tópico: Business Intelligence
created: 2026-02-12T14:00:00
updated: 2026-02-12T14:05:00
---

## Conceito

> [!note] Data Mesh
> Etapa mais recente na evolução da arquitetura de dados, surgindo por volta de 2019 como uma alternativa aos modelos centralizadores (como o Data Warehouse e o Data Lake). No contexto mais amplo do armazenamento de dados, sua principal inovação é a **descentralização da responsabilidade**, tratando os dados não como subprodutos de sistemas, mas como **produtos de valor** gerenciados por quem melhor os conhece: os domínios de negócio

---
## A Filosofia da Descentralização (Domínios)

Diferente das arquiteturas tradicionais onde uma equipe central de TI ou engenharia de dados cuida de todo o repositório, o Data Mesh propõe que **cada área da empresa (Marketing, Finanças, Logística, etc.) seja responsável pelos seus próprios dados**.

- Essa abordagem valoriza o conhecimento de quem está na ponta da operação.
- O modelo resolve o problema do "gargalo" técnico, onde uma única equipe central fica sobrecarregada com demandas de toda a organização

---
## Os Quatro Princípios Fundamentais

As fontes destacam quatro pilares que sustentam o Data Mesh para garantir que a descentralização não gere caos:

• **Domínio Orientado:** A responsabilidade pelo tratamento e qualidade das informações fica com os times que as geram.
• **Dados como Produto (Data Product):** Os dados devem ser entregues com qualidade garantida, documentação clara e facilidade de acesso, sendo úteis e confiáveis para o consumo de outras áreas.
• **Plataforma de Autoatendimento (Self-service):** As equipes de domínio devem ter ferramentas que lhes deem autonomia para trabalhar com os dados sem depender constantemente de especialistas centrais.
• **Governança Federada:** Mesmo com a autonomia, existem padrões, regras de segurança e boas práticas compartilhadas entre todos os times para garantir a interoperabilidade (que os dados de diferentes domínios "falem a mesma língua")

---
## Tópicos Relacionados

- [[Modelagem Multidimensional]]
- [[Processo ETL]]
- [[Data Warehouse]]
- [[Data Lake]]
- [[Data Mart]]
