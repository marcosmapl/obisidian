
## Metodologia de Auditoria de Segurança da Informação

*Incidência: Baixa*

Uma auditoria de segurança da informação segue, tipicamente, uma sequência lógica: primeiro se conhece o ambiente (inventário de informações, sistemas e rede) e, só depois, se avalia a adequação dos controles já existentes frente a esse ambiente.

|Etapa|O que verifica|
|---|---|
|**Inventário de informações**|O que está armazenado na rede, quais sistemas operacionais e ativos existem — o "raio-x" inicial do ambiente.|
|**Revisão da PSI**|Verificação aprofundada dos procedimentos de segurança já existentes e conferência de sua aderência aos padrões exigidos.|
|**Avaliação de riscos**|Identificação de ameaças e vulnerabilidades, análise do ambiente de controle para dimensionar risco e impacto potencial.|
|**Configuração de firewall**|Verificação do principal dispositivo de barreira contra acessos indevidos, incluindo a política de acesso remoto.|
|**Teste de penetração**|Simulação de ataques reais a sistemas, redes e aplicações web para identificar vulnerabilidades exploráveis.|

O Bizu do Tópico

Regra de Ouro para provas:

- A banca costuma trocar **PSI** (Política de Segurança da Informação) por **PETI** ou **PDTI** nas alternativas — PETI/PDTI são planos estratégicos/diretores de TI, não o documento de segurança revisado nessa etapa.
- Não confundir **teste de estresse** (mede desempenho sob carga) com **teste de penetração** (busca vulnerabilidades exploráveis) — a simulação de ataque real é sempre penetração.

**Pegadinha clássica FCC:** trocar "Avaliação de riscos" por "Definição do Plano de contingência" — plano de contingência é resposta a um risco já mapeado, não a etapa de identificá-lo.

**Macete:** Inventário → PSI → Riscos → Firewall → Pentest (do mais amplo ao mais técnico).

2. Técnicas de Auditoria Assistida por Computador (TAACs)Incidência: Alta

TAACs (ou CAATs, em inglês) são técnicas que usam o computador como ferramenta para coletar e analisar evidências de auditoria em ambientes informatizados. A escolha da técnica certa é o ponto mais cobrado do assunto.

|Técnica|Como funciona|
|---|---|
|**Simulação Paralela**|O auditor desenvolve seu próprio programa, reprocessa os dados reais já lançados pela gestão com os mesmos parâmetros/requisitos originais e compara os resultados com os obtidos pelo sistema.|
|**Integrated Test Facility (ITF)**|O auditor insere um subsistema fictício (entidade de teste) dentro do sistema principal, processando dados fictícios junto com transações reais de outros segmentos — gera relatórios separados para análise, sem contaminar a produção.|
|**Simulação de Dados / Test Deck**|O auditor elabora uma massa de testes (campos inválidos, valores-limite, transações incompletas, incompatíveis ou duplicadas) e a submete ao programa em ambiente controlado, avaliando se os controles programados reagem como esperado.|
|**Rastreamento de Programas**|Acompanha passo a passo a lógica interna do programa durante a execução, permitindo enxergar o caminho percorrido pelo processamento.|
|**Mapeamento Estatístico (mapping)**|Identifica quais trechos de código foram efetivamente executados — útil para localizar código morto, não testado ou potencialmente fraudulento.|
|**Análise de Log / Accounting**|Exame das trilhas de auditoria (logs) para detectar erros de programa/operação, uso de programas fraudulentos e tentativas de acesso indevido em dispositivos e aplicativos da rede.|
|**Ferramentas Generalistas de Auditoria**|Softwares (tipo ACL/IDEA) que processam simultaneamente diversos arquivos e diferentes formatos, fazem amostragem estatística, sumarizam e apontam duplicidades — e ainda permitem integração com vários softwares e hardwares.|

### Abordagem Através do Computador × Abordagem Ao Redor do Computador

#### Através do Computador

O auditor examina a lógica interna do processamento (o "miolo" do programa) — usa TAACs como rastreamento, mapping ou test deck para abrir a caixa-preta.

