---
disciplina: Tecnologia da Informação
tópico: Computação em Nuvem
created: 2026-11-09T19:45:00
updated: 2026-11-09T19:45:00
---

> [!info] Definição
> Os **modelos de implantação** definem **quem pode usar** a infraestrutura de nuvem e **onde ela está localizada**. O NIST SP 800-145 define quatro modelos: **pública, privada, comunitária e híbrida**.

## Nuvem Pública (*Public Cloud*)

- Infraestrutura provisionada para **uso aberto pelo público em geral**.
- Pertence e é operada por **empresa, instituição acadêmica ou órgão governamental** (ou combinação deles), existindo **nas instalações do provedor**.
- **Recursos compartilhados** entre múltiplos clientes (multi-inquilino).
- Vantagens: menor custo, alta escalabilidade. Desvantagem: menor controle.
- **Exemplos**: AWS, Microsoft Azure, Google Cloud.

## Nuvem Privada (*Private Cloud*)

- Infraestrutura provisionada para **uso exclusivo de uma única organização** (com múltiplas unidades de negócio).
- Pode ser **de propriedade, gerenciada e operada** pela própria organização, por terceiros, ou combinação — e pode existir **dentro ou fora** das instalações da organização.
- Vantagens: maior controle, segurança e personalização. Desvantagens: maior custo e responsabilidade.

> [!warning] Pegadinha de prova
> Nuvem privada **não precisa estar** fisicamente nas instalações da organização, nem ser operada por ela — o que a define é o **uso exclusivo**.

## Nuvem Comunitária (*Community Cloud*)

- Infraestrutura provisionada para **uso exclusivo de uma comunidade de organizações** com **interesses em comum** (missão, requisitos de segurança, políticas, conformidade).
- Pode ser gerenciada por uma ou mais organizações da comunidade, por terceiros, ou combinação; dentro ou fora das instalações.
- Exemplo típico: nuvens compartilhadas entre **órgãos públicos** de uma mesma esfera.

## Nuvem Híbrida (*Hybrid Cloud*)

- **Composição de duas ou mais infraestruturas distintas** (privada, comunitária ou pública) que **permanecem entidades únicas**, mas são **interligadas por tecnologia padronizada ou proprietária** que permite portabilidade de dados e aplicações.
- Caso de uso clássico: ***cloud bursting*** — transbordo de carga da nuvem privada para a pública em picos de demanda.

## Conceitos relacionados

- **Multicloud**: uso de **múltiplos provedores de nuvem** (ex.: AWS + Azure) para evitar *vendor lock-in* e aumentar resiliência. Difere da híbrida: multicloud não exige integração entre as nuvens nem combinação de modelos distintos.
- **Nuvem governamental (GovCloud)**: regiões/ofertas dedicadas ao setor público, com requisitos adicionais de conformidade e soberania de dados.
