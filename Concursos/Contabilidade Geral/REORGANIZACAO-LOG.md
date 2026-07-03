Reorganização e padronização — Contabilidade Geral

Data: 2026-07-02

Ações realizadas:

- Padronizei nomes de MOC em alguns tópicos substituindo '—' por ' - ':
  - `01 - Conceitos Fundamentais/MOC - Conceitos Fundamentais.md` (criado a partir do arquivo existente)
  - `02 - Contas Contábeis/MOC - Contas Contábeis.md` (criado)
- Atualizei `Contabilidade Geral.md` para apontar para os novos nomes padronizados.
- Removi `Patrimônio— Conceito.md.bak` (arquivo backup placeholder).
- Criei `Concursos/SUMÁRIO-Resumo-Disciplinas.md` com índice básico das disciplinas.

Recomendações pendentes:

1. Fazer bulk-rename de outros arquivos `MOC — *.md` no workspace para `MOC - *.md` (há muitos, especialmente em `Tecnologia da Informação` e `Direito`).
2. Adicionar frontmatter YAML padronizado (disciplina/tópico/created/updated) em todas as notas; atualmente algumas já têm, outras não.
3. Mover backups reais para `Concursos/backups/` em vez de deixar no mesmo diretório.
4. Validar todos os links dentro dos MOCs após renomeação — alguns links podem apontar para os nomes antigos.

Sugestão de padrão de frontmatter:

---
disciplina: <Nome da Disciplina>
tópico: <Tópico ou MOC>
created: YYYY-MM-DDTHH:MM:SS
updated: YYYY-MM-DDTHH:MM:SS
---


