---
disciplina: Tecnologia da Informação
tópico: Banco de Dados
created: 2025-12-13T08:42:00
node_size: "10"
---
# Definição

Um modelo de três níveis (externo, conceitual e interno) para Sistemas de Gerenciamento de Banco de Dados (SGBDs) que promove a independência dos dados, separando a visão do usuário (externo), a estrutura lógica do banco (conceitual) e o armazenamento físico (interno), permitindo flexibilidade e manutenção.

## Nível Externo (visão/usuário)
- **O que é**: A visão mais abstrata, como os **usuários individuais** veem o banco de dados, focando apenas nos dados relevantes para eles, escondendo detalhes.
- **Para quem**: Usuários finais, aplicações.

#ti/bd/ansi-sparc/nível/externo

## Nível Conceitual (lógico)
- **O que é**: Descreve a estrutura lógica completa do banco de dados (tabelas, relacionamentos, restrições), sem se preocupar com o armazenamento físico.
- **Para quem**: **Administradores de Banco de Dados** (DBAs) e desenvolvedores.

#ti/bd/ansi-sparc/nível/conceitual

## Nível Interno (físico)
- **O que é**: Descreve como os dados são realmente armazenados fisicamente no disco (arquivos, índices, caminhos de acesso).
- **Para quem**: O próprio SGBD. 

#ti/bd/ansi-sparc/nível/interno
#ti/bd/ansi-sparc 
