# SECURITY PRINCIPLES - [TryhackMe](https://tryhackme.com/room/securityprinciples)

🗓️ Data: 13-05-2025  
🔗 Link: https://tryhackme.com/room/securityprinciples

---

## 🧠 O que aprendi

### CIA

- **Triade de Seguranca**: Confidencialidade, apenas as pessoas certas tenham acesso aos dados; Integridade, garante que a informacao nao seja alterada, e detectar se sofreu alguma alteracao; Disponibilidade, garante que o sistema ou servico esteja disponivel quando preciso.

### Fundamental Concepts of Security Models

- **Bell-LaPadula Model:** Confidencialidade, _write up, read down_
- **Biba Model:** Integridade, _no write up, no read down_
- **Clark-Wilson Model:** CDI, integradade dos dados que queremos proteger; UDI, outras informacoes como usuarios e entradas no sistema; TPs, operacoes como read/write que mantem a integridade dos CDIs; IVPs, revisam e garantem a validade dos CDIs.

### Defence-in-depth

Refere-se a um sistema de seguranca de miltiples niveles, também chamado de Multi-Level Security

### ISO/Iec 19249

**5 Principios de Arquitetura**

- **Domain Separation:** um conjutno de componentes relacionados são agrupados como uma única entidade.
- **Layering:** Quando um sistema é estruturado em várias camandas, torna-se possível impor poleiticas de seguranca em diferentes níveis.
- **Encapsulation:** Se escondem certas informacoes para previr uma manipulacao direta nos dados.
- **Redundancy:** Este principio garante a disponibilidade e integridade, exemplo de uma configuracao RAID 5 com 3 drives, se um falha, os outros continuam disponíveis.
- **Virtualization:** consiste no compartilhamento de um único conjunto de hardware entre vários sistemas operacionais. Oferece recursos como sandbox, e vigilancia de sistemas maliciosos.

**5 Principios de Design**

- **Least Privilage:** Reponde a pergunta, quem pode acceder isso?, "need-to-know basis.
- **Attack Surface Minimisation:** Todo sistema possui vulnerabilidades, e representam um risco, então é importante minimizar ao maximo as vulnerabilidades.
- **Centralized Paramenter Validation:** Inputs inválidos podem ser usadas para explorar vulnerabilidade no sistema. EPortanto, a validacao de paramentros é uma etapa necessaria.
- **Centralized General Security Services:**
  Centralizar servios de seguranca, como autenticacão, mas deve garantir a disponibilidade e evitar crear pontos de falha.
- **Preparing for Error and Exeption Handling** Devemos sempre considerar que errores e exepcoes vao sempre acontecer. Este principio diz, que o sistema tem que ser projetado para serem a prova de falhas.

### Zero Trust versus Trust but Verify

- **Trust but Verify:** devemos sempre verificar incluso quando confiamos na entidade e seu comportamento.
- **Zero Trust:** Esse princípio trata a confiança como uma vulnerabilidade e, consequentemente, atende a ameaças internas.
  _"Never Trust, Always Verify"_

### Threat versus Risk

- **Vulnerability:** Significa suscetível a ataques ou danos.
- **Threat:** ameaca é um perigo potencial associados a essa fraqueza ou vulnerabilidade.
- **Risk:** associados à probabilidade de um agente de ameaca explorar uma vulnerabilidade e impactar os negocios.

---
