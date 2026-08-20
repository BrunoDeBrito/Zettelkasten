---
tags:
  - ZettelkastenMethod/ObsidianSetup/BacklinksAndGraph
category: ZettelkastenMethod/ObsidianSetup
created: 2026-08-19
---
> [!summary] Em uma frase
> Backlinks (painel nativo do Obsidian) mostram quem aponta para a nota que você está lendo — é o equivalente digital de "quais fichas físicas foram colocadas perto desta". O grafo é a visão macro da mesma informação. Os dois juntos são a ferramenta de descoberta de conexão que Luhmann fazia manualmente.

## Backlinks: o mecanismo mais importante que ninguém usa direito

Todo link `[[Nota B]]` escrito dentro de "Nota A" cria automaticamente uma entrada no painel de **Backlinks** de "Nota B", visível quando você abre ela. Isso significa: **ao criar uma nota nova e linkar para 3 notas antigas, essas 3 notas antigas "ganham" uma referência de volta sem trabalho extra.**

Prática recomendada: sempre que terminar de escrever uma nota permanente, **abra cada nota que você linkou** e confira o painel de Backlinks dela — é comum notar ali outra nota relacionada que você tinha esquecido, porque ela também aparece na mesma lista de backlinks.

## Grafo: útil para diagnóstico, não para navegação do dia a dia

O grafo visual (Configurações → Núcleo → Grafo, já habilitado neste vault) é ótimo para **duas coisas específicas**:

1. **Achar notas órfãs** — nós isolados, sem nenhuma linha, saltam aos olhos visualmente.
2. **Ver clusters temáticos emergirem** — se você colorir por tag/pasta (Configurações do grafo → Grupos), áreas densas revelam onde um assunto amadureceu o suficiente para merecer uma [[Notas Estruturais e MOCs|MOC]].

Não é bom para navegação cotidiana (fica poluído rápido com >100 notas) — para isso, use busca (`Ctrl/Cmd+O`) e os próprios backlinks.

## Query Dataview para achar notas órfãs

O mesmo mecanismo do Dataview serve para achar notas sem link de saída — um sinal de nota mal-processada (ver [[Erros Comuns e Como Evitá-los]]):

```dataview
LIST
FROM "" AND -"Templates"
WHERE length(file.outlinks) = 0
```

E notas sem nenhum backlink de entrada precisam ser checadas manualmente (Dataview não expõe `file.inlinks` de forma direta) — abra o painel de Backlinks de cada nota nova recém-criada como parte da rotina, ver [[Rotina Diária e Semanal de Manutenção]].

## Local graph — o "grafo pessoal" de cada nota

Além do grafo global, o Obsidian tem um **Grafo Local** (ícone no canto de cada nota, ou comando "Abrir grafo local") que mostra só os vizinhos diretos (1–2 saltos) da nota atual. É a visão mais útil no momento de decidir onde conectar uma nota nova: abra o grafo local de uma nota candidata a link e veja rapidamente o que já está perto dela.

## Ver também
- [[Estrutura Pastas vs Tags vs Links]]
- [[Notas Estruturais e MOCs]]
- [[Métricas e Revisão Periódica do Sistema]]
