# Projetos de HTML e CSS - SENAI

Autor: Matheus Boff (ADS - SENAI Sorocaba)

Este repositório reúne três projetos feitos para as aulas de HTML e CSS.

## Estrutura

```
.
├── atividade-01/        # Box Model + Flexbox
│   ├── index.html
│   └── style.css
├── vertice-css-puro/    # Página de vendas de carros em CSS puro
│   ├── index.html
│   └── style.css
└── vertice-tailwind/    # Mesma página feita com Tailwind CSS
    └── index.html
```

## 1. Atividade 01: 20 caixas (Box Model + Flexbox)

Página com 20 caixas para praticar o Box Model e o Flexbox.

- CSS externo, ligado ao HTML pela tag `<link>`.
- Cada caixa tem valores próprios de **Content** (`width`, `height`), **Padding**, **Border** e **Margin**.
- 20 propriedades de Flexbox para organizar as caixas, cada uma numerada nos comentários do CSS.
- Layout responsivo com `@media`.

**Como abrir:** abra `atividade-01/index.html` no navegador.

## 2. Vértice Motors (HTML e CSS puro)

Página de vendas de carros feita só com HTML e CSS, sem framework.

- Cabeçalho fixo, seção principal, busca, catálogo com 6 carros, diferenciais, depoimentos e rodapé.
- Classes no padrão BEM (ex.: `.card__title`) e cores e fontes em variáveis CSS.
- Responsivo, com Flexbox, Grid e `@media`.

**Como abrir:** abra `vertice-css-puro/index.html` no navegador.

## 3. Vértice Motors (Tailwind CSS)

A mesma página do projeto 2, agora feita com Tailwind CSS.

- Só o `index.html`: o estilo fica nas classes utilitárias (ex.: `flex items-center gap-4`).
- Cores e fontes configuradas em `tailwind.config`, dentro do próprio HTML.
- Tailwind carregado por CDN, então **precisa de internet** para aparecer estilizado.

**Como abrir:** abra `vertice-tailwind/index.html` no navegador.

## Comparação: CSS puro x Tailwind

| | CSS puro | Tailwind |
|---|---|---|
| Arquivos | HTML + CSS | Só HTML |
| Nomes de classes | Criados por mim (`.card__title`) | Já prontos (`text-lg font-bold`) |
| Responsivo | `@media` no fim do CSS | Prefixos na classe (`md:flex`) |
| Hover | Regra separada (`.card:hover`) | Na classe (`hover:-translate-y-1`) |
| Reuso | Uma classe serve para vários elementos | As classes se repetem no HTML |
| HTML | Mais limpo | Mais longo |

## Tecnologias

HTML5, CSS3 (Box Model, Flexbox, Grid, variáveis) e Tailwind CSS (via CDN).
