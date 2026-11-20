---
tipo: regra
id: RN-GER-007
titulo: 'Carência: enquanto os dias de atraso (contados dentro da faixa) são menores que'
area: geral
status: confirmada
evidencias:
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java
  linhas: 130-140
  hash: 7e71ff0bab8d85037951660a5de7fc35c311443ce059eb5fa91f4d7063b697b1
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java
  linhas: 154-156
  hash: ee5aa90ebbc26b5b40fc268fa35ecd2a007aebaffa9deb74e276b097c4327009
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
origem: analises/A-0001.md
---

# RN-GER-007 · Carência: enquanto os dias de atraso (contados dentro da faixa) são menores que

- **Identificador:** RN-GER-007
- **Área:** geral
- **Status:** confirmada
- **Origem:** [analises/A-0001.md](../analises/A-0001.md)

## Enunciado

Carência: enquanto os dias de atraso (contados dentro da faixa) são menores que a carência, não há multa. Sem carência, a multa de cada dia é o valor diário corrigido pelo que já foi lançado (valor diário × dias de atraso − multas já lançadas). Com carência, quando ainda não houve lançamento, o primeiro lançamento é de uma vez só: valor diário × dias de carência.[^1][^2]

## Evidências

[^1]: `server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java:130-140` · hash `7e71ff0bab8d85037951660a5de7fc35c311443ce059eb5fa91f4d7063b697b1` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
[^2]: `server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java:154-156` · hash `ee5aa90ebbc26b5b40fc268fa35ecd2a007aebaffa9deb74e276b097c4327009` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
