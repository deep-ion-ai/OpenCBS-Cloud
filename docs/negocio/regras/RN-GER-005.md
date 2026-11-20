---
tipo: regra
id: RN-GER-005
titulo: 'Nos tipos percentuais, o percentual da penalidade é anual: o valor do dia é'
area: geral
status: confirmada
evidencias:
- arquivo: server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/PenaltyHelper.java
  linhas: 12-18
  hash: f84d27c79f6165511051ed766f91617470439f7a82ce085f576328a1ea7a7ec3
  commit: ab200dde82bd9b87905bf24399240b0bbe83d2a7
origem: analises/A-0001.md
---

# RN-GER-005 · Nos tipos percentuais, o percentual da penalidade é anual: o valor do dia é

- **Identificador:** RN-GER-005
- **Área:** geral
- **Status:** confirmada
- **Origem:** [analises/A-0001.md](../analises/A-0001.md)

## Enunciado

Nos tipos percentuais, o percentual da penalidade é anual: o valor do dia é base × percentual ÷ (dias do ano × 100), arredondado a 2 casas (arredondamento bancário). Dias do ano = 365 ou 366 conforme o ano da data de cálculo.[^1]

## Evidências

[^1]: `server/opencbs-loans/src/main/java/com/opencbs/loans/penalties/PenaltyHelper.java:12-18` · hash `f84d27c79f6165511051ed766f91617470439f7a82ce085f576328a1ea7a7ec3` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
