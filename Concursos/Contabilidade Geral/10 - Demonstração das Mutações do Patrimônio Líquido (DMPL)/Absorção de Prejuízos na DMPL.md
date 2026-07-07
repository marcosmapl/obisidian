---
disciplina: Contabilidade Geral
tópico: Demonstrações Contábeis
created: 2026-07-06T00:00:00
updated: 2026-07-06T00:00:00
---

## Conceito

Quando a empresa apura **prejuízo no exercício**, ele deve ser absorvido pelas contas do PL em uma **ordem legal específica**, antes de ser mantido como saldo devedor em Prejuízos Acumulados.

---
## Ordem de absorção do prejuízo

> [!important] Memorize esta sequência — cobrada com frequência em provas!

```
1º  Lucros Acumulados (saldo anterior, se existir)
2º  Reservas de Lucros (exceto Reserva Legal)
3º  Reserva Legal
4º  Reservas de Capital
```

> [!note] Base legal
> A ordem está implícita na **Lei nº 6.404/76**, arts. 189 e 200, e é consolidada pela doutrina.

---
## Por que essa ordem?

| Etapa | Justificativa |
|---|---|
| **Lucros Acumulados** | Absorção imediata antes de atingir reservas |
| **Reservas de Lucros (exceto RL)** | Foram constituídas do lucro — revertem ao ponto de origem |
| **Reserva Legal** | Mais protegida; só absorve prejuízo após esgotar as demais reservas de lucro |
| **Reservas de Capital** | Última linha de defesa; sua finalidade principal não é absorção de prejuízo |

> [!warning] Reservas de Capital **não absorvem** prejuízo ordinariamente, apenas quando as anteriores se esgotam.

---
## Lançamentos contábeis

**Absorção com Reserva de Lucros:**
```
D – Reserva de Lucro (ex.: Reserva de Contingências)
C – Prejuízos Acumulados
```

**Absorção com Reserva Legal:**
```
D – Reserva Legal
C – Prejuízos Acumulados
```

**Absorção com Reserva de Capital:**
```
D – Reserva de Capital
C – Prejuízos Acumulados
```

---
## Como fica na DMPL

Cada absorção aparece como uma **linha separada** na DMPL:

| Evento | Luc/Prej Acum. | Res. de Lucros | Reserva Legal | Res. de Capital | Total |
|---|---|---|---|---|---|
| Prejuízo do exercício | (−16.000) | — | — | — | (−16.000) |
| Absorção c/ Res. Contingências | +10.000 | (−10.000) | — | — | 0 |
| Absorção c/ Reserva Legal | +5.000 | — | (−5.000) | — | 0 |
| Absorção c/ Reserva de Capital | +1.000 | — | — | (−1.000) | 0 |
| **Saldo final** | **0** | **0** | **0** | **+1.000** | **101.000** |

> [!tip] Se o prejuízo for maior do que todas as reservas disponíveis, o saldo devedor permanece em **Prejuízos Acumulados** no BP.

---
## Exemplo numérico

**Dados em 31/12/20X2:**
- Capital Social: R$ 100.000
- Reserva Legal: R$ 5.000
- Reserva de Capital: R$ 2.000
- Reserva para Contingências: R$ 10.000
- Prejuízo do exercício: R$ 16.000

**Absorção:**
1. Lucros Acumulados anteriores: R$ 0 (conta zerada)
2. Reserva para Contingências: R$ 10.000 → absorve R$ 10.000 (saldo → R$ 0)
3. Reserva Legal: R$ 5.000 → absorve R$ 5.000 (saldo → R$ 0)
4. Reserva de Capital: R$ 2.000 → absorve R$ 1.000 (saldo → R$ 1.000)

**PL final:** Capital R$ 100.000 + Reserva de Capital R$ 1.000 = **R$ 101.000**

---
## Pontos de prova

- A **Reserva Legal** só pode ser utilizada para absorção de prejuízo após **esgotadas as demais Reservas de Lucros**.
- As **Reservas de Capital** são utilizadas apenas para absorção de prejuízo que ==não possa ser coberto pelas Reservas de Lucros== (art. 200, Lei nº 6.404/76).
- A conta **Lucros Acumulados** deve encerrar zerada ou com saldo devedor — nunca credor.
- Se o prejuízo exceder todas as reservas disponíveis, a diferença fica como saldo em **Prejuízos Acumulados** no Balanço Patrimonial.

---
## Tópicos Relacionados

- [[Demonstração das Mutações do Patrimônio Líquido (DMPL)]]
- [[Elaboração da DMPL — Passo a Passo]]
- [[Reservas de Lucros]]
- [[Reservas de Capital]]
- [[Reserva Legal]]
- [[Prejuízos Acumulados]]
- [[MOC — Demonstração das Mutações do Patrimônio Líquido (DMPL)]]

## Situações Líquidas

### Superavitária

> [!note] Patrimônio Líquido > 0 (positivo)

- **Ativo >  Passivo Exigível**
- Positiva
- Confortável
- Favorável
### Nula

> [!note] Patrimônio Líquido = 0

- **Ativo = Passivo**
- Compensada
- Neutra
- Igualitária
### Passivo à Descoberto

> [!note] Patrimônio Líquido < 0 (negativo) 

- **Ativo <  Passivo**
- Negativa
- Desconfortável
- Desfavorável
- Deficitária
- Passiva

### Constituição da Sociedade

> [!note] Ativo = Patrimônio Líquido

- Passivo Exigível = 0