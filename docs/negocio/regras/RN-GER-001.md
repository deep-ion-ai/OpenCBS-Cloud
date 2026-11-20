---
tipo: regra
id: RN-GER-001
titulo: A multa é calculada no fechamento do dia, uma vez por empréstimo, olhando as
area: geral
status: confirmada
evidencias:
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java
  linhas: 62-72
  hash: 118b4e7d0ee4a8b192466cb6216a61f4dc2cdd2585d1733f99b3ef19d60ee74a
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
origem: analises/A-0001.md
---

# RN-GER-001 · A multa é calculada no fechamento do dia, uma vez por empréstimo, olhando as

- **Identificador:** RN-GER-001
- **Área:** geral
- **Status:** confirmada
- **Origem:** [analises/A-0001.md](../analises/A-0001.md)

## Enunciado

A multa é calculada no fechamento do dia, uma vez por empréstimo, olhando as parcelas não pagas cujo vencimento é anterior ao dia do fechamento (data de referência = dia anterior ao fechamento). Empréstimo sem penalidades configuradas não gera multa.[^1]

## Evidências

[^1]: `server/opencbs-loans/src/main/java/com/opencbs/loans/services/loancloseday/LoanPenaltyAccrualProcessor.java:62-72` · hash `118b4e7d0ee4a8b192466cb6216a61f4dc2cdd2585d1733f99b3ef19d60ee74a` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
