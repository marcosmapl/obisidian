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

- **5 características essenciais** → ver [[Características Essenciais]]
- **3 modelos de serviço** → ver [[Modelos de Serviço]]
- **4 modelos de implantação** → ver [[Modelos de Implantação]]

## Atores (ISO/IEC 17788 e NIST SP 500-292)

- **Consumidor (Cloud Consumer)**: pessoa ou organização que utiliza os serviços de nuvem.
- **Provedor (Cloud Provider)**: entidade responsável por disponibilizar os serviços de nuvem.
- **Auditor (Cloud Auditor)**: realiza avaliação independente dos serviços (segurança, desempenho, conformidade).
- **Corretor (Cloud Broker)**: intermedeia, agrega e gerencia o uso e a entrega de serviços entre consumidores e provedores.
- **Operador de rede (Cloud Carrier)**: provê a conectividade e o transporte dos serviços entre provedor e consumidor.

## Vantagens

- **Redução de custos**: elimina investimentos iniciais em infraestrutura (CAPEX → OPEX).
- **Escalabilidade e elasticidade**: recursos crescem ou diminuem conforme a demanda.
- **Pagamento por uso** (*pay-as-you-go*): cobra-se apenas pelo que é consumido.
- **Alta disponibilidade**: redundância geográfica e acordos de nível de serviço (SLA).
- **Agilidade**: provisionamento rápido de ambientes e serviços.

## Desvantagens e riscos

- **Dependência do provedor** (*vendor lock-in*): dificuldade de migrar entre provedores.
- **Dependência de conectividade**: sem rede, não há acesso aos serviços.
- **Segurança e privacidade**: dados sob custódia de terceiros; atenção à LGPD e à soberania dos dados.
- **Menor controle**: o consumidor não administra a infraestrutura subjacente.
