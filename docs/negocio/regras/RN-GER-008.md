---
tipo: regra
id: RN-GER-008
titulo: Cada multa lançada vira um evento de "acúmulo de multa" no empréstimo e um
area: geral
status: confirmada
evidencias:
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java
  linhas: 178-189
  hash: 270deb7ca506392622abaac3f07a0ae351de3dd7fb9055e4774434b46062b336
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
origem: analises/A-0001.md
---

# RN-GER-008 · Cada multa lançada vira um evento de "acúmulo de multa" no empréstimo e um

- **Identificador:** RN-GER-008
- **Área:** geral
- **Status:** confirmada
- **Origem:** [analises/A-0001.md](../analises/A-0001.md)

## Enunciado

Cada multa lançada vira um evento de "acúmulo de multa" no empréstimo e um lançamento contábil: debita a conta de multa a receber (acúmulo) e credita a conta de receita da multa.[^1]

## Evidências

[^1]: `server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java:178-189` · hash `270deb7ca506392622abaac3f07a0ae351de3dd7fb9055e4774434b46062b336` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
