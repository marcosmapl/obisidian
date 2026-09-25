

## 1. Algoritmos Simétricos

> **Mesma chave para cifrar e decifrar.**  
> Geralmente são **muito mais rápidos** que os algoritmos assimétricos e são utilizados para criptografia de grandes volumes de dados.

### AES — Advanced Encryption Standard

- **Tipo:** cifra de bloco
- **Chaves:** 128, 192 ou 256 bits
- **Bloco:** 128 bits
- **Velocidade:** ⚡ rápida
- **Segurança:** 🔒 alta
- **Uso:** criptografia de dados, arquivos, discos, VPN, TLS etc.
- **Destaque:** principal padrão moderno de criptografia simétrica.
- **Prova:** AES = **simétrico + bloco + 128/192/256 bits**.

### ChaCha20

- **Tipo:** cifra de fluxo (_stream cipher_)
- **Chave:** 256 bits
- **Velocidade:** ⚡ muito rápida, especialmente em software e dispositivos sem aceleração AES
- **Segurança:** 🔒 alta
- **Uso:** TLS/Internet e dispositivos móveis
- **Destaque:** frequentemente utilizado em conjunto com **Poly1305** → ChaCha20-Poly1305 (AEAD).
- **Prova:** ChaCha20 = **simétrico + fluxo + 256 bits**.

### 3DES / Triple DES / TDEA

- **Tipo:** cifra de bloco
- **Base:** DES aplicado em múltiplas etapas
- **Chaves:** tradicionalmente associado a 112 ou 168 bits nominais, dependendo da variante
- **Bloco:** 64 bits
- **Velocidade:** 🐌 lenta
- **Segurança:** ⚠️ legado; não recomendado para novos sistemas
- **Uso:** sistemas antigos
- **Prova:** 3DES = **DES triplo + bloco + legado + lento**.

### DES — Data Encryption Standard

- **Tipo:** cifra de bloco
- **Chave efetiva:** **56 bits**
- **Bloco:** 64 bits
- **Velocidade:** relativamente rápida para sua época, mas obsoleta atualmente
- **Segurança:** ❌ insuficiente contra força bruta moderna
- **Substituído por:** AES
- **Prova:** DES = **56 bits → inseguro/obsoleto**.

### Blowfish

- **Tipo:** cifra de bloco
- **Chave:** variável, **32 a 448 bits**
- **Bloco:** 64 bits
- **Velocidade:** ⚡ rápida em software
- **Segurança:** historicamente considerada boa, mas atualmente é uma opção legada
- **Uso:** sistemas antigos e aplicações específicas
- **Prova:** Blowfish = **bloco + chave variável + 32–448 bits**.

### Twofish

- **Tipo:** cifra de bloco
- **Chaves:** 128, 192 ou 256 bits
- **Bloco:** 128 bits
- **Velocidade:** rápida
- **Segurança:** 🔒 considerada forte
- **Destaque:** foi um dos **5 finalistas** da competição AES, mas o vencedor foi o Rijndael (AES).
- **Prova:** Twofish = **finalista do AES + bloco + 128/192/256 bits**.

### IDEA — International Data Encryption Algorithm

- **Tipo:** cifra de bloco
- **Chave:** 128 bits
- **Bloco:** 64 bits
- **Velocidade:** rápida
- **Segurança:** historicamente considerada forte, mas atualmente é menos utilizada que AES
- **Uso:** sistemas/protocolos legados, historicamente associado ao PGP
- **Prova:** IDEA = **bloco + chave de 128 bits**.

---
## 2. Algoritmos Assimétricos

> **Utilizam um par de chaves:**  
> 🔑 **pública** + 🔐 **privada**.
> 
> São mais lentos que algoritmos simétricos e são utilizados principalmente para **assinaturas digitais, autenticação, troca/acordo de chaves e criptografia de pequenas quantidades de dados**.

### RSA — Rivest-Shamir-Adleman

- **Tipo:** criptografia assimétrica / assinatura digital
- **Base matemática:** fatoração de números inteiros
- **Chaves:** tradicionalmente 2048 bits ou mais em aplicações modernas
- **Velocidade:** 🐌 mais lento que algoritmos simétricos
- **Segurança:** alta quando utilizado com parâmetros e esquemas adequados
- **Uso:** certificados digitais, assinaturas e criptografia de chaves
- **Prova:** RSA = **assimétrico + fatoração + assinatura/certificados**.

### ECDSA — Elliptic Curve Digital Signature Algorithm

- **Tipo:** algoritmo de assinatura digital assimétrica
- **Base matemática:** curvas elípticas / problema do logaritmo discreto
- **Chaves:** menores que RSA para nível de segurança comparável
- **Velocidade:** eficiente
- **Segurança:** alta quando utilizado com parâmetros seguros
- **Uso:** assinaturas digitais, certificados e sistemas de autenticação
- **Prova:** ECDSA = **assinatura + curva elíptica**.

### Diffie-Hellman (DH)

- **Tipo:** acordo/troca de chaves
- **Base matemática:** logaritmo discreto
- **Chaves:** depende dos parâmetros utilizados
- **Velocidade:** mais lento que criptografia simétrica
- **Função principal:** **estabelecer uma chave compartilhada**
- **Importante:** DH **não é, por si só, um algoritmo de criptografia de dados nem de assinatura digital**.
- **Prova:** DH = **acordo de chave**.

