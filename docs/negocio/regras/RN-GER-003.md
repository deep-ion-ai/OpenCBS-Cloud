---
tipo: regra
id: RN-GER-003
titulo: Cada penalidade só vale dentro da sua faixa de dias de atraso (dia inicial e
area: geral
status: confirmada
evidencias:
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java
  linhas: 93-96
  hash: e15e8004fe453948c5aed696f76ba2e591aa192c4d089d2389a52d1b72a65ff8
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
origem: analises/A-0001.md
---

# RN-GER-003 · Cada penalidade só vale dentro da sua faixa de dias de atraso (dia inicial e

- **Identificador:** RN-GER-003
- **Área:** geral
- **Status:** confirmada
- **Origem:** [analises/A-0001.md](../analises/A-0001.md)

## Enunciado

Cada penalidade só vale dentro da sua faixa de dias de atraso (dia inicial e dia final). Fora da faixa, ela não gera multa naquele dia.[^1]

## Evidências

[^1]: `server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java:93-96` · hash `e15e8004fe453948c5aed696f76ba2e591aa192c4d089d2389a52d1b72a65ff8` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
