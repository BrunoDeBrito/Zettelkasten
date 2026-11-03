---
title: "Bullet Journal"
author: Bruno De Brito
tags:
  - SecondBrain/OtherMethods/BulletJournal
category: SecondBrain/OtherMethods
created: 2026-10-13
---
> [!summary] Em uma frase
> O **Bullet Journal** (Ryder Carroll) é um método de caderno para tarefas, eventos e notas, baseado em **registro rápido** com símbolos e na **migração** consciente de tarefas. A ideia de migração é uma das melhores ferramentas contra listas que só crescem.

## Os símbolos (rapid logging)
| Símbolo | Significado | Equivalente no Obsidian (Basics.md) |
|---|---|---|
| `•` | Tarefa | `- [ ]` |
| `×` | Tarefa feita | `- [x]` |
| `>` | Migrada (levada para frente) | `- [>]` |
| `<` | Agendada (para o futuro log) | `- [<]` |
| `○` | Evento | — (use data) |
| `–` | Nota | `- texto` |
| `*` | Prioridade | `- [!]` ou `- [*]` |

Repare que os status de checkbox em `Basics.md` já trazem essa linguagem.

## Os módulos
- **Index:** sumário do caderno.
- **Future Log:** os próximos meses, coisas com data distante.
- **Monthly Log:** calendário + tarefas do mês.
- **Daily Log:** o registro do dia, escrito ao longo dele.
- **Coleções:** listas temáticas (livros para ler, ideias de vídeo).

## A migração (a parte mais valiosa)
No fim do mês, você olha **cada tarefa aberta** e decide:
1. Ainda importa? → **migra** (`>`) para o mês seguinte, **reescrevendo à mão**.
2. Não importa mais? → **risca**.

Reescrever dá trabalho **de propósito**: se não vale o trabalho de copiar, não vale fazer. Isso mata tarefas zumbis.

## Como aplicar no Obsidian
- **Daily Note** = Daily Log.
- **Status `[>]`** ao adiar uma tarefa, em vez de deixar ela atrasada para sempre.
- **Revisão mensal:** consulta das tarefas abertas há mais de 30 dias e decisão consciente para cada uma:
````markdown
```tasks
not done
created before 30 days ago
```
````
(Precisa que o Tasks registre a data de criação: opção "Set created date on every added task" nas configurações do plugin.)

## Ver também
- [[GTD no Obsidian - Estrutura e Exemplos]]
- [[Rotina Integrada - Diária Semanal Mensal]]
