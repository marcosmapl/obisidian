---
disciplina: Tecnologia da Informação
tópico: Computação em Nuvem
created: 2026-11-09T19:45:00
updated: 2026-11-09T19:45:00
---

> [!info] Definição (NIST SP 800-145)
> **Computação em Nuvem** é um modelo que permite **acesso ubíquo, conveniente e sob demanda**, via rede, a um **conjunto compartilhado de recursos computacionais configuráveis** (redes, servidores, armazenamento, aplicações e serviços), que podem ser **rapidamente provisionados e liberados com mínimo esforço de gerenciamento** ou interação com o provedor de serviços.

## Composição do modelo NIST

O modelo de nuvem do NIST é composto por:

### Características Essenciais

#### Autoatendimento sob demanda (*On-demand self-service*)

O consumidor pode **provisionar recursos computacionais unilateralmente**, de forma automática, **sem necessidade de interação humana** com o provedor.

#### Amplo acesso à rede (*Broad network access*)

Os recursos estão **disponíveis pela rede** e são acessados por **mecanismos padronizados**, a partir de plataformas heterogêneas (celulares, tablets, notebooks, estações de trabalho).

#### Agrupamento de recursos (*Resource pooling*)

Os recursos do provedor são **agrupados (pool)** para atender **múltiplos consumidores** em modelo **multi-inquilino** (*multi-tenant*), com recursos físicos e virtuais **atribuídos e reatribuídos dinamicamente** conforme a demanda. Em geral, o consumidor **não conhece a localização exata** dos recursos.

#### Elasticidade rápida (*Rapid elasticity*)

Os recursos podem ser **provisionados e liberados elasticamente**, em alguns casos automaticamente, acompanhando a demanda. Para o consumidor, os recursos **aparentam ser ilimitados**.

#### Serviço mensurado (*Measured service*)

O uso dos recursos é **monitorado, controlado e reportado automaticamente**, com **medição** apropriada ao tipo de serviço (armazenamento, processamento, banda, usuários ativos), garantindo **transparência** para provedor e consumidor e viabilizando o modelo *pay-as-you-go*.

> [!tip] Mnemônico
> **A**utoatendimento • **A**mplo acesso • **A**grupamento • **E**lasticidade • **S**erviço mensurado — "**3A + E + S**"

### Modelos de Serviço


> [!info] Definição
> Os **modelos de serviço** definem **o que é entregue** ao consumidor e **qual o nível de controle e responsabilidade** de cada parte. O NIST SP 800-145 define três modelos: **IaaS, PaaS e SaaS**.

- [[Infraestrutura como Serviço (IaaS)]]
- [[Plataforma como Serviço (PaaS)]]
-  [[Software como Serviço (SaaS)]]


| **On-Premises**    | ==🔵IaaS==           | ==🟢PaaS==           | ==🔴SaaS==           |
| -------------- | -------------------- | -------------------- | -------------------- |
| **Applications**   | Applications         | Applications         | ==🟠Applications==   |
| **Data**           | Data                 | Data                 | ==🟠Data==           |
| **Runtime**        | Runtime              | ==🟠Runtime==        | ==🟠Runtime==        |
| **Middleware**     | Middleware           | ==🟠Middleware==     | ==🟠Middleware==     |
| **O/S**            | O/S                  | ==🟠O/S==            | ==🟠O/S==            |
| **Virtualization** | ==🟠Virtualization== | ==🟠Virtualization== | ==🟠Virtualization== |
| **Servers**        | ==🟠Servers==        | ==🟠Servers==        | ==🟠Servers==        |
| **Storage**        | ==🟠Storage==        | ==🟠Storage==        | ==🟠Storage==        |
| **Networking**     | ==🟠Networking==     | ==🟠Networking==     | ==🟠Networking==     |

### Modelos de Implantação

