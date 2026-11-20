---
tipo: regra
id: RN-GER-004
titulo: 'Existem cinco tipos de penalidade, que definem a base de cálculo: valor fixo'
area: geral
status: confirmada
evidencias:
- arquivo: server/opencbs-core/src/main/java/com/opencbs/core/domain/enums/PenaltyType.java
  linhas: 4-10
  hash: 004c876e16acf3b2a22f5d542af0f26c4074b52b9aa09ed6cb42d840ac5d32d1
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
origem: analises/A-0001.md
---

# RN-GER-004 · Existem cinco tipos de penalidade, que definem a base de cálculo: valor fixo

- **Identificador:** RN-GER-004
- **Área:** geral
- **Status:** confirmada
- **Origem:** [analises/A-0001.md](../analises/A-0001.md)

## Enunciado

Existem cinco tipos de penalidade, que definem a base de cálculo: valor fixo (FLAT), valor desembolsado (BY_DISBURSEMENT_AMOUNT), saldo devedor de principal (BY_OLB), principal em atraso (BY_LATE_PRINCIPAL) e juros em atraso (BY_LATE_INTEREST).[^1]

## Evidências

[^1]: `server/opencbs-core/src/main/java/com/opencbs/core/domain/enums/PenaltyType.java:4-10` · hash `004c876e16acf3b2a22f5d542af0f26c4074b52b9aa09ed6cb42d840ac5d32d1` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
