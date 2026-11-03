---
title: "LYT na Prática - Exemplos no Obsidian"
author: Bruno De Brito
tags:
  - SecondBrain/LYT/PracticalExamples
category: SecondBrain/LYT
created: 2026-10-13
---
> [!summary] Em uma frase
> Na prática, LYT é: **capturar** numa Daily Note, **relacionar** linkando a um MOC (ou criando um quando der aperto) e **usar** os MOCs como ponto de partida para escrever e estudar.

## Fluxo de um dia típico
1. Abre a **Home**, que mostra os MOCs e os esforços "On".
2. Durante o dia, anota na **Daily Note** (Calendar).
3. Algo vale virar nota? Cria a nota (um "Dot") e **linka a pelo menos um MOC**. Isso substitui decidir uma pasta.
4. Se um MOC ficou grande demais, divide em dois (ex.: "Programação MOC" → "PHP MOC" + "Docker MOC").

## Exemplo: nota "Dot" (ideia)
```markdown
---
title: "Strategy e State parecem iguais mas diferem em quem decide a troca"
tags:
  - Atlas/Dots
up: "[[Padrões de Projeto MOC]]"
---
No Strategy, o **cliente** escolhe o algoritmo. No State, o **próprio objeto**
muda de estado e troca o comportamento sozinho.

Fonte: [[Strategy]], [[State]] (Refactoring Guru)
```

A propriedade `up` é uma convenção do LYT: aponta para o MOC "pai". Plugins como *Breadcrumbs* usam isso para navegação, mas funciona sem plugin também (é só um link).

## Exemplo: consulta de esforços na Home
````markdown
```dataview
TABLE rank AS "Prioridade"
FROM "Efforts/On"
SORT rank DESC
```
````

## Exemplo: achar notas sem MOC (órfãs de mapa)
````markdown
```dataview
LIST FROM "Atlas/Dots"
WHERE !up
```
````

## O que pegar do LYT mesmo sem adotar o ACE
- A **Home note**.
- A propriedade **`up`** ligando nota → MOC.
- O critério do **"mental squeeze point"** para criar MOCs.
- A ideia de **esforços por intensidade** (On, Simmering, Sleeping) em vez de "ativo/inativo". Ótimo para cursos que andam devagar.

## Ver também
- [[MOCs e Home Note]]
- [[Backlinks Grafo e Descoberta de Conexões]]