#### Ao Redor do Computador

O auditor confere apenas as entradas e saídas do processamento, sem examinar a lógica interna — trata o sistema como uma caixa-preta e faz a auditoria "por fora".

O Bizu do Tópico

Regra de Ouro para provas:

- Todo enunciado que descreve **massa de testes com dados fictícios em ambiente separado** = **Test Deck / Simulação de Dados**, mesmo que a questão troque o nome da técnica nas alternativas.
- ITF = dados fictícios **misturados** com dados reais de produção, dentro do sistema real. Test Deck/Simulação = dados de teste em ambiente **separado** da produção.
- **Ferramentas generalistas** (GAS) são valorizadas justamente por processar **múltiplos formatos diferentes** ao mesmo tempo — exigir "mesmo formato" é a pegadinha que inverte o conceito.

**Pegadinha clássica FCC:** descrever "conferir apenas entradas e saídas" e chamar de "avaliação de caixa branca" — caixa branca examina a lógica interna (é o oposto); o nome correto é **abordagem ao redor do computador** (caixa-preta).

**Macete:** Redor = por FORA (entrada/saída) | Através = por DENTRO (lógica/código).

3. Controles Internos e Segregação de FunçõesIncidência: Média

### Modos de Implantação dos Controles Internos

#### Preventivo

Orienta para que sejam evitadas as ocorrências de falhas, desperdícios, irregularidades e ilegalidades — atua antes do fato.

#### Detectivo

Constata falhas, desperdícios e irregularidades sanáveis que ocorrem durante a realização dos fatos — atua durante/logo após.

#### Corretivo

Aponta falhas, desperdícios e irregularidades já consumadas, sanáveis ou insanáveis, ocorridas após os fatos — atua depois.

### Segregação de Funções (Segregation of Duties — SoD)

- Método para reduzir o risco de uso acidental ou deliberado indevido dos sistemas, dividindo responsabilidades entre pessoas distintas.
- O **início de um evento** (ex.: emitir um pedido de compra) deve ser separado de sua **autorização** e da **confirmação/recebimento**.
- Atividades que, juntas, permitiriam a um único indivíduo concretizar uma fraude devem ser segregadas entre pessoas diferentes — o objetivo é justamente dificultar o conluio, e não concentrar a atividade em uma só pessoa.
- Na prática de acessos, a segregação se materializa com **RBAC** (Role Based Access Control — perfis de acesso por função) combinado a **SoD**, evitando conflitos de perfis e privilégios excessivos.
- Quando funções antagônicas são exercidas cumulativamente pela mesma pessoa (lançar, aprovar e liberar pagamento, por exemplo), abre-se espaço para fraude — a solução é segregar, não terceirizar ou trocar de responsável.

### Ambiente de Controle

Componente do controle interno relacionado às diretrizes, políticas e à cultura organizacional (o "tom no topo"): documentos que estabelecem regras gerais e comunicam responsabilidades aos colaboradores fazem parte do **ambiente de controle**, e não de uma atividade de controle específica.

O Bizu do Tópico

Regra de Ouro para provas:

- Preventivo = **antes** · Detectivo = **durante** · Corretivo = **depois**. A banca gosta de trocar o momento de cada um nas definições.
- Segregação de funções nunca é resolvida com **terceirização do controle** — o problema é a concentração de poderes, não quem exerce o cargo.

**Pegadinha clássica FCC:** afirmar que, para reduzir risco de conluio, os controles devem ser planejados de modo que "somente uma pessoa esteja envolvida" — ERRADO. É exatamente o oposto: conluio se combate **distribuindo** a execução entre mais pessoas, para exigir cumplicidade de várias.

**Macete:** Regras gerais/diretrizes de conduta → Ambiente de Controle | Controle específico embutido num processo → Atividade de Controle.

4. Risco de Auditoria, Amostragem e Tipos de TesteIncidência: Média

**Risco de auditoria** é o risco de o auditor emitir uma opinião ou parecer inadequado diante dos fatos reais — por exemplo, apontar uma causa para uma distorção sem comprovação técnica suficiente que a sustente.

### Teste de Conformidade × Teste Substantivo

#### Teste de Conformidade

Avalia se os controles internos estão sendo cumpridos e operando como desenhado — foco na **adesão às regras** (ex.: regras de atestação e revogação de acesso).

#### Teste Substantivo

Busca evidência direta sobre a ocorrência do fato/transação em si (o que de fato aconteceu) — comprova valores, saldos e eventos concretos.

- Tentativas de violação de regras de acesso **podem ocorrer acidentalmente** (não apenas de forma intencional) e sua ocorrência concreta deve ser comprovada por **testes substantivos**; já a adequação das próprias regras de acesso e dos controles internos deve ser avaliada por **testes de conformidade**.

### Amostragem em Auditoria

- Quando o **risco de amostragem** é grande e a organização aceita trabalhar com uma **taxa aceitável de desvio maior**, sendo a **taxa esperada de desvio pequena**, a folga entre o esperado e o aceitável permite usar uma amostra **menor** — não é preciso ampliar o espaço amostral.
- Quando uma auditoria por amostragem já revelou falha em controles internos, o passo seguinte para aprofundar o exame de forma planejada e minuciosa é a **revisão integral** (exame de 100% dos itens), e não uma nova amostragem.

O Bizu do Tópico

Regra de Ouro para provas:

- Conformidade fiscaliza **o controle** (a regra está sendo seguida?); Substantivo fiscaliza **o fato** (o que realmente aconteceu?).
- Falha achada por amostra → aprofundar é sinônimo de **revisão integral**, não de "mais amostra".

**Pegadinha clássica FCC:** afirmar que violações de acesso "ocorrem sempre intencionalmente" — ERRADO. Podem ser acidentais; por isso a auditoria precisa de evidência (teste substantivo) e não apenas de suposição de má-fé.

**Macete:** Conformidade = **regra** · Substantivo = **fato**.

5. Planejamento, Programa e Tipos de AuditoriaIncidência: Alta

Um **conjunto de auditorias planejado para um determinado período de tempo**, com um propósito específico (ex.: avaliar a integridade dos dados nas interfaces entre sistemas), constitui um **Programa de Auditoria** — e não um projeto isolado.

### Ciclo do Programa de Auditoria

|Ordem|Etapa|
|---|---|
|1|**Definir os objetivos** do programa.|
|2|**Detalhar o programa** (escopo, recursos, cronograma).|
|3|**Implementar o programa.**|
|4|**Monitorar o programa.**|
|5|**Analisar e melhorar o programa.**|

### Escopo da Auditoria de TI

#### Auditoria de Aplicativos

Avalia controles específicos embutidos nas transações, voltados a prevenir, detectar e corrigir erros e irregularidades durante entrada, processamento e saída de dados.

#### Controles Gerais

Avaliam o ambiente de TI como um todo — entre eles, os **controles de acesso**, que limitam ou detectam o acesso a recursos computacionais, protegendo contra modificação não autorizada, perda e divulgação indevida de informações.

- Fatores de risco realmente **auditáveis** na gestão de ativos de TI são operacionais e concretos (ex.: procedimento de suporte técnico) — não elementos estratégicos e intangíveis como "cultura de gestão de riscos" ou "capital disponível".

### Espécies de Auditoria (classificação por finalidade)

|Espécie|Foco|
|---|---|
|**Acompanhamento da Gestão**|Atuação tempestiva sobre atos efetivos e efeitos potenciais (positivos e negativos), evidenciando melhorias e economias e prevenindo gargalos ao desempenho da missão institucional.|
|**Inspeção**|Verificação pontual e específica de fatos ou situações determinadas, geralmente decorrente de denúncia ou necessidade de esclarecimento.|
|**Especial**|Exame de fatos que fogem do planejamento regular, por determinação superior ou situação excepcional.|
|**Levantamento**|Conhecer a organização, seus sistemas e identificar objetos e escopos para futuras fiscalizações.|

O Bizu do Tópico

Regra de Ouro para provas:

- Programa ≠ Projeto: **programa** é um conjunto de auditorias recorrentes; **projeto** é algo pontual e finito.
- "Prevenir, detectar e corrigir erros na entrada/processamento/saída" é a **definição-padrão de Auditoria de Aplicativos** — decore essa frase.
- "Atuação tempestiva + evidenciar melhorias/economias + prevenir gargalos na missão institucional" é a **definição-padrão de Acompanhamento da Gestão**.

**Macete do ciclo:** **D-D-I-M-A** → Definir → Detalhar → Implementar → Monitorar → Analisar/melhorar.

6. Papéis de Trabalho, Evidências e Produtos da AuditoriaIncidência: Média

- **QACI** (Questionário de Avaliação de Controle Interno) é o instrumento que reúne questões objetivas, escalas do tipo Likert e espaço para comentários, usado para auxiliar a avaliação dos controles internos que mitigam os riscos do processo auditado.
- **Papéis de trabalho** são todos os registros produzidos e coletados pelo auditor durante o trabalho — inclusive relatórios técnicos ou consultas (ex.: consultas SQL a bancos de dados) usados para embasar as conclusões.
- **Constatações (achados) de auditoria** resultam da comparação entre os **critérios** estabelecidos (o que deveria ser) e as **evidências** coletadas (o que de fato foi encontrado).

|Produto da Auditoria|Conteúdo|
|---|---|
|**Relatório de fraquezas de controle interno**|Objetivo do projeto de auditoria, pontos de controle auditados, conclusão sobre cada ponto e alternativas de solução propostas.|

O Bizu do Tópico

Regra de Ouro para provas:

- Achado de auditoria = **Critério** (o esperado) **vs.** **Evidência** (o encontrado). Decore essa fórmula — é definição literal cobrada em prova.
- "Papel de trabalho" é um conceito amplo: qualquer registro do que o auditor fez, viu ou consultou entra nessa categoria — inclusive relatórios técnicos gerados por terceiros usados como suporte.

**Pegadinha clássica FCC:** inventar nomes de produtos de auditoria que soam técnicos ("Certificado de controle interno", "Relatório de aumento de custos") mas não correspondem a produtos reais — desconfie de nomenclaturas que a literatura de auditoria não usa.

**Macete:** Achado = Critério **−** Evidência (a diferença entre os dois é o próprio achado).

7. Complementares — Logs, Contratos e Licitações de TIIncidência: Baixa

### Cuidados com Logs de Eventos e Segurança

- Se o número de objetos auditados cresce muito, o log de segurança pode atingir sua capacidade e, conforme a configuração, forçar o desligamento do computador.
- Logs de eventos cheios param de registrar informações — configura-se o método de retenção para que entradas antigas sejam substituídas pelas recentes.
- Remover eventos antigos abre brecha para que invasores gerem eventos "de cobertura" e apaguem evidências de ataque — o risco se reduz automatizando arquivamento e backup dos logs.
- Mesmo com diretivas corretas de tamanho e retenção, é possível, sim, detectar e rastrear atividades não autorizadas — dizer que isso é "impossível" é sempre a alternativa incorreta.

### Fiscalização de Contratos de TI

A entidade contratante **não pode** transferir integralmente ao fornecedor a responsabilidade por reportar entregas — é obrigatório existir um **preposto/fiscal do contrato** por parte da contratante para acompanhar a execução no local.

### Licitações Internacionais de Bens e Serviços de Informática

- O edital deve estar ajustado às diretrizes da **política monetária e do comércio exterior**.
- Não é correto priorizar fornecedores estrangeiros em detrimento de fornecedores nacionais que atendam às normas técnicas brasileiras.

O Bizu do Tópico

Regra de Ouro para provas:

- Toda vez que a alternativa disser que algo é "**impossível** detectar" mesmo com controles adequados, desconfie — é o tipo de afirmação absoluta que costuma ser a incorreta.
- Contrato de TI sem preposto da contratante é sempre **irregular**, independentemente de o fornecedor cumprir bem sua parte.

**Macete:** Log cheio → sobrescreve (retenção) + backup automatizado = mitigação padrão cobrada em prova.