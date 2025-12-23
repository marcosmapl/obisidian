---
disciplina: Tecnologia da Informação
tópico: SQL
created: 2025-12-20T09:11:00
---

A linguagem **SQL (ANSI)** define um conjunto de tipos de dados utilizados para armazenar e manipular informações em bancos de dados relacionais. Esses tipos são classificados conforme a natureza do dado.

---

## 📝 Tipos de Dados Textuais

Utilizados para armazenamento de caracteres e cadeias de texto.

- **CHAR(n)**  
    Texto de tamanho **fixo**.
    
- **VARCHAR(n)**  
    Texto de tamanho **variável**.
    
- **CLOB** (_Character Large Object_)  
    Grandes volumes de texto.
    

---

## 🔢 Tipos de Dados Numéricos

Utilizados para valores inteiros ou reais.

- **INTEGER / INT**  
    Número inteiro padrão.
    
- **SMALLINT**  
    Inteiro de menor faixa.
    
- **FLOAT**  
    Número real com precisão aproximada.
    
- **REAL**  
    Número real de precisão simples.
    
- **DOUBLE PRECISION**  
    Número real de maior precisão.
    

---

## 🧬 Tipos de Dados Binários

Armazenam dados em formato binário.

- **BIT(n)**  
    Sequência binária de tamanho fixo.
    
- **BIT VARYING(n)**  
    Sequência binária de tamanho variável.
    
- **BLOB** (_Binary Large Object_)  
    Grandes volumes de dados binários (imagens, arquivos, etc.).
    

---

## 🔘 Tipo de Dado Booleano

Utilizado para valores lógicos.

- **TRUE**
    
- **FALSE**
    
- **NULL** (ausência de valor)
    

---

## 📅 Tipos de Dados de Data

Representam datas do calendário.

- **DATE**  
    Possui **10 posições**, no formato **DD-MM-YYYY**  
    Exemplo: `30-03-2019`
    

### Funções associadas:

- **DAY()**
    
- **MONTH()**
    
- **YEAR()**
    

---

## ⏰ Tipos de Dados de Hora

Representam horários.

- **TIME**  
    Possui **8 posições**, no formato **HH:MM:SS**  
    Exemplo: `23:54:55`
    

### Funções associadas:

- **HOUR()**
    
- **MINUTE()**
    
- **SECOND()**
    

---

## ⏱️ Outros Tipos de Dados Temporais

Tipos avançados relacionados a data e hora.

- **TIMESTAMP**  
    Combina data e hora.
    
- **INTERVAL**  
    Representa intervalo de tempo.
    
- **DATETIME**  
    Data e hora em um único campo (dependente do SGBD).