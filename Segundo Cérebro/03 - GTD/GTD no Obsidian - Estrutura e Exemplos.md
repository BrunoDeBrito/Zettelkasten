---
title: "GTD no Obsidian - Estrutura e Exemplos"
author: Bruno De Brito
tags:
  - SecondBrain/GTD/ObsidianSetup
category: SecondBrain/GTD
created: 2026-10-13
---
> [!info] Contexto desta nota
> Copiada do vault `SecondBrainObsidian` em 2026-11-02. Onde aparecem "este vault" e caminhos como `1 - Projects/`, a nota descreve aquele vault, não este.

> [!summary] Em uma frase
> Com o plugin **Tasks** (já instalado), dá para fazer GTD inteiro no Obsidian: tarefas ficam **dentro das notas de projeto** e as listas (próximas ações, aguardando, contextos) são **consultas**, não arquivos que você mantém à mão.

> [!question] Obsidian ou app separado?
> Muita gente usa um app dedicado (Todoist, TickTick, Things) para tarefas porque tem notificação, celular e recorrência melhores. Os dois caminhos funcionam. A regra do GTD é só: **um sistema confiável**. Se escolher app externo, linke a nota do projeto no Obsidian a partir da tarefa.

## Convenções sugeridas
| Conceito GTD | Formato no Obsidian |
|---|---|
| Inbox | Daily Note (`- [ ] coisa`) ou nota `0 - Inbox/Inbox.md` |
| Próxima ação | `- [ ] verbo + objeto #ctx/computador` |
| Contexto | Tag `#ctx/computador`, `#ctx/telefone`, `#ctx/rua`, `#ctx/casa` |
| Aguardando | Tag `#aguardando` + data `⏳` |
| Agenda | Data `📅` (ou calendário externo) |
| Algum dia/talvez | Nota `Algum Dia Talvez.md` ou status `[>]` |
| Projeto | Nota de projeto em `1 - Projects/` com as próprias tarefas |

Os status extras do `Basics.md` (`[/]` em andamento, `[>]` adiado, `[-]` cancelado, `[?]` dúvida) funcionam bem com o Tasks.

## Painel "Próximas Ações" (crie uma nota com isto)
````markdown
## @computador
```tasks
not done
tags include #ctx/computador
group by filename
```

## @telefone
```tasks
not done
tags include #ctx/telefone
```

## Aguardando
```tasks
not done
tags include #aguardando
sort by scheduled
```

## Atrasadas
```tasks
not done
due before today
```
````

## Projetos sem próxima ação (o check mais importante da revisão)
````markdown
```dataviewjs
for (const p of dv.pages('"1 - Projects"').where(p => p.status === "ativo")) {
  const open = p.file.tasks.where(t => !t.completed);
  if (open.length === 0) dv.paragraph("⚠️ " + p.file.link);
}
```
````

## Exemplo de Daily Note como inbox
```markdown
# 2026-10-13
## Captura
- [ ] ver vaga Stripe
- ideia: vídeo sobre Xdebug no Docker
- "aprender mais rápido que todo mundo" (Startup Enxuta)
- [ ] ligar dentista

## Processado na revisão
(mover cada item para o lugar certo, ver [[Fluxograma de Processamento da Inbox]])
```

## Ver também
- [[Listas, Contextos e Próximas Ações]]
- [[PARA no Obsidian - Estrutura e Exemplos]]
- [[Template - Revisão Semanal Integrada]]
