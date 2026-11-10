---
disciplina: Tecnologia da Informação
tópico: Computação em Nuvem
created: 2026-11-09T19:45:00
updated: 2026-11-09T19:45:00
---

> [!info] Definição
> Os **modelos de serviço** definem **o que é entregue** ao consumidor e **qual o nível de controle e responsabilidade** de cada parte. O NIST SP 800-145 define três modelos: **IaaS, PaaS e SaaS**.

## IaaS — Infraestrutura como Serviço

- Entrega **recursos de infraestrutura**: processamento, armazenamento, redes e outros recursos computacionais fundamentais.
- O consumidor **não gerencia a infraestrutura física**, mas **controla** sistemas operacionais, armazenamento e aplicações instaladas (e, possivelmente, componentes de rede como firewalls).
- **Maior controle e maior responsabilidade** do consumidor entre os três modelos.
- **Exemplos**: Amazon EC2, Google Compute Engine, Azure Virtual Machines.

## PaaS — Plataforma como Serviço

- Entrega uma **plataforma para desenvolvimento, teste e implantação** de aplicações (linguagens, bibliotecas, serviços e ferramentas suportados pelo provedor).
- O consumidor **controla apenas as aplicações implantadas** e suas configurações; **não gerencia** SO, servidores, armazenamento ou rede.
- Público-alvo típico: **desenvolvedores**.
- **Exemplos**: Heroku, Google App Engine, Azure App Service.

## SaaS — Software como Serviço

- Entrega **aplicações prontas** em execução na infraestrutura do provedor, acessadas via navegador ou interface de programa.
- O consumidor **não gerencia nada da infraestrutura ou da plataforma**; no máximo, ajusta **configurações específicas do usuário**.
- **Menor controle e menor responsabilidade** do consumidor.
- **Exemplos**: Gmail, Microsoft 365, Salesforce.

## Comparativo de responsabilidades

| Camada | On-premises | IaaS | PaaS | SaaS |
|---|---|---|---|---|
| Aplicação | Consumidor | Consumidor | Consumidor | **Provedor** |
| Runtime / Middleware | Consumidor | Consumidor | **Provedor** | **Provedor** |
| Sistema Operacional | Consumidor | Consumidor | **Provedor** | **Provedor** |
| Virtualização | Consumidor | **Provedor** | **Provedor** | **Provedor** |
| Servidores / Rede / Storage | Consumidor | **Provedor** | **Provedor** | **Provedor** |

## Outros modelos (XaaS)

- **FaaS (Function as a Service)** / ***Serverless***: execução de funções sob demanda, sem gerenciar servidores; cobrança por execução. Ex.: AWS Lambda, Azure Functions.
- **DaaS (Desktop as a Service)**: desktops virtuais entregues pela nuvem.
- **DBaaS (Database as a Service)**: banco de dados gerenciado. Ex.: Amazon RDS.
- **STaaS (Storage as a Service)**: armazenamento como serviço → ver [[Armazenamento em Nuvem]].
