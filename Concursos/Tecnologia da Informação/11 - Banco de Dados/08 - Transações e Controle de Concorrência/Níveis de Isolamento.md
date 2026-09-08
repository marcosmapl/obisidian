
**Os 4 níveis de isolamento são Read Uncommited, Read Commited, Repeatable Read e Serializable. Veja uma descrição de cada um deles:

- **Read Uncommitted:** Permite a máxima concorrência entre transações. Neste nível, todas as três anomalias (Dirty Reads, Non-repeatable Reads e Phantom Reads) são possíveis. Usado apenas em contextos onde integridade não é primordial.
- **Read Committed:** Evita o problema de Dirty Reads, garantindo que uma transação apenas leia dados confirmados. Todavia, ainda é possível observar alterações realizadas por outras transações já confirmadas durante sua execução, permitindo Non-repeatable Reads e Phantom Reads. É o nível padrão em diversos sistemas como PostgreSQL, Oracle e SQL Server.
- **Repeatable Read:** Elimina Dirty Reads e Non-repeatable Reads, garantindo que, se um dado for lido múltiplas vezes dentro da mesma transação, os valores retornados sejam sempre iguais. No entanto, ainda permite o Phantom Read, possibilitando que novos registros possam ser incluídos ou removidos por outras transações. É o nível padrão no MySQL.
- **Serializable:** É o nível mais restritivo, eliminando todas as três anomalias. Funciona executando as transações como se fossem sequenciais, mesmo que ocorram simultaneamente, utilizando técnicas de bloqueio rigorosas ou controle por multiversionamento. Oferece segurança máxima, porém a um custo significativo em termos de desempenho e concorrência.

|Nível de Isolamento|Leitura Suja|Leitura Não-Repetível|Fantasma|
|---|---|---|---|
|**Read Uncommitted**|✅ Permite|✅ Permite|✅ Permite|
|**Read Committed**|❌ Não permite|✅ Permite|✅ Permite|
|**Repeatable Read**|❌ Não permite|❌ Não permite|✅ Permite|
|**Serializable**|❌ Não permite|❌ Não permite|❌ Não permite|