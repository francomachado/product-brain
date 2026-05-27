# 🧠 Product Brain — Vault Template

> **Autor:** Paulo Franco
> **LinkedIn:** [linkedin.com/in/paulofrancomachado](https://www.linkedin.com/in/paulofrancomachado/)
> **Stack:** Obsidian + Claude Cowork + Python

---

## 🎯 O que é este vault

**Product Brain** é uma estrutura de segundo cérebro projetada para líderes de produto, plataforma e tecnologia. Ela organiza captura, processamento e tomada de decisão em um sistema único, auditável e navegável.

O vault responde a três perguntas que qualquer líder precisa responder rápido:

| Pergunta | Como o vault responde |
|----------|----------------------|
| **Onde captura?** | `00_Inbox/` recebe transcrições brutas, ideias e leituras |
| **Como processa?** | Templates + IA (Claude Cowork) transformam capturas em decisões estruturadas |
| **Onde decide?** | `01_Projects/` e `02_Areas/` mantêm o conhecimento organizado por método PARA |

---

## 🗂️ Estrutura (PARA Method)

```
ProductBrain/
├── 00_Dashboard.md                  ← Home do vault
├── 00_Inbox/                        ← CAPTURA BRUTA (processar em ≤48h)
│   ├── reunioes_brutas/             ← cole transcrições aqui
│   ├── ideias_rapidas/              ← pensamentos rápidos, sem filtro
│   └── leituras/                    ← PDFs, artigos, referências
│
├── 01_Projects/                     ← PROJECTS (com deadline e entregável)
│   └── Projeto_Exemplo/
│
├── 02_Areas/                        ← AREAS (responsabilidades contínuas)
│   ├── Lideranca_e_Pessoas/
│   ├── Plataforma_e_Arquitetura/
│   ├── Produto_e_UX/
│   └── Governanca_e_Compliance/
│
├── 03_Resources/                    ← RESOURCES (base de conhecimento atemporal)
│   ├── Produtos_e_Solucoes/         ← documentação dos seus produtos
│   │   ├── Produto_A/
│   │   └── Produto_B/
│   ├── Mercado_e_Segmento/          ← inteligência competitiva e de mercado
│   ├── Tecnologia_e_AI/             ← referências técnicas e de inovação
│   └── Referencias_Externas/        ← benchmarks, artigos, frameworks
│
├── 04_Archives/                     ← ARCHIVES (concluídos ou pausados)
│   ├── 2024/
│   ├── 2025/
│   └── 2026/
│
├── 05_Templates/                    ← TEMPLATES versionados
│   ├── TPL_Reuniao.md
│   ├── TPL_Weekly_Report.md
│   ├── TPL_Feature_Doc.md
│   ├── TPL_Projeto.md
│   ├── TPL_Decision_Record.md
│   ├── TPL_1on1.md
│   └── Prompts/                     ← prompts de IA para cada template
│
├── 06_Scripts/                      ← AUTOMAÇÃO
│   ├── doc_scraper.py               ← extrator de documentação pública
│   ├── requirements.txt
│   ├── urls.txt                     ← URLs seed para o scraper
│   └── output_logs/
│
├── 07_MOC/                          ← MAPS OF CONTENT (índices navegáveis)
│   ├── MOC_Produtos.md
│   ├── MOC_Decisoes.md
│   └── MOC_Reunioes.md
│
└── 99_Attachments/                  ← imagens, PDFs e arquivos anexados
```

---

## 🚀 Como usar

### 1. Abrir como vault no Obsidian

```bash
# Extraia o zip em uma pasta local
# No Obsidian: "Open folder as vault" → selecione a pasta ProductBrain/
```

Configurações recomendadas (ajuste em Settings → Files & Links):
- Novos arquivos → `00_Inbox/`
- Templates → `05_Templates/`
- Attachments → `99_Attachments/`
- Links no formato wiki `[[ ]]`

### 2. Adapte as pastas ao seu contexto

Substitua `Produto_A` e `Produto_B` em `03_Resources/Produtos_e_Solucoes/` pelos produtos reais da sua empresa. Adicione projetos em `01_Projects/` conforme necessário.

### 3. Instale os templates no Obsidian

Ative o plugin **Templates** nativo do Obsidian e aponte para `05_Templates/`. Para acesso via IA, conecte o Claude Cowork e use os prompts em `05_Templates/Prompts/`.

---

## 🔄 Fluxos de trabalho principais

### Fluxo A — Reunião vira decisão estruturada

```
Transcrição (Teams / Granola / Otter)
        │
        ▼
00_Inbox/reunioes_brutas/transcricao_YYYY-MM-DD.md
        │
        ▼  (IA processa com TPL_Reuniao)
        │
01_Projects/<projeto>/Reuniao_YYYY-MM-DD_<tema>.md
        ├── Resumo executivo
        ├── Decisões tomadas
        ├── Action items
        └── Riscos e bloqueios
        │
        ▼
Decision Record → Weekly Report
```

### Fluxo B — Feature nasce e amadurece

```
Ideia ou pedido de cliente
        │
        ▼
00_Inbox/ideias_rapidas/
        │
        ▼  (TPL_Feature_Doc — JTBD + hipótese + outcome)
        │
01_Projects/<produto>/Feature_<nome>.md
        │
        ▼
Decision Record para escolhas técnicas
        │
        ▼
Status: discovery → delivery → live
```

### Fluxo C — Documentação pública vira base de conhecimento

```
URLs públicas dos seus produtos
        │
        ▼
06_Scripts/doc_scraper.py
        │
        ▼
03_Resources/Produtos_e_Solucoes/<Produto>/*.md
        │
        ▼
07_MOC/MOC_Produtos.md (índice navegável)
```

---

## 📋 Templates inclusos

| Template | Quando usar |
|----------|-------------|
| `TPL_Reuniao` | Toda reunião — transcrição + resumo + decisões |
| `TPL_Weekly_Report` | Toda sexta — relatório semanal por projeto |
| `TPL_Feature_Doc` | Nova feature em discovery ou delivery |
| `TPL_Projeto` | Iniciar um novo projeto |
| `TPL_Decision_Record` | Decisões com ≥2 opções e trade-offs reais |
| `TPL_1on1` | Reuniões 1:1 com liderados diretos |

---

## 💡 Princípios do sistema

1. **PARA não é organização por categoria — é por acionabilidade.** Projects têm deadline. Areas são contínuas. Resources são atemporais. Archives são concluídos.
2. **Templates são contratos cognitivos.** Eles forçam você a pensar nos campos certos antes de começar a escrever.
3. **MOC é navegação por significado, não por localização.** Uma nota pode estar em qualquer pasta e aparecer em múltiplos MOCs.
4. **Automação coleta — você conecta.** Scripts alimentam o vault; a inteligência de ligação entre notas é sua.
5. **Decisões registradas protegem o decisor.** Um Decision Record escrito hoje responde a pergunta "por que fizemos isso?" em 12 meses.

---

> _"A mente é para ter ideias, não para guardá-las."_ — David Allen

> _"A vantagem competitiva de um líder não está no que ele lembra, mas no que ele consegue conectar."_ — Paulo Franco
