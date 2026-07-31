---
disciplina: Estatística
tópico: Conceitos Fundamentais
created: 2026-07-31T06:31:00
updated: 2026-07-31T06:31:00
---

Em estatística, as **classes** são as subdivisões ou intervalos nos quais um conjunto de dados, geralmente de uma **variável quantitativa contínua**, é agrupado para facilitar a análise. Esse agrupamento resulta em uma **distribuição de frequências intervalar**, que simplifica a visualização do comportamento global dos dados, embora ocorra uma perda de informação detalhada sobre os valores individuais.

---
## Tipos de Intervalos e Notações

Para identificar uma classe, é necessário conhecer seus limites e a natureza do intervalo (se é aberto ou fechado). O material destaca as seguintes notações:

| Tipo de Intervalo      | Notação Matemática | Notação Estatística | Significado                     |
| ---------------------- | ------------------ | ------------------- | ------------------------------- |
| **Aberto**             | a<x<b              | a↔b                 | Não inclui os extremos a e b.   |
| **Fechado à esquerda** | a≤x<b              | a⊢b                 | Inclui a, mas não inclui b.     |
| **Fechado à direita**  | a<x≤b              | a⊣b                 | Inclui b, mas não inclui a.     |
| **Fechado**            | a≤x≤b              | a⊣⊢b                | Inclui ambos os extremos a e b. |

---
## Parâmetros de uma Classe

### Limites de Classe

Cada classe possui um **limite inferior (**linf​**)**, que é o menor valor possível da classe, e um **limite superior (**lsup​**)**, que é o maior valor possível.

### Ponto Médio (PM)

Também chamado de **marca ou representante da classe**, é a média aritmética simples dos limites: PM=2linf​+lsup​​ Se a amplitude das classes for constante, os pontos médios formarão uma **progressão aritmética**.

### Amplitude do Intervalo de Classe (h)

É a distância entre os limites de uma classe: h=lsup​−linf​ Embora desejável, a amplitude não precisa ser obrigatoriamente constante em todas as classes de uma distribuição.

---
## Determinação do Número de Classes (k)

Existem duas formas principais de definir o número "ideal" de classes para um conjunto de n dados:

### Fórmula de Sturges 

$$ k = 1 + 3,3 \cdot logn $$

### Abordagem Simplificada(para n ≤ 50)

$$ k = n $$
​

---
## Amplitude Total (AT)

É a diferença entre o **limite superior da última classe (lmax​)** e o **limite inferior da primeira classe (lmin​)**: 

$$ AT = l_{max} ​− l_{min}​ $$

Se todas as classes tiverem a mesma amplitude (h), então 

$$ AT = h \cdot k $$

---
## Densidade de Frequência (di​)

Consiste no quociente entre a frequência da classe (absoluta ou relativa) e sua respectiva amplitude: di​=hi​fi​​ Este conceito é fundamental para a construção de **histogramas**, onde a altura das barras deve ser proporcional à frequência (ou densidade) do intervalo.

---
## Tópicos Relacionados

- [[Distribuição de Frequências]]
- [[Tipos de Frequência]]
- [[Representação Gráfica]]
- [[Dados Estatísticos]]