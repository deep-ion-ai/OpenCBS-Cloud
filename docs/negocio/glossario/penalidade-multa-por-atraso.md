---
tipo: termo
termo: Penalidade (multa por atraso)
sinonimos:
- Multa por atraso
- Penalty
- penalties
area: cobranca
origem: analises/A-0001.md
---

# Penalidade (multa por atraso)

- **Sinônimos:** Multa por atraso, Penalty, penalties
- **Área:** cobranca
- **Origem:** [analises/A-0001.md](../analises/A-0001.md)

## Definição de negócio

Regra cadastrada que define a multa cobrada de um empréstimo em atraso: tipo (valor fixo ou percentual anual sobre desembolso, saldo devedor, principal ou juros em atraso), faixa de dias de atraso, carência e as contas contábeis de acúmulo, receita e baixa.[^1]

## Onde vive no código

- tabela penalties
- classe com.opencbs.core.domain.Penalty
- classe LoanPenaltyAccrualProcessor (cálculo diário)
- classes em opencbs-loans/penalties (um cálculo por tipo)

## Evidências

[^1]: `server/opencbs-core/src/main/java/com/opencbs/core/domain/Penalty.java:19-20` · hash `1240390480ebb8eca3ee5e039e929255b21f39ed1629a6c4d1d89dac1876f638` · commit `ab200dde82bd9b87905bf24399240b0bbe83d2a7`
