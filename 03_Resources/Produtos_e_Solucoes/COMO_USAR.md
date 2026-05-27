---
title: "Como usar Produtos e Soluções"
tags: [produtos, resources, instrucao]
---

# 📦 Como usar Produtos e Soluções

Esta pasta contém uma subpasta para cada produto ou solução da sua empresa.

## Como adicionar um produto

1. Crie uma subpasta: `03_Resources/Produtos_e_Solucoes/NomeDoProduto/`
2. Crie a nota principal `NomeDoProduto.md` com descrição, links e contexto
3. Adicione o produto ao [[MOC_Produtos]]

## Automatização

Use `06_Scripts/doc_scraper.py` para extrair documentação pública automaticamente:

```bash
python doc_scraper.py --file urls.txt
```

Cada URL gera um `.md` na pasta do produto correspondente.
