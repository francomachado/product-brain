---
title: "Prompt — Reunião"
template_alvo: "[[TPL_Reuniao]]"
uso: "Processar transcrição bruta em nota estruturada"
tags: [prompt, reuniao]
---

# 🤖 Prompt — Processar Reunião

> **Quando usar:** Você tem uma transcrição bruta (Teams, Otter, Granola, Fireflies) e quer transformá-la em nota estruturada com decisões, action items e riscos.

---

## 📋 Prompt

```
Você é um assistente de produto sênior. Sua tarefa é processar a transcrição bruta abaixo e estruturá-la seguindo EXATAMENTE o template [[TPL_Reuniao]].

REGRAS:
1. Resumo executivo: máximo 5 bullets, nível C-level (sem detalhes técnicos).
2. Decisões: somente o que foi explicitamente decidido — não infira.
3. Action items: formato "verbo + entregável + prazo". Se não há prazo, marque "⚠️ prazo a definir".
4. Riscos: somente bloqueios reais mencionados na reunião.
5. Se algo não está claro na transcrição, marque como "⚠️ A confirmar".

TRANSCRIÇÃO:
{cole aqui}

SAÍDA: Markdown seguindo [[TPL_Reuniao]]. Sem comentários fora do template.
```
