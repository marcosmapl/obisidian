---
disciplina: Tecnologia da Informação
tópico: Business Intelligence
created: 2026-02-12T09:25:00
updated: 2026-02-12T09:30:00
---

## Tabelas Fato

- Tabela que armazena informações **quantitativas** para análise de dados.
- Armazenam:
	- Ocorrências, Eventos ou Fatos de um processo de negócio da organização.
	- Medidas/métricas quantitativas (valores ou indicadores).
	- Podem ser medidas de desempenho, métricas operacionais, medidas agregadas, etc.|
- São efetivamente criadas apenas após a criação de tabelas dimensionais. 
- São tabelas que geralmente **crescem verticalmente**: mais registros ou linhas;
- Respondem à pergunta: _“O que está sendo medido nesse processo de negócio?”_
- Exemplo:
	- Quantidade
	- Valor
	- Lucro
	- Margem
	- Perda
	- Impostos

### Tipos de Fato

- **Fato Transacional**: Elas geralmente utilizam métricas aditivas, aquelas métricas que podem ser somadas por todas as dimensões.
- **Fato Agregada**: Esta tabela fato tem a função de acelerar o desempenho das consultas. Ela é criada com dados da tabela fato, alterando sua granularidade, ou seja, ela sumariza os dados, gerando uma tabela menor.
- **Fato Consolidada**: Essa tabela fato é bem parecida com a agregada, mas serve para combinar duas áreas de negócio.
- **Fato Snapshot Periódico**: Uma linha em uma tabela de fatos de snapshot periódico resume muitos eventos de medição que ocorrem durante um período padrão, como um dia, uma semana ou um mês. Em outras palavras, a granularidade é o período e, não, a transação individual.
- **Fato Snapshot Acumulado**: Uma linha em uma tabela de fatos de snapshot acumulado resume os eventos de medição que ocorrem em etapas previsíveis entre o início e o fim de um processo.
- **Fato Sem Fato**: Ela também é chamada de fato de associação ou de intersecção, mas o termo técnico é fato sem fato. Ela serve para fazer uma intersecção de dimensões.

### Tipos de Medida

- **Aditivas**: podem ser agregadas (Ex: Lucro Líquido)
- **Semi-Aditivas**: podem ser agradas para algumas dimensões, não todas (Ex: Saldo em Conta).
- **Não Aditivas**: nunca podem ser agregadas (Ex: Taxas e Percentuais).

---
## Tabelas Dimensão

- Tabela com os atributos **qualitativos** (dimensões) que ajudam a analisar os fatos.
- Podem ser desnormalizadas e com hierarquia (decomposições em outras tabelas).
- Possuem uma chave primária que identificam unicamente seus registros
- São tabelas que geralmente **crescem horizontalmente**: mais atributos ou colunas.
- Respondem à pergunta: "_Quando_?", "_O que_?", "_Onde_?" e _"Quem?";_
- Exemplos:
	- Nome
	- CPF
	- Data Nascimento
	- Dia da Semana
	- Código