---
disciplina: Tecnologia da Informação
tópico: Business Intelligence
created: 2026-02-06T04:55:00
updated: 2026-02-06T05:00:00
---
## Fontes de Dados

- CRM/ERP
- Sistemas legados
- Banco de Dados
- API
- Planilhas Eletrônicas
- Documentos

---
## Processo ETL

- **Seleção**: define o que será utilizado
- **Extração**: coleta os dados das fontes.
	- Completa
	- Incremental
	- CDC
	- Em Lote
	- Tempo Real
- **Transformação**: limpeza, padronização ("SP" e "São Paulo"), deduplicação, enriquecimento (Ex: faixas etárias), cálculos e conformidades de chaves.
- **Integração**: consolida os dados de diversas fontes num modelo comum
- **Carga**: grava os dados em ODS/Staging Area, posteriormete os dados são levados para o Data Warehouse

### Operation Data Store (ODS) x Staging Area

**Staging Area (área de estágio)**  
É a camada **temporária** onde os dados extraídos das fontes são armazenados **brutos ou quase brutos** apenas para processamento ETL.

**ODS (Operational Data Store)**  
É um repositório **integrado, limpo e consultável**, com dados atuais, usado como **base operacional intermediária** antes do Data Warehouse.

|Aspecto|Staging Area|ODS|
|---|---|---|
|Finalidade|Suporte técnico ao ETL|Integração operacional dos dados|
|Persistência|Temporária|Persistente (curto prazo)|
|Qualidade dos dados|Brutos / parcialmente tratados|Limpos, integrados e padronizados|
|Estrutura|Próxima às fontes|Normalizada e consistente|
|Acesso por usuários|Não|Pode ser consultado|
|Tempo de retenção|Horas ou dias|Dias ou semanas|
|Papel no fluxo|Extração → transformação|Integração → preparação para DW|

**Fluxo típico com ambos**
- **Fontes → Staging → Transformações → ODS → Data Warehouse → BI**
	- **Staging** = área técnica de processamento
	- **ODS** = camada de dados operacionais confiáveis

**Analogia simples**
- **Staging** → “mesa de triagem bagunçada” onde chegam os dados brutos.
- **ODS** → “estoque organizado” pronto para uso operacional e envio ao Data Warehouse.

Use **Staging** quando precisar:
- Carregar dados brutos temporariamente
- Executar ETL pesado
- Isolar falhas de carga

Use **ODS** quando precisar:
- Integrar sistemas operacionais
- Disponibilizar dados recentes confiáveis
- Alimentar o Data Warehouse com qualidade

---
## Data Warehouse

Depois de passar pelo ETL, os dados chegam ao **Data Warehouse**, o grande repositório central onde tudo fica armazenado de forma integrada, segura e pronta para análise. Aqui, temos dois componentes importantes:

- **Metadados:** informações sobre os dados armazenados no DW, como estruturas e atributos de tabelas, especificações do modelo de dados, rotinas de acesso, log de extrações, entre outros;
    
- **Replicação:** mecanismos para copiar e sincronizar dados entre diferentes sistemas e o Data Warehouse. Isso garante a continuidade de negócio e reduz latência para filiais/regiões.

No DW, os dados são organizados em estruturas próprias, como:
- **Tabelas Fato:** com os dados numéricos e eventos (como vendas, acessos, pagamentos).
- **Tabelas Dimensão:** com os atributos que ajudam a analisar os fatos (professores, cursos, datas, etc).

![[Pasted image 20260206060956.png]]

### Data Mart

os Data Warehouses podem ser subdivididos em Data Marts, que são como “fatias” do DW focadas em áreas específicas da empresa — como marketing, finanças ou recursos humanos.

---
## API e Middlewares

Os usuários finais e as aplicações não acessam o DW diretamente. Existe uma camada intermediária — composta por middlewares, conectores e APIs — que faz essa ponte, garantindo que o acesso seja eficiente, seguro e escalável.

---
## Visualização

É aqui que os dados, já tratados e organizados, são transformados em gráficos, relatórios, painéis e dashboards interativos. Com isso, analistas, gestores e executivos conseguem explorar informações, identificar tendências, acompanhar indicadores e tomar decisões com base em evidências reais.

---
## Resumo
 
![[ChatGPT Image Feb 6, 2026, 05_17_35 AM.png]]