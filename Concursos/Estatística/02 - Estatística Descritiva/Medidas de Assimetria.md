---
disciplina: Estatística
tópico: Estatística Descritiva
created: 2026-08-04T19:30:00
updated: 2026-08-04T19:32:00
---

> [!note] Assimetria
> **Grau de afastamento de uma distribuição** em relação ao **eixo de simetria**. 

---
## Distribuição Simétrica

Uma **distribuição é simétrica** quando possui um **único valor** para a **moda**, a **média** e a **mediana**.

$$ M_o = M_d = \bar{X} $$

![[Pasted image 20260804194730.png]]

---
## Distribuição Assimétrica

Uma **distribuição é assimétrica** quando ==não possui um único valor== para a **moda**, a **média** e a **mediana**.

### Distribuição Assimétrica à Esquerda (Negativa)

Dizemos que a **assimetria é negativa** quando os **valores mais baixos das observações são predominantes.**

![[Pasted image 20260804200917.png]]

$$ \bar{X} \lt M_d \lt M_o $$

> [!tip] Média à **esquerda**

### Distribuição Assimétrica à Direita (Positiva)

Dizemos que a **assimetria é positiva** quando os **valores mais altos das observações são predominantes**.

![[Pasted image 20260804201432.png]]

$$ M_o \lt M_d \lt \bar{X} $$

> [!tip] Média à **direita**

---
## Coeficiente de Assimetria

Os **coeficientes de assimetria** são usados para **quantificar o desvio de uma distribuição em relação a uma distribuição simétrica**.

### 1º Coeficiente de Pearson

$$ A_{M_o} = \frac{ \bar{X} - M_o }{ S } $$

- Distribuição **Simétrica**: AMo = 0
- Distribuição **Assimétrica Positiva** (Direita): AMo > 0
- Distribuição **Assimétrica Negativa** (Esquerda): AMo < 0
	- **Fraca**: 0 < | AMo | < 0,15
	- **Moderada**: 0,15 < | AMo | < 1
	- **Forte**: | AMo | > 1

### 2º Coeficiente de Pearson

$$ M_o = 3 \times M_d - 2 \times \bar{X} $$ 
$$ A_{M_d} = \frac{ 3 \times ( \bar{X} - M_d ) }{ S } $$


---
## Tópicos Relacionados

- [[Medidas de Curtose]]