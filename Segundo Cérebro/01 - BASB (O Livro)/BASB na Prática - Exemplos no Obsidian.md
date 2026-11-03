---
title: "BASB na Prática - Exemplos no Obsidian"
author: Bruno De Brito
tags:
  - SecondBrain/BASB/PracticalExamples
category: SecondBrain/BASB
created: 2026-10-13
---
> [!info] Contexto desta nota
> Copiada do vault `SecondBrainObsidian` em 2026-11-02. Onde aparecem "este vault" e caminhos como `1 - Projects/`, a nota descreve aquele vault, não este.

> [!summary] Em uma frase
> Exemplos concretos de como cada etapa do BASB fica no Obsidian, usando os plugins que **já estão instalados** neste vault (Kindle, Web Clipper, Templater, Dataview, Tasks, Calendar).

## Mapa: etapa → ferramenta neste vault
| Etapa | Ferramenta | Onde cai |
|---|---|---|
| Capturar livro | `obsidian-kindle-plugin` | `3 - Resources/Library and Highlights/Highlight Summaries/Kindle/` |
| Capturar web | Obsidian Web Clipper | `3 - Resources/Clippings/` |
| Capturar ideia solta | Daily Note (Calendar) | `0 - Inbox/` |
| Organizar | Pastas PARA (`1 - Projects` a `4 - Archive`) + links | Ver [[PARA no Obsidian - Estrutura e Exemplos]] |
| Destilar | `**negrito**` e `==destaque==` | Dentro da própria nota |
| Expressar | Nota de projeto + Templater | Pasta do projeto |

## Exemplo 1: nota de projeto (formato)
```markdown
---
title: "Post LinkedIn - MVP"
tags:
  - Projects/LinkedInMVP
status: ativo
deadline: 2026-10-30
---
## Objetivo
Publicar um post sobre MVP usando A Startup Enxuta.

## Material (pacotes intermediários)
- [[A startup enxuta - Eric Ries]]: destacar trechos sobre MVP
- [[Prompts Linkeidn]]: prompt de revisão de texto

## Tarefas
- [ ] Destilar highlights (camada 2) 📅 2026-10-20
- [ ] Rascunho 📅 2026-10-25
- [ ] Publicar 📅 2026-10-30

> [!todo] Ponte de Hemingway
> Próximo passo: ...
```
As tarefas com `📅` são do plugin **Tasks** e aparecem em qualquer consulta de tarefas do vault.

## Exemplo 2: destilando um highlight do Kindle
Antes (camada 1, como o plugin entrega):
> O único jeito de vencer é aprender mais rápido que todo mundo.

Depois (camadas 2 e 3, na 2ª leitura):
> O único jeito de vencer é ==**aprender mais rápido**== que todo mundo.

E no topo da nota do livro (camada 4):
```markdown
> [!summary] Resumo
> - Velocidade de aprendizado > velocidade de entrega.
> - MVP = experimento, não produto.
```

## Exemplo 3: painel de projetos ativos (Dataview)
Cole numa nota "Home" ou "Projetos":
````markdown
```dataview
TABLE status, deadline
FROM "1 - Projects"
WHERE status = "ativo"
SORT deadline ASC
```
````

## Exemplo 4: as tarefas da semana (Tasks)
````markdown
```tasks
not done
due before in 7 days
group by filename
```
````

## Ver também
- [[O Método CODE - Capturar Organizar Destilar Expressar]]
- [[PARA no Obsidian - Estrutura e Exemplos]]
- [[GTD no Obsidian - Estrutura e Exemplos]]
