---
tipo: regra
id: RN-GER-002
titulo: Os dias de atraso contam a partir do vencimento da parcela em aberto mais
area: geral
status: confirmada
evidencias:
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java
  linhas: 82-89
  hash: 236820158df43affe581f7e18e1f294076ffe8866231ba0ff901ad73980440c5
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
origem: analises/A-0001.md
---

# RN-GER-002 · Os dias de atraso contam a partir do vencimento da parcela em aberto mais

- **Identificador:** RN-GER-002
- **Área:** geral
- **Status:** confirmada
- **Origem:** [analises/A-0001.md](../analises/A-0001.md)

## Enunciado

Os dias de atraso contam a partir do vencimento da parcela em aberto mais antiga (não de cada parcela). Em cronogramas "fato" conta-se o número real de dias; nos demais usa-se o calendário comercial 30/360.[^1]

## Evidências

[^1]: `server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java:82-89` · hash `236820158df43affe581f7e18e1f294076ffe8866231ba0ff901ad73980440c5` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
