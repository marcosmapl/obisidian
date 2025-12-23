---
disciplina: Estatística
tópico: MOC Principal
tags:
  - estatistica
  - moc
created: 2025-03-22T16:49:00
updated: 2025-12-23T00:00:00
progresso: 0
node_size: "80"
---

> [!abstract] Sobre esta disciplina
> **Estatística** é a ciência que coleta, organiza, descreve, analisa e interpreta dados numéricos, fornecendo ferramentas para a **tomada de decisões** em condições de incerteza através de métodos científicos.

---
## 📌 Índice de Tópicos (MOCs)

### 01 — [[Concursos/Estatística/01 - Conceitos Fundamentais/MOC — Conceitos Fundamentais|MOC — Conceitos Fundamentais]]
População, amostra, tipos de variáveis e dados estatísticos.

### 02 — [[Concursos/Estatística/02 - Estatística Descritiva/MOC — Estatística Descritiva|MOC — Estatística Descritiva]]
Tabelas, gráficos, medidas de posição, variabilidade e forma.

### 03 — [[Concursos/Estatística/03 - Probabilidade/MOC — Probabilidade|MOC — Probabilidade]]
Espaço amostral, eventos, probabilidade condicional e teorema de Bayes.

### 04 — [[Concursos/Estatística/04 - Variáveis Aleatórias/MOC — Variáveis Aleatórias|MOC — Variáveis Aleatórias]]
Variáveis discretas e contínuas, esperança, variância e covariância.

### 05 — [[Concursos/Estatística/05 - Distribuições de Probabilidade/MOC — Distribuições de Probabilidade|MOC — Distribuições de Probabilidade]]
Distribuições discretas (Binomial, Poisson) e contínuas (Normal, t, χ², F).

### 06 — [[Concursos/Estatística/06 - Amostragem/MOC — Amostragem|MOC — Amostragem]]
Técnicas de amostragem, distribuição amostral e teorema central do limite.

### 07 — [[Concursos/Estatística/07 - Inferência Estatística/MOC — Inferência Estatística|MOC — Inferência Estatística]]
Estimação de parâmetros, intervalos de confiança e testes de hipóteses.

### 08 — [[Concursos/Estatística/08 - Números-Índices/MOC — Números-Índices|MOC — Números-Índices]]
Índices de Laspeyres, Paasche, Fisher e deflacionamento de séries.

### 09 — [[Concursos/Estatística/09 - Correlação/MOC — Correlação|MOC — Correlação]]
Coeficiente de correlação de Pearson e interpretação de associações.

### 10 — [[Concursos/Estatística/10 - Regressão/MOC — Regressão|MOC — Regressão]]
Regressão linear simples, mínimos quadrados e coeficiente de determinação.

---
## 📚 Recursos Adicionais

### 🔗 Links Úteis
- [[Caderno de Erros — Estatística]]
- [[Questões Comentadas — Estatística]]
- [[Fórmulas Estatísticas]]
- [[Tabelas Estatísticas (Z, t, χ², F)]]

### 🏷️ Tags Principais
#estatistica #estatistica/descritiva #estatistica/probabilidade #estatistica/inferencia #estatistica/regressao

---
## 📊 Progresso de Estudos

```dataview
TABLE WITHOUT ID
  file.name as "Tópico",
  progresso as "Progresso %"
FROM "Concursos/Estatística"
WHERE contains(file.name, "MOC")
SORT file.name
```

---
## 🔑 Conceitos e Fórmulas Essenciais

### Medidas de Posição
**Média Aritmética:**
$$\bar{x} = \frac{\sum x_i}{n}$$

**Mediana:** valor central ordenado

**Moda:** valor mais frequente

### Medidas de Dispersão
**Variância:**
$$s^2 = \frac{\sum(x_i - \bar{x})^2}{n-1}$$

**Desvio-Padrão:**
$$s = \sqrt{s^2}$$

**Coeficiente de Variação:**
$$CV = \frac{s}{\bar{x}} \times 100\%$$

### Probabilidade
**Probabilidade Condicional:**
$$P(A|B) = \frac{P(A \cap B)}{P(B)}$$

**Teorema de Bayes:**
$$P(A|B) = \frac{P(B|A) \cdot P(A)}{P(B)}$$

### Distribuições
**Binomial:** $P(X=k) = \binom{n}{k} p^k (1-p)^{n-k}$

**Normal:** $Z = \frac{X - \mu}{\sigma}$

### Inferência
**IC para Média:** $\bar{x} \pm t_{\alpha/2} \cdot \frac{s}{\sqrt{n}}$

**Correlação:** $r = \frac{Cov(X,Y)}{s_X \cdot s_Y}$

**Regressão:** $\hat{Y} = b_0 + b_1 X$, onde $R^2 = r^2$

---
## 📖 Divisões da Estatística

```
Estatística
    ├── Estatística Descritiva
    │   ├── Organização de dados
    │   ├── Apresentação de dados
    │   └── Medidas resumo
    │
    ├── Probabilidade
    │   ├── Teoria dos conjuntos
    │   ├── Eventos aleatórios
    │   └── Cálculo de probabilidades
    │
    └── Inferência Estatística
        ├── Estimação
        ├── Testes de hipóteses
        └── Análise de associação
```