> [!info] Definição
> Os **modelos de implantação** definem **quem pode usar** a infraestrutura de nuvem e **onde ela está localizada**. O NIST SP 800-145 define quatro modelos: **pública, privada, comunitária e híbrida**.

- [[Nuvem Pública (Public Cloud)]]
- [[Nuvem Privada (Private Cloud)]]
- [[Nuvem Comunitária (Community Cloud)]]
- [[Nuvem Híbrida (Hybrid Cloud)]]
  
| **CARACTERÍSTICA**  | **NUVEM**  **PÚBLICA**                       | **NUVEM** **PRIVADA**                          | **NUVEM** **HÍBRIDA**                      | **NUVEM COMUNITÁRIA**                                |
| ------------------- | -------------------------------------------- | ---------------------------------------------- | ------------------------------------------ | ---------------------------------------------------- |
| **ACESSO**          | Aberto ao público (mediante pagamento)       | Restrito a uma única organização               | Combinação de pública e privada            | Compartilhado por organizações com interesses comuns |
| **PROPRIEDADE**     | Provedor de serviços (ex: AWS, Azure)        | Organização ou provedor dedicado               | Mista (organização + provedor)             | Gerida por grupo ou entidade coletiva                |
| **INFRAESTRUTURA**  | Compartilhada entre múltiplos clients        | Exclusiva de uma única empresa                 | Parte compartilhada, parte dedicada        | Compartilhada entre entidades do mesmo setor         |
| **CUSTO**           | Baixo custo inicial, modelo sob demanda      | Alto custo inicial e de manutenção             | Custo intermediário (varia com o uso)      | Custo compartilhado entre os membros                 |
| **SEGURANÇA**       | Boa, mas com menos controle sobre o ambiente | Alta (controle total sobre políticas e acesso) | Variável, dependendo da parte usada        | Alta (regras definidas entre as partes envolvidas)   |
| **ESCALABILIDADE**  | Alta                                         | Limitada à capacidade interna                  | Alta (pela parte pública)                  | Moderada                                             |
| **GERENCIAMENTO**   | Responsabilidade do provedor                 | Responsabilidade da organização                | Misto (dependendo do ambiente)             | Compartilhado entre os membros                       |
| **EXEMPLOS DE USO** | Aplicações web, startups, testes rápidos     | Instituições financeiras, dados sigilosos      | Empresas que precisam escalar com controle | Universidades, órgãos públicos, consórcios de saúde  |

---
## Atores (ISO/IEC 17788 e NIST SP 500-292)

- **Consumidor (Cloud Consumer)**: pessoa ou organização que utiliza os serviços de nuvem.
- **Provedor (Cloud Provider)**: entidade responsável por disponibilizar os serviços de nuvem.
- **Auditor (Cloud Auditor)**: realiza avaliação independente dos serviços (segurança, desempenho, conformidade).
- **Corretor (Cloud Broker)**: intermedeia, agrega e gerencia o uso e a entrega de serviços entre consumidores e provedores.
- **Operador de rede (Cloud Carrier)**: provê a conectividade e o transporte dos serviços entre provedor e consumidor.

---
## Vantagens

- **Redução de custos**: elimina investimentos iniciais em infraestrutura (CAPEX → OPEX).
- **Escalabilidade e elasticidade**: recursos crescem ou diminuem conforme a demanda.
- **Pagamento por uso** (*pay-as-you-go*): cobra-se apenas pelo que é consumido.
- **Alta disponibilidade**: redundância geográfica e acordos de nível de serviço (SLA).
- **Agilidade**: provisionamento rápido de ambientes e serviços.

---
## Desvantagens e riscos

- **Dependência do provedor** (*vendor lock-in*): dificuldade de migrar entre provedores.
- **Dependência de conectividade**: sem rede, não há acesso aos serviços.
- **Segurança e privacidade**: dados sob custódia de terceiros; atenção à LGPD e à soberania dos dados.
- **Menor controle**: o consumidor não administra a infraestrutura subjacente.
