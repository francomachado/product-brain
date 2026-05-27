---
title: "Como usar Scripts"
tags: [scripts, automacao, instrucao]
---

# ⚙️ Como usar Scripts

Scripts que automatizam tarefas repetitivas do vault.

## Scripts disponíveis

| Script | O que faz |
|--------|-----------|
| `doc_scraper.py` | Extrai documentação pública de URLs e gera notas `.md` em `03_Resources/Produtos_e_Solucoes/` |

## Como instalar

```bash
cd 06_Scripts
pip install -r requirements.txt
```

## Como usar o scraper

```bash
# Modo 1 — URLs do arquivo seed
python doc_scraper.py --file urls.txt

# Modo 2 — URL avulsa
python doc_scraper.py https://seusite.com/produto/

# Modo 3 — Forçar reescrita de arquivos existentes
python doc_scraper.py --file urls.txt --overwrite
```

## Adicionar novos produtos

Edite o dicionário `PRODUCT_MAP` em `doc_scraper.py`:

```python
PRODUCT_MAP = {
    "slug-do-produto": "NomeDoProduto",
    # adicione aqui
}
```

## output_logs/

Logs de execução do scraper ficam aqui. Ignorados pelo git por padrão.
