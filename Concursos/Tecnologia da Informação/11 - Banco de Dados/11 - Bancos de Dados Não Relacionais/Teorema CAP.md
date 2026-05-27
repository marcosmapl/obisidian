---
disciplina: Tecnologia da Informação
tópico: Bancos de Dados Não Relacionais
created: 2026-03-11T05:15:00
updated: 2026-03-11T05:15:00
---

## Conceito

O **Teorema CAP** afirma que um sistema distribuído **não pode garantir simultaneamente três propriedades**.

Ele pode garantir **no máximo duas das três**
### Consistência (Consistency)

Todos os nós veem **os mesmos dados ao mesmo tempo**.

Após uma escrita, qualquer leitura retorna **o valor mais recente**.

---
### Disponibilidade (Availability)

Todo pedido recebe **uma resposta**, mesmo que **não seja a versão mais recente dos dados**.

O sistema continua funcionando mesmo com falhas.

---
### Tolerância à Partição (Partition Tolerance)

O sistema continua operando **mesmo com falhas de comunicação entre nós** da rede.

Essa característica é **essencial em sistemas distribuídos modernos**.

---
### Combinações possíveis

|Modelo|Característica|
|---|---|
|**CP**|Consistência + Tolerância à partição|
|**AP**|Disponibilidade + Tolerância à partição|
|**CA**|Consistência + Disponibilidade (sem tolerância a partições)|

Em sistemas distribuídos reais, geralmente assume-se **P**, restando escolher entre **C ou A**.