---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2025-12-13T08:42:00
updated: 2025-12-26T00:10:00
---
## 🔸Definição

> [!note] Arquitetura ANSI/SPARC
> É um modelo de três níveis (**externo**, **conceitual** e **interno**) para Sistemas de Gerenciamento de Banco de Dados (SGBDs) que promove a independência dos dados, separando a visão do usuário (externo), a estrutura lógica do banco (conceitual) e o armazenamento físico (interno), permitindo flexibilidade e manutenção.

![[Pasted image 20251226001200.png]]

---
## 🔸Nível Externo (visão/usuário)

- **O que é**: A **visão** mais abstrata, como os **usuários individuais** veem o banco de dados, focando apenas nos dados relevantes para eles, escondendo detalhes.
- **Para quem**: Usuários finais, aplicações.
- **Atividades**: Definição de visões.

#ti/bd/ansi_sparc/nível/externo

---
## 🔸Nível Conceitual (lógico/comunidade)

- **O que é**: Descreve a **estrutura lógica** completa do banco de dados (tabelas, relacionamentos, restrições), sem se preocupar com o armazenamento físico.
- **Para quem**: **Administradores de Banco de Dados** (DBAs) e desenvolvedores.
- **Atividades**: Definição de **tabelas**, **PKs**, **FKs**, etc.

#ti/bd/ansi-sparc/nível/conceitual

---
## 🔸Nível Interno (físico)

- **O que é**: Descreve como os dados são realmente **armazenados e organizados fisicamente** no disco (arquivos, índices, caminhos de acesso).
- **Para quem**: O próprio SGBD. 
- **Atividades**: Especificação de algoritmos e estruturas de dados para armazenamento.

> [!warning] CESPE: não considera que o nível físico seja responsável por **gerenciar o armazenamento dos registros** no dispositivo físico (HD/SSD).

#ti/bd/ansi-sparc/nível/interno

#ti/bd/ansi-sparc 

---
## 🔸Links Relacionados

- [[Independência Lógica de Dados]]
- [[Independência Física de Dados]]
