
## Conceito

📌 **Ajuste a Valor Presente (AVP)** → é a quantia que representa **hoje** um **fluxo de caixa futuro**, descontado por uma taxa que reflete o valor do dinheiro no tempo e os riscos da operação, ou seja:

> É o valor de um fluxo de caixa futuro, descontados eventuais juros embutidos na operação.

---
## Obrigatoriedade

- **Ativo ou Passivo de Longo Prazo**: (acima de 12 meses).
- **Ativo ou Passivo de Curto Prazo**: taxa de juros for relevante.

---
## Mensuração

**Diretrizes Gerais**

**Ativos e Passivos Não Monetários** adquiridos a prazo **com juros implícitos ou explícitos embutidos** devem ser mensurados pelo seu valor presente quando do seu reconhecimento inicial.

- **Uma vez ajustado,** o item não monetário **não deve mais ser submetido a ajustes** subsequentes no que respeita à figura de **juros embutidos.**
- ⚠️ **Nem todo** ativo ou passivo não monetário **está sujeito** ao efeito do ajuste a valor presente.

**Não devem** ser Ajustados a Valor Presente:

- Adiantamento em Dinheiro para recebimento ou pagamento em bens e serviços.
- Imposto de Renda Diferido (Ativo ou Passivo).
- Financiamentos do BNDES, contratados com taxa de juros diferentes das taxas praticadas pelo mercado em geral.
- Contrato de mútuo que não possui data definida de vencimento.

**Diretrizes mais Específicas**

- AVP deve ser calculado no **momento inicial** da operação
    - Adoção do método de **taxa efetiva de juros** no registro inicial da operação

---
## Lançamento

### Venda com Juros

**No momento da venda**

```
D - Clientes (AC) ...................... Valor Total Futuro
C - AVP Clientes (Ret. AC) ............. Valor dos Juros a Receber
C - Receita Bruta (R) .................. Valor Presente (Receita Efetiva)
```

**Mensalmente**, devem-se reconhecer as receitas com juros correspondentes:

```
D - AVP Clientes (Ret. AC) ............. Valor dos Juros no Período
C - Juros Ativos (R) ................... Valor dos Juros no Período
```

### Compra com Juros

**No momento da compra**

```
C - Fornecedores (PC) ................. Valor Total Futuro (compra)
D - AVP Fornecedores (Ret. PC) ........ Valor dos Juros a Pagar
D - Despesa ........................... Valor Presente (Despesa Efetiva)
```

**Mensalmente**, devem-se reconhecer as despesas com juros correspondentes:

```
D - Juros Passivos (D) ................ Valor dos Juros no Período
C - AVP Fornecedores (Ret. PC) ........ Valor dos Juros no Período 
```

--- 
## Cálculo do Valor Presente

$$ VP = \frac{VF}{(1 + i)^n} $$

Onde:
- **VP**: valor presente
- **VF**: valor futuro
- **i**: taxa de desconto
- **n**: número de períodos