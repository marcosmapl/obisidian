---
disciplina: Tecnologia da Informação
tópico: Ciência de Dados
created: 2026-05-27T11:10:00
updated: 2026-05-27T11:15:00
---

## Papéis Clássicos

O DMBOK apresenta um conjunto de papéis clássicos de governança de dados e suas respectivas responsabilidades:

### Data Steward (Owner)

- Também chamado de **Dono ou Gestor de Dados**
- Custodião/Zelador de Dados
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

> [!note] Dados Mestres (Master Data)
> **Dados críticos e compartilhados** sobre entidades de negócio fundamentais (ex: clientes, produtos, funcionários). 
> A gestão de dados mestres (MDM) busca uma **"versão única da verdade"**.
> ==Atenção: Dados mestres NÃO armazenam informações sobre tabelas e sua localização física; isso é papel dos metadados==.

> [!note] Linhagem de Dados (Data Lineage)
> Documenta a origem dos dados, suas transformações e movimentações ao longo do tempo. Essencial para rastreabilidade e análise de impacto.

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
- **Acurácia**: Representação correta da realidade.
- **Completude**: proporção de dados existentes em relação a todos os atributos presentes.
- **Unicidade**: ausência de duplicidade.
- **Consistência**: ausência de contradições entre dados.
- **Validade**: conformidade com formatos e regras.
- **Tempestividade/Oportunidade**: disponibilidade no tempo certo.
- **Performance**: tempo de resposta e acesso satisfatório.

---
## Documentos e Artefatos

- **Políticas de Dados**: regras de alto nível
- **Normas/Padrões**: práticas recomendadas ou obrigatórias
- **Procedimentos**: "como fazer" tarefas específicas

> [!tip] Documento principal
> O manual de normas e padrões NÃO é o principal documento; a Política de Governança de Dados é mais fundamental.

---
## Tópicos Relacionados

- [[Técnicas de Qualidade de Dados]]