### ECDH — Elliptic Curve Diffie-Hellman

- **Tipo:** acordo de chaves assimétrico
- **Base matemática:** curvas elípticas
- **Chaves:** menores que DH tradicional para nível de segurança comparável
- **Velocidade:** eficiente
- **Função:** estabelecimento de chave compartilhada
- **Prova:** ECDH = **DH + curvas elípticas**.

### DSA — Digital Signature Algorithm

- **Tipo:** assinatura digital
- **Base matemática:** logaritmo discreto
- **Função:** gerar e verificar assinaturas digitais
- **Não serve:** como algoritmo de criptografia de dados
- **Status:** legado; em padrões atuais do NIST, DSA ficou restrito à **verificação de assinaturas existentes**.
- **Prova:** DSA = **assinatura digital + logaritmo discreto**.

### ElGamal

- **Tipo:** criptografia assimétrica / assinatura em construções relacionadas
- **Base matemática:** logaritmo discreto
- **Chaves:** geralmente maiores que as de sistemas de curvas elípticas para segurança equivalente
- **Velocidade:** mais lento que algoritmos simétricos
- **Função:** criptografia e construção de esquemas de assinatura
- **Prova:** ElGamal = **assimétrico + logaritmo discreto**.

---
## 📊 Tabela-resumo

|Algoritmo|Tipo|Chave|Velocidade|Segurança/Status|Principal finalidade|
|---|---|--:|---|---|---|
|**AES**|Simétrico / Bloco|128/192/256|⚡ Rápida|🔒 Alta|Criptografia de dados|
|**ChaCha20**|Simétrico / Fluxo|256|⚡ Muito rápida|🔒 Alta|Criptografia de dados|
|**3DES**|Simétrico / Bloco|112/168*|🐌 Lenta|⚠️ Legado|Sistemas antigos|
|**DES**|Simétrico / Bloco|56|🐌 Obsoleto|❌ Fraca|Sistemas legados|
|**Blowfish**|Simétrico / Bloco|32–448|⚡ Rápida|⚠️ Legado|Criptografia de dados|
|**Twofish**|Simétrico / Bloco|128/192/256|⚡ Rápida|🔒 Forte|Criptografia de dados|
|**IDEA**|Simétrico / Bloco|128|⚡ Rápida|⚠️ Legado|Criptografia de dados|
|**RSA**|Assimétrico|≥2048 comum|🐌 Lenta|🔒 Alta|Assinatura/certificados|
|**ECDSA**|Assimétrico / Assinatura|Variável|⚡ Eficiente|🔒 Alta|Assinatura digital|
|**DH**|Assimétrico / Acordo|Variável|🐌 Lenta|🔒 Alta*|Troca/acordo de chave|
|**ECDH**|Assimétrico / Acordo|Variável|⚡ Eficiente|🔒 Alta*|Troca/acordo de chave|
|**DSA**|Assimétrico / Assinatura|Variável|🐌 Lenta|⚠️ Legado|Assinatura digital|
|**ElGamal**|Assimétrico|Variável|🐌 Lenta|🔒 Forte*|Criptografia/assinatura|


## ⚠️ Pegadinhas clássicas

1. **AES não é assimétrico** → é **simétrico**.
    
2. **RSA não é simétrico** → é **assimétrico**.
    
3. **DH não cifra diretamente os dados** → seu objetivo principal é **estabelecer uma chave compartilhada**.
    
4. **ECDH não é assinatura digital** → é **acordo de chaves**.
    
5. **ECDSA é assinatura digital** → não é usado para criptografar grandes volumes de dados.
    
6. **DSA ≠ DAS** → o correto é **DSA (Digital Signature Algorithm)**.
    
7. **DES possui chave efetiva de 56 bits**, apesar de operar com blocos de 64 bits.
    
8. **AES possui bloco de 128 bits**, independentemente de a chave ser 128, 192 ou 256 bits.
    
9. **Twofish foi finalista do AES**, mas não foi o vencedor.
    
10. **Criptografia simétrica é muito mais rápida** que a assimétrica e é a escolha típica para proteger grandes volumes de dados.
    
11. **Chave maior não significa automaticamente algoritmo melhor**: é preciso considerar o algoritmo e o nível de segurança proporcionado.
    
12. **Criptografia ≠ hash**: SHA-256, SHA-3 etc. são funções hash, não algoritmos de criptografia.


![[Pasted image 20260924223729.jpg]]

---
## Processo de criptografia

### Chaves do destinatário

- Garantir a **integridade** e **confidencialidade**
- **Chave pública** do destinatário é usada para **cifrar**
- **Chave privada** do destinatário é usada para **decifrar**
- Como somente o proprietário da chave privada tem acesso a mesma. Ao criptografar uma mensagem com a chave pública do destinatário, sabemos que somente ele terá acesso ao conteúdo da mensagem.

### Chaves do emissor

- Garantir a **autenticidade** do emissor
- **Chave privada** do emissor é usada para **cifrar** (encriptar)
- **Chave pública** do emissor é usada para **decifrar** (desencriptar). 
- Assim, qualquer pessoa que tenha a chave pública do emissor pode conferir a autenticidade do emissor.