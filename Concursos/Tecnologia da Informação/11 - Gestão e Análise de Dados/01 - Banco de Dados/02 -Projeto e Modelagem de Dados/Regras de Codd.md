---
created: 2026-01-14T15:20:00
updated: 2026-01-10T15:25:00
disciplina: Tecnologia da Informação
tópico: Banco de Dados
---
## Conceito

> [!note] Regras de Codd
> Foram criadas para definir o que é necessário para que um SGBD seja considerado **relacional**

#tecnologia_informacao/banco_dados/regras_codd

---
## Regras

### Regra 0

- Um SGBD  relacional  deve  gerenciar  seus  dados usando apenas suas capacidades relacionais.

### Regra 1

> [!note] Informação
> Todas as informações em um banco de dados relacional são representadas explicitamente no nível lógico e de forma exatamente por valores em tabelas, ou seja, seus valores de coluna em linhas dentro das tabelas.

### Regra 2

> [!note]  Garantia de Acesso
> Todos os valores atômicos(dados) de um banco de dados relacional devem ter a garantia de acesso, sendo tal acesso por combinação do nome da tabela, sua chave primária e o nome da coluna. A combinação destes dados forma um identificador único, mitigando problemas posteriores de interpretação da informação.

### Regra 3

> [!note] Tratamento sistemático de nulos
> Independente do tipo de dado que deva ser armazenado num campo, o valor nulo (**null**) é aquele que é diferente de uma cadeia de espaços vazios ou zeros, porém é suportado por qualquer SGBD;

### Regra 4

> [!note] Catálogo dinâmico baseado no modelo relacional
> A descrição lógica do banco de dados(metadados) deve ser apresentada na mesma forma dos dados comuns, sendo possível, para acessar tais dados, usar a mesma linguagem regular que é usada no banco de dados

### Regra 5

> [!note] Sublinguagem ampla de dados
> O banco de dados deve dar suporte à configuração do nível de inserções, atualizações e exclusões. No entanto, deve haver pelo menos uma língua cujas declarações são expressivas, por meio de uma sintaxe bem definida, como cadeias de caracteres, e que possibilite: definir dados, visualizar definições, manipular dados de forma interativa ou por programa, aplicar restrições de integridade, aplicar autorizações e estabelecer limites nas transações

### Regra 6

> [!note] Atualização de visualização
> Qualquer visualização que possa ser atualizada teoricamente, o sistema deve permitir fazer, ou seja, o SGBD deve permitir a construção de diferentes visões de dados. Vale salientar que nem sempre as atualizações feitas em visões terão reflexo nas suas tabelas associadas

### Regra 7

> [!note] Inserção, atualização e exclusão de alto nível
> O SGBD deve permitir que as operações de inserção, atualização e exclusão possam ser definida em diferentes níveis, fazendo uso da linguagem definida para manipulação de dados.

### Regra 8

> [!note] Independência Física de Dados
> Os aplicativos de uso em terminal não devem ser afetados quando houver mudanças nas estruturas ou no armazenamento dos dados

### Regra 9

> [!note] Independência Lógica de Dados
> Os aplicativos de uso em terminal não devem ser afetados quando houver alterações na estrutura lógica das tabelas, ou nas visões criadas

### Regra 10

> [!note] Independência de Integridade
> Possibilidade de criação de todas as definições de integridade relacional através da linguagem relacional e que elas sejam armazenadas no catálogo de sistema e **não no nível de aplicação**. As aplicações não devem ser afetadas por mudanças ocorridas nas restrições de integridade

### Regra 11

> [!note] Independência de Distribuição
> Os usuários finais e aplicativos não devem ser afetados e nem devem conhecer sobre a localização dos dados

### Regra 12

> [!note] Não transposição das Regras
> Como o sistema deve permitir acesso em baixo nível aos dados, as regras de integridade do banco de dados devem ser preservadas, de tal forma, que qualquer tentativa de acesso por usuário ou aplicação, sem respeitar as regras, seja impedida pelo SGBD










