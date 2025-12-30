
As cláusulas **ON DELETE** e **ON UPDATE** definem as **ações referenciais** aplicadas pelo SGBD quando ocorre a **exclusão** ou a **alteração** de um valor da **chave primária (ou única)** na tabela **referenciada** por uma **FOREIGN KEY**.

Essas opções são parte do **SQL ANSI** e são frequentemente cobradas em concursos públicos.

---
## **[[CASCADE]]**

- **ON DELETE CASCADE**: ao excluir um registro da tabela pai, os registros correspondentes na tabela filha são **automaticamente excluídos**.
    
- **ON UPDATE CASCADE**: ao atualizar o valor da chave referenciada, os valores correspondentes na tabela filha são **automaticamente atualizados**.
    

**Uso típico:** forte dependência entre os registros.

---
## **[[RESTRICT]]**

- Impede a exclusão ou atualização do registro na tabela pai **enquanto existirem registros relacionados** na tabela filha.
    
- A operação é **bloqueada** e ocorre erro.
    

**Observação:** em alguns SGBDs, `RESTRICT` é equivalente a `NO ACTION`.

---
## **[[NO ACTION]]**

- A exclusão ou atualização é **rejeitada** se houver registros relacionados.
    
- A verificação ocorre **ao final da instrução** (ou da transação, conforme o SGBD).
    

**Diferença teórica:** `NO ACTION` adia a verificação; `RESTRICT` pode impedir imediatamente.

---
## **[[SET NULL]]**

- **ON DELETE SET NULL**: ao excluir o registro da tabela pai, a FOREIGN KEY na tabela filha é definida como **NULL**.
    
- **ON UPDATE SET NULL**: ao alterar o valor da chave referenciada, a FOREIGN KEY passa a **NULL**.
    

**Requisito:** a coluna da FOREIGN KEY deve **permitir NULL**.

---
## **[[SET DEFAULT]]**

- **ON DELETE SET DEFAULT**: ao excluir o registro da tabela pai, a FOREIGN KEY assume seu **valor padrão**.
    
- **ON UPDATE SET DEFAULT**: ao alterar o valor da chave referenciada, a FOREIGN KEY assume o **DEFAULT** definido.
    

**Requisito:** a coluna deve possuir um valor **DEFAULT** válido.

---
## Resumo Comparativo

| Opção       | Efeito principal                      |
| ----------- | ------------------------------------- |
| CASCADE     | Propaga a ação para a tabela filha    |
| RESTRICT    | Bloqueia a ação se houver dependentes |
| NO ACTION   | Rejeita a ação após verificação       |
| SET NULL    | Remove o vínculo (define NULL)        |
| SET DEFAULT | Define valor padrão                   |

---
## Resumo para concurso

> **ON DELETE / ON UPDATE** controlam o comportamento do SGBD frente à **manutenção da integridade referencial**, sendo essenciais para compreender o impacto das operações de exclusão e atualização em tabelas relacionadas.