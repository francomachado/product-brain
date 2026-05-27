---
title: "DEC — {{title}}"
data: {{date:YYYY-MM-DD}}
status: proposta   # proposta | aprovada | rejeitada | substituida
decisor: ""
contexto_projeto: ""
tipo: decision-record
tags: [decisao, adr]
---

# 🎯 Decisão — {{title}}

> 🤖 Para estruturar trade-offs e matriz ponderada, use [[PROMPT_Decision_Record]].

> **Data:** {{date:DD/MM/YYYY}} · **Status:** `proposta`
> **Decisor:** [[ ]] · **Projeto:** [[ ]]

## 🧭 Contexto

_(Qual o cenário? Por que precisamos decidir algo agora? Que pressões existem?)_

## ❓ Pergunta a decidir

> _(Uma frase única, em formato de pergunta fechada — respondível com o nome de uma opção.)_

## 🔀 Opções consideradas

### Opção A — _____
- ✅ Prós:
- ❌ Contras:
- 💰 Custo / esforço: S | M | L | XL
- ⏱️ Time-to-value:
- 🔁 Reversibilidade: Fácil | Média | Difícil

### Opção B — _____
- ✅ Prós:
- ❌ Contras:
- 💰 Custo / esforço:
- ⏱️ Time-to-value:
- 🔁 Reversibilidade:

### Opção C — _____ _(se aplicável)_
- ✅ Prós:
- ❌ Contras:
- 💰 Custo / esforço:
- ⏱️ Time-to-value:
- 🔁 Reversibilidade:

## 🏛️ Critérios de decisão

> Pesos devem somar 100% e refletir o contexto real da decisão.

| Critério | Peso | Opção A | Opção B | Opção C |
|----------|------|---------|---------|---------|
| Time-to-market | % |  |  |  |
| TCO de 12 meses | % |  |  |  |
| Risco técnico / compliance | % |  |  |  |
| Diferencial competitivo | % |  |  |  |
| Reversibilidade | % |  |  |  |
| **Total ponderado** | 100% |  |  |  |

> _Notas 1–5 por critério (5 = melhor). Soma ponderada decide._

## ✅ Decisão

> **Optamos por _____ porque _____.**

## 📐 Consequências

**Esperadas:**
-

**Trade-offs aceitos:**
-

## 🔁 Quando revisitar

> _(Evento ou métrica observável — não data arbitrária.)_
> Ex: "Quando o custo mensal ultrapassar R$ X" ou "Se o concorrente Y lançar Z".

## 🔗 Notas relacionadas

- [[ ]]
