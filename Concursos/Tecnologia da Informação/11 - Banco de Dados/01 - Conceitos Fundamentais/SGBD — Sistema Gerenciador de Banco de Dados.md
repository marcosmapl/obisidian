---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2026-01-14T15:10:00
updated: 2026-01-14T15:15:00
---

## Conceito

> [!note] Sistema Gerenciador de Banco de Dados
> Conjunto de programação que funcionam integrados e permitem a construção, manipulação e manutenção de um Banco de Dados

---
## Propriedades

Um **Sistema Gerenciador de Banco de Dados (SGBD)**, ou DBMS (Database Management System), é um _conjunto de softwares_ que atua como uma interface entre os usuários/aplicações e o banco de dados físico. Ele permite criar, definir, manipular, controlar e gerenciar bancos de dados.

Principais **funções e objetivos** de um SGBD:

- **Definição de Dados:** Permitir a criação e modificação da estrutura do BD (esquema) através de uma Linguagem de Definição de Dados (DDL - Data Definition Language).
- **Manipulação de Dados:** Permitir a consulta, inserção, atualização e exclusão de dados através de uma Linguagem de Manipulação de Dados (DML - Data Manipulation Language, como SQL).
- **Controle de Acesso e Segurança:** Gerenciar permissões de usuários, impedindo acessos não autorizados.
- **Controle de Redundância e Consistência:** Minimizar a repetição desnecessária de dados e garantir que os dados sejam consistentes e íntegros.
- **Controle de Concorrência:** Gerenciar o acesso simultâneo de múltiplos usuários aos dados, evitando conflitos e inconsistências.
- **Backup e Recuperação:** Fornecer mecanismos para cópias de segurança e restauração do BD em caso de falhas.
- **Garantia de Integridade:** Impor regras que assegurem a validade e a precisão dos dados (ex: restrições de domínio, integridade referencial, etc.).
- **Independência de Dados:** Isolar as aplicações das alterações na estrutura física (independência física) ou lógica (independência lógica) do BD.
- **Interface com Aplicações:** Prover APIs e drivers para que programas possam interagir com o BD.
- **Catálogo de Dados (Dicionário de Dados):** Manter metadados sobre a estrutura do BD.

Componentes típicos de um SGBD incluem processador de consultas, gerenciador de transações, gerenciador de buffer, gerenciador de armazenamento, etc.

---
## Funcionalidades

- [[Tabelas]]
- [[Visões (Views)]]
- [[Gatilhos (Triggers)]]
- [[Índices (Indexes)]]
- [[Procedimentos Armazenados (Stored Procedures)]]
- [[Tarefas (Jobs)]]

---
## Tópicos Relacionados

- [[Banco de Dados — Conceito]]
