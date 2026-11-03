---
title: "MOCs e Home Note"
author: Bruno De Brito
tags:
  - SecondBrain/LYT/MOCsAndHome
category: SecondBrain/LYT
created: 2026-10-13
---
> [!info] Contexto desta nota
> Copiada do vault `SecondBrainObsidian` em 2026-11-02. Onde aparecem "este vault" e caminhos como `1 - Projects/`, a nota descreve aquele vault, não este.

> [!summary] Em uma frase
> Um **MOC (Map of Content)** é uma nota-mapa que junta links sobre um tema e explica como eles se relacionam. A **Home note** é o MOC dos MOCs: o ponto de partida do vault.

## O que diferencia um bom MOC de uma lista de links
| Lista de links (fraca) | MOC (bom) |
|---|---|
| `- [[Docker]]` `- [[Xdebug]]` | Agrupa por subtema, com cabeçalhos |
| Sem contexto | Uma frase por link dizendo **por que** ele está ali |
| Gerada sozinha | Curada à mão (pode **ter** um Dataview no fim, mas não **ser** só isso) |
| Estática | Evolui: ganha seções, perguntas abertas, tensões |

## Quando criar um MOC
- Quando você tem **5 ou mais notas** sobre um tema e já se perde para achá-las.
- Quando começa um **estudo** de um tema novo e quer um lugar para ir juntando.
- **Nunca** "para organizar desde já" um tema vazio.

## Formato sugerido de MOC
```markdown
---
title: "Padrões de Projeto MOC"
tags:
  - Atlas/Maps/DesignPatterns
---
> [!summary] Sobre
> Como eu entendo design patterns: quando ajudam, quando atrapalham.

## Começar por aqui
- [[Padrão de projeto]]: definição
- [[Crítica dos padrões]]: o contraponto, ler cedo

## Por intenção
- **Criar objetos:** [[Factory Method]], [[Builder]]
- **Trocar comportamento:** [[Strategy]], [[State]]: os dois parecem iguais, a diferença é quem decide a troca

## Perguntas abertas
- Em Laravel, Service Container substitui Factory?

## Tudo sobre o tema (auto)
(Dataview no fim, como rede de segurança)
```

## Home note
Uma nota só, aberta ao iniciar o Obsidian (dá para configurar com o core plugin de Workspaces ou o plugin Homepage). Conteúdo típico:
- Links para os 5 a 10 MOCs principais
- Painel de projetos ativos (Dataview)
- Link para a Daily Note de hoje
- [[Os 12 Problemas Favoritos]]

O `README.md` deste vault já faz o papel de Home; ele pode evoluir para isso.

## Ver também
- [[Notas Estruturais e MOCs]]: a visão do Zettelkasten sobre o mesmo conceito
- [[LYT na Prática - Exemplos no Obsidian]]
