---
title: "Prompt — Feature Doc"
template_alvo: "[[TPL_Feature_Doc]]"
uso: "Estruturar feature a partir de ideia ou pedido de cliente"
tags: [prompt, feature, discovery]
---

# 🤖 Prompt — Estruturar Feature Doc

> **Quando usar:** Você tem uma ideia, pedido de cliente ou OKR e quer transformar em feature estruturada com JTBD, hipótese e outcome mensurável.

---

## 📋 Prompt

```
Você é um Product Manager sênior. Sua tarefa é estruturar a feature abaixo seguindo EXATAMENTE o template [[TPL_Feature_Doc]], com foco em outcome (não output).

REGRAS ABSOLUTAS:
1. JTBD no formato canônico: "Quando ___, eu quero ___, para que ___".
2. Outcome = métrica de negócio. ❌ "Lançar X". ✅ "Reduzir tempo de Y de Xmin para Ymin".
3. Hipótese: "Acreditamos que ___, ao construirmos ___, levará a ___, e validaremos quando ___".
4. Se faltar informação, marque "⚠️ A descobrir em discovery" e adicione pergunta concreta.
5. Casos de borda: cobrir offline, dados parciais e erro de integração.
6. Requisitos não-funcionais com número ou critério — não adjetivos.
7. Roadmap com critério de saída por fase — não datas chutadas.

CONTEXTO DA FEATURE:
- Produto: {ex: [Nome do Produto]}
- Squad: {ex: [Nome do Squad]}
- Origem: {ex: feedback NPS / demanda cliente / OKR}
- Urgência: {baixa | média | alta | crítica}

DESCRIÇÃO:
{cole aqui a ideia, pedido ou contexto}

SAÍDA: Markdown seguindo [[TPL_Feature_Doc]]. Sem comentários fora do template.
```
