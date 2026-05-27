---
disciplina: Tecnologia da Informação
tópico: Ciência de Dados
created: 2026-05-27T11:10:00
updated: 2026-05-27T11:15:00
---

## Papéis Clássicos

O DMBOK apresenta um conjunto de papéis clássicos de governança de dados e suas respectivas responsabilidades:

### DATA OWNER

- Também chamado de **Dono ou Gestor de Dados**
- Administrador de Dados de Negócio (**Business Data Steward**)
- **Possui autoridade de aprovação para decisões sobre dados dentro de seu domínio**.
- Responsável pela **qualidade**
- Representa os **stakeholders**

### TECHNICAL DATA STEWARD

- Também chamado de Administrador, Mantenedor, Curador ou Custodiante de Dados
- **São profissionais de TI que operam dentro de áreas de conhecimento técnico**.
- Responsável pela **implementação técnicas e operações de armazenamento**
- Garante **segurança** e **disponibilidade**

### DATA PRODUCERS

Também chamados de Produtores ou Criadores de Dados, são os **responsáveis por criar ou capturar os dados que alimentam os processos de negócios**.

### DATA CONSUMERS

Também chamados de Consumidores de Dados, são aqueles que se **beneficiam diretamente das entregas primárias de dados ou utilizam os dados para executar suas funções**. 

---
## Data Stewardship

Processo de gerenciamento de ciclo de vida dos dados para garantir que sejam **PRECISOS**, **DISPONÍVEIS**, **SEGUROS** e em **CONFORMIDADE**.

### Atividades

1. Gerenciamento de Metadados Principais
2. Documentação de Regras e Padrões
3. Gerenciamento de Problemas de Qualidade
4. Execução Operacional da Governança

---
## Modelos Operacionais de Governança de Dados

![[Pasted image 20260527113606.png]]

### Modelo Centralizado

No Modelo Centralizado, uma **única organização de governança de dados supervisiona todas as atividades em todas as áreas temáticas**.

### Modelo Replicado (Colegiado)

No Modelo Replicado, **cada unidade de negócio adota o mesmo modelo operacional e padrões de governança de dados**.

### Modelo Federado (Compartilhada)

O Modelo Federado combina elementos centralizados e descentralizados. Uma organização central de governança de dados coordena com várias unidades de negócios para manter definições e padrões consistentes, enquanto permite certa autonomia local.

---
## Dama Wheel

Funciona como um mapa conceitual que mostra como a governança de dados está no centro e como as demais **áreas** se conectam para garantir que os dados sejam tratados como um ativo estratégico.

Em volta dela estão dez áreas especializadas, como:

### Data Governance (Governança de Dados)
- Direciona e supervisiona o gerenciamento de dados, estabelecendo um sistema de direitos de decisão sobre os dados relevantes para as necessidades organizacionais.
### Data Architecture (Arquitetura de Dados)
- Define o plano para o gerenciamento de ativos de dados, alinhando-se às estratégias organizacionais para o estabelecimento de requisitos estratégicos de dados e os designs para atendimento destes requisitos.
### Data Modeling and Design (Modelagem e Design de Dados)
- processo de descoberta, análise, representação e comunicação de requisitos de dados por meio de uma forma precisa de representação, o modelo de dados.
### Data Storage and Operations (Armazenamento de Dados e Operações)
- Inclui o design, a implementação e o suporte ao armazenamento de dados de modo a maximizar o seu valor. Operações proveem suporte ao ciclo de vida dos dados, desde o planejamento ao descarte.

### Data Security (Segurança de Dados)
- Assegura a manutenção da privacidade e da confidencialidade dos dados, que os mesmos não sejam violados e que sejam acessados de modo apropriado.

### Data Integration and Interoperability (Integração e Interoperabilidade de Dados):
- Inclui processos relacionados à movimentação e consolidação de dados entre bancos de dados, sistemas e organizações.

### Document and Content Management (Gerenciamento de Documentos e Conteúdos):
- Inclui o planejamento, a implementação e as atividades de controle utilizadas para gerenciar o ciclo de vida de dados e informações encontradas em uma variedade de mídias não estruturadas e semi-estruturadas, especialmente documentos necessários para o suporte a requisitos de conformidade legal e regulatória.

### Reference and Master Data (Dados Mestres e de Referência)
- Inclui **reconciliação e manutenção contínuas de dados críticos compartilhados entre sistemas**, de modo a possibilitar que estes acessem as versões mais precisas, atualizadas e relevantes das entidades essenciais para o negócio.

### Data Warehousing and Business Intelligence (Data Warehousing e Business Intelligence)
- Inclui os processos de planejamento, implementação e controle para o gerenciamento de tomadas de decisão orientadas a dados, permitindo que as pessoas obtenham valor a partir de dados por meio de análise e relatórios.

### Metadata (Metadados)
- Inclui o planejamento, a implementação e o controle das atividades necessárias para possibilitar o acesso a metadados integrados e de alta qualidade, incluindo definições, modelos, fluxos de dados e outras informações necessárias para o entendimento dos dados e dos sistemas onde os mesmos foram criados, são mantidos e acessados.

### Data Quality (Qualidade de Dados)
- Inclui o planejamento e a implementação de técnicas de gerenciamento da qualidade para medir, avaliar e melhorar a adequação dos dados para uso organizacional.

![[Pasted image 20260527115126.png]]

---
## Dimensões da Qualidade de Dados

As principais dimensões de Qualidade de Dados são:
- **Acurácia**
- **Completude**
- **Unicidade**
- **Consistência**
- **Validade**
- **Temporalidade**

### Acurácia – Accuracy

Considerada por muitos autores a Dimensão de Qualidade de Dados mais importante, **representa o quão corretamente os dados descrevem** o “mundo real”. Se não houver precisão, a informação pode não ser válida para uso.
### Completude – Completeness

A completude é a **proporção de dados existentes em relação a todos os atributos presentes**. Em outras palavras, avaliaremos quanta informação está faltando em cada item dos nossos dados.
### Unicidade – Uniqueness

A Unicidade, ou Singularidade, é uma Dimensão de Qualidade de Dados que se refere a **termos apenas um registro único de algo** – por exemplo, um número de identificação.
### Consistência – Consistency

A Dimensão de Consistência diz que **deve-se comparar um item de uma  base de dados ou dataset com a mesma representação desse item em outro local**.
### Validade – Validity

Essa Dimensão de Qualidade de Dados **compara a representação do dado em relação a sua definição**. Avaliaremos o formato, tipo, valores permitidos e outros atributos do dado.
### Temporalidade – Timeliness

É a capacidade que o dado tem de **representar corretamente um momento no tempo**. Tem também relação com a velocidade de atualização dos dados. Um problema nesta dimensão também indica problemas na Precisão dos dados.
