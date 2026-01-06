---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2025-12-13T08:42:00
updated: 2025-12-26T00:10:00
---
## Definição

> [!note] Arquitetura ANSI/SPARC
> É um modelo de três níveis (**externo**, **conceitual** e **interno**) para Sistemas de Gerenciamento de Banco de Dados (SGBDs) que promove a independência dos dados, separando a visão do usuário (externo), a estrutura lógica do banco (conceitual) e o armazenamento físico (interno), permitindo flexibilidade e manutenção.

![[Pasted image 20251226001200.png]]

---
## Nível Externo

- **O que é**: A **visão** mais abstrata, como os **usuários individuais** veem o banco de dados, focando apenas nos dados relevantes para eles, escondendo detalhes.
- **Maior nível de abstração**
- **Para quem**: Usuários finais, aplicações.
- **Atividades**: Definição de visões.

> [!tip] Também chamado de **Nível Lógico de Visão de Usuário** (C. J. Date)

#ti/bd/ansi_sparc/nível/externo

---
## Nível Conceitual

- **O que é**: Descreve a **estrutura lógica** completa do banco de dados (tabelas, relacionamentos, restrições, operações e restrições), sem se preocupar com o armazenamento físico.
- **Para quem**: **Administradores de Banco de Dados** (DBAs) e desenvolvedores.
- **Atividades**: Definição de **tabelas**, **PKs**, **FKs**, etc.

> [!tip] Também chamado de **Nível Lógico de Comunidade** (C. J. Date)

#ti/bd/ansi-sparc/nível/conceitual

---
## Nível Interno

- **O que é**: Descreve como os dados são realmente **armazenados e organizados fisicamente** no disco (arquivos, índices, caminhos de acesso).
- Nível mais **próximo do nível físico**
- **Menor nível de abstração**
- **Para quem**: O próprio SGBD. 
- **Atividades**: Especificação de algoritmos e estruturas de dados para armazenamento.

> [!tip] Também chamado de **Nível Físico ou Armazenamento** (C. J. Date) 

> [!warning] NÃO lida com o **armazenamento dos registros nos dispositivos físicos (HD/SSD)**.

#ti/bd/ansi-sparc/nível/interno

#ti/bd/ansi-sparc 

---
## Tópicos Relacionados

- [[Independência Lógica de Dados]]
- [[Independência Física de Dados]]
