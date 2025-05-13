# SECURITY PRINCIPLES - [TryHackMe](https://tryhackme.com/room/securityprinciples)

🗓️ Data: 13-05-2025  
🔗 Link: https://tryhackme.com/room/securityprinciples

---

## 🧠 O que aprendi

### CIA

- **Tríade de Segurança**:
  - **Confidencialidade**: apenas as pessoas certas tenham acesso aos dados;
  - **Integridade**: garante que a informação não seja alterada e detecta se sofreu alguma alteração;
  - **Disponibilidade**: garante que o sistema ou serviço esteja disponível quando preciso.

---

### Fundamental Concepts of Security Models

- **Bell-LaPadula Model**: Confidencialidade – _write up, read down_
- **Biba Model**: Integridade – _no write up, no read down_
- **Clark-Wilson Model**:
  - **CDI**: dados cuja integridade queremos proteger
  - **UDI**: dados como entradas de usuário e informações gerais
  - **TPs**: operações (como leitura/escrita) que mantêm a integridade dos CDIs
  - **IVPs**: verificam e garantem a validade dos CDIs

---

### Defence-in-depth

Refere-se a um sistema de segurança com múltiplos níveis, também chamado de _Multi-Level Security_.

---

### ISO/IEC 19249

#### 🧱 5 Princípios de Arquitetura

- **Domain Separation**: componentes relacionados são agrupados como uma única entidade.
- **Layering**: estruturação em camadas permite impor políticas de segurança em diferentes níveis.
- **Encapsulation**: certas informações são ocultadas para evitar manipulação direta.
- **Redundancy**: garante disponibilidade e integridade (ex: RAID 5 com 3 discos, um pode falhar).
- **Virtualization**: compartilhamento de hardware entre múltiplos sistemas operacionais. Oferece sandboxing e monitoramento contra ameaças.

#### 🧩 5 Princípios de Design

- **Least Privilege**: acesso mínimo necessário — _need-to-know basis_.
- **Attack Surface Minimisation**: reduzir ao máximo as vulnerabilidades do sistema.
- **Centralized Parameter Validation**: inputs inválidos podem ser vetores de ataque; validar é essencial.
- **Centralized General Security Services**: serviços como autenticação devem ser centralizados, com cuidado para não gerar ponto único de falha.
- **Preparing for Error and Exception Handling**: o sistema deve estar preparado para lidar com falhas inevitáveis.

---

### Zero Trust vs Trust but Verify

- **Trust but Verify**: mesmo confiando, é necessário verificar constantemente.
- **Zero Trust**: trata a confiança como uma vulnerabilidade.
  - _"Never Trust, Always Verify"_

---

### Threat vs Risk

- **Vulnerability**: estado de suscetibilidade a ataques ou danos.
- **Threat**: ameaça — perigo potencial associado a uma vulnerabilidade.
- **Risk**: risco — probabilidade de uma ameaça explorar uma vulnerabilidade e causar impacto nos negócios.
