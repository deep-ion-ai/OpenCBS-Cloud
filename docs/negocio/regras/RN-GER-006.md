---
tipo: regra
id: RN-GER-006
titulo: 'Base por tipo: o valor fixo é o próprio valor cadastrado, sem divisão por dia'
area: geral
status: confirmada
evidencias:
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/FlatPenalty.java
  linhas: 22-23
  hash: 5ebcaf3328e73cb1580bb2ea9a6c619057650679abad918f51d42c69442a3c7e
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/LatePrincipalPenalty.java
  linhas: 24-25
  hash: 5338c543b024484aa6fb6cc17336ad9675a051064bdf526cce6a79fb6bb4110c
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/LateInterestPenalty.java
  linhas: 24-25
  hash: 55f711c849133bd9217f6c3c20b5b8cb6bbec2b08c9e22a670fad6f357dcbad9
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/DisbursementAmountPenalty.java
  linhas: 30-31
  hash: 7017c4758086ce57b1e2c36b7717d3a14122971332968f2bc8047574a06ab0c3
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/OlbPenalty.java
  linhas: 25-26
  hash: d0ee4ee6e898ce2fa6b232e40080a29d41de06684885b886cf17efbb098542df
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
origem: analises/A-0001.md
---

# RN-GER-006 · Base por tipo: o valor fixo é o próprio valor cadastrado, sem divisão por dia

- **Identificador:** RN-GER-006
- **Área:** geral
- **Status:** confirmada
- **Origem:** [analises/A-0001.md](../analises/A-0001.md)

## Enunciado

Base por tipo: o valor fixo é o próprio valor cadastrado, sem divisão por dia; por principal em atraso e por juros em atraso a base é a soma do principal (ou dos juros) devido em todas as parcelas vencidas e não pagas; por desembolso a base é o valor do empréstimo; por saldo devedor, o saldo do dia.[^1][^2][^3][^4][^5]

## Evidências

[^1]: `server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/FlatPenalty.java:22-23` · hash `5ebcaf3328e73cb1580bb2ea9a6c619057650679abad918f51d42c69442a3c7e` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
[^2]: `server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/LatePrincipalPenalty.java:24-25` · hash `5338c543b024484aa6fb6cc17336ad9675a051064bdf526cce6a79fb6bb4110c` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
[^3]: `server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/LateInterestPenalty.java:24-25` · hash `55f711c849133bd9217f6c3c20b5b8cb6bbec2b08c9e22a670fad6f357dcbad9` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
[^4]: `server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/DisbursementAmountPenalty.java:30-31` · hash `7017c4758086ce57b1e2c36b7717d3a14122971332968f2bc8047574a06ab0c3` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
[^5]: `server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/OlbPenalty.java:25-26` · hash `d0ee4ee6e898ce2fa6b232e40080a29d41de06684885b886cf17efbb098542df` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
