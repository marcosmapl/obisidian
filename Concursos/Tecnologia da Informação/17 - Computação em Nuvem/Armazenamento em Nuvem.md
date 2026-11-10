---
disciplina: Tecnologia da Informação
tópico: Computação em Nuvem
created: 2026-11-09T19:45:00
updated: 2026-11-09T19:45:00
---

> [!info] Definição
> **Armazenamento em Nuvem** (*Cloud Storage* / STaaS) é o modelo em que os dados são armazenados em infraestrutura remota do provedor, acessível via rede, com **escalabilidade, redundância e pagamento por uso**.

## Tipos de armazenamento

### Armazenamento de Objetos (*Object Storage*)

- Dados armazenados como **objetos** (dado + metadados + identificador único) em um espaço plano (*flat namespace*), sem hierarquia de diretórios.
- Acesso via **API HTTP/REST**.
- **Altamente escalável**; ideal para dados **não estruturados**: backups, mídias, logs, data lakes, conteúdo estático.
- **Exemplos**: Amazon S3 (buckets), Azure Blob Storage, Google Cloud Storage.

### Armazenamento de Blocos (*Block Storage*)

- Dados divididos em **blocos de tamanho fixo**, apresentados ao SO como **discos/volumes**.
- **Baixa latência e alto desempenho**; ideal para **bancos de dados** e discos de máquinas virtuais.
- Em geral, um volume é anexado a **uma única instância** por vez.
- **Exemplos**: Amazon EBS, Azure Managed Disks, Google Persistent Disk.

### Armazenamento de Arquivos (*File Storage*)

- Dados organizados em **hierarquia de diretórios e arquivos**, acessados via protocolos de rede (**NFS, SMB/CIFS**).
- Permite **compartilhamento simultâneo** entre múltiplas instâncias/usuários.
- **Exemplos**: Amazon EFS, Azure Files, Google Filestore.

## Comparativo

| Critério | Objetos | Blocos | Arquivos |
|---|---|---|---|
| Estrutura | Objetos + metadados (plano) | Blocos / volumes | Hierarquia de pastas |
| Acesso | API HTTP/REST | Como disco local (SO) | NFS / SMB |
| Desempenho | Moderado | **Alto (baixa latência)** | Moderado |
| Escalabilidade | **Virtualmente ilimitada** | Limitada ao volume | Limitada |
| Uso típico | Backup, mídia, data lake | Banco de dados, VM | Compartilhamento de arquivos |

## Classes de armazenamento (tiers)

- **Hot (acesso frequente)**: menor latência, maior custo de armazenamento.
- **Cool/Infrequent (acesso esporádico)**: custo menor de armazenamento, custo maior por acesso.
- **Archive / Cold (arquivamento)**: custo mínimo, recuperação lenta (minutos a horas). Ex.: Amazon S3 Glacier.

## Conceitos de prova

- **Durabilidade** ≠ **disponibilidade**: durabilidade é a probabilidade de **não perder** o dado (ex.: "11 noves" do S3); disponibilidade é a capacidade de **acessá-lo** quando necessário.
- **Redundância**: réplicas em múltiplos discos, zonas de disponibilidade ou regiões.
- **Consistência eventual** vs. **consistência forte** em sistemas distribuídos de armazenamento.
