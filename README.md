# notspam.studio · análises

Repositório que aloja as análises públicas de marca (one-shot, prospecção) do estúdio notspam.studio, publicadas via GitHub Pages.

Não confundir com [`relatorios`](https://github.com/AdrianaNotSpam/relatorios) — esse aloja relatórios mensais recorrentes de clientes activos.

## Site público

- Raiz (neutra): https://adriananotspam.github.io/analises/
- Análise por marca: https://adriananotspam.github.io/analises/<slug-marca>/

(Custom domain futuro: `analises.notspamstudio.com` — pendente DNS na OVH.)

## Estrutura

```
/
├── index.html          # página raiz neutra
├── robots.txt          # bloqueia indexação
├── <slug-marca>/
│   └── index.html      # análise da marca
└── README.md
```

Cada análise é um one-shot: vai a uma marca específica numa janela de tempo específica, com o objectivo de mostrar o tipo de trabalho do estúdio ao dono da marca.

## Como adicionar uma análise nova

1. Criar pasta `<slug-marca>/` (minúsculas, hífenes, sem acentos — ex.: `lemon-jelly`, `casa-portuguesa`)
2. Colocar `index.html` dentro, com todos os assets relativos (`assets/`, `fonts/`, etc.)
3. Garantir que tem `<meta name="robots" content="noindex, nofollow" />` no head
4. Commit + push

## Privacidade

- Repo é público (requisito do GitHub Pages grátis)
- Os HTML têm `noindex` (não aparecem no Google)
- `robots.txt` bloqueia todos os crawlers
- Página raiz não expõe a lista de marcas analisadas
