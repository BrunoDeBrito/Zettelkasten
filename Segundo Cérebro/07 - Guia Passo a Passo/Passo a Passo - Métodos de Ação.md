---
title: "Passo a Passo - Métodos de Ação"
author: Bruno De Brito
tags:
  - SecondBrain/StepByStep/ActionMethods
category: SecondBrain/StepByStep
created: 2026-11-02
---
> [!summary] Em uma frase
> Estes métodos respondem a **"o que faço agora?"**: mantenha **um** sistema de tarefas como fonte da verdade (hoje, o GTD-leve) e use os outros como complementos.

## GTD
**Use quando:** tiver muitos compromissos e sua cabeça virar lista de tarefas. Método de David Allen. Teoria: [[GTD]], com passos no Obsidian em [[GTD no Obsidian - Estrutura e Exemplos]].

**Versão leve (a base):**
1. **Capture** tudo na Daily Note.
2. **Esclareça** no fim do dia: isso exige ação? Se não, descarte, guarde ou deixe para "algum dia".
3. Se levar **menos de 2 minutos**, faça agora.
4. Se tiver mais de um passo, é um **projeto**: crie a nota e defina a próxima ação física.
5. **Organize** com o plugin Tasks, usando data apenas onde houver prazo real.
6. **Revise** toda semana com `Templates/Second Brain - Revisão Semanal.md`.
7. **Engaje:** escolha de 1 a 3 itens a cada manhã.

**Para ir além da versão leve:** acrescente listas por contexto, como `@pc` e `@rua`, a lista "aguardando" e os [[Horizontes de Foco]].

**Melhor forma:** escreva ações que comecem com verbo. `Abrir o Web Clipper e mudar a pasta`, e não `Web Clipper`.
**Evite:** pular a revisão semanal. Sem ela, o sistema perde a confiança, e isso costuma ser o fim do método.
**Teste:** faça 4 revisões semanais seguidas.

## Bullet Journal
**Use quando:** preferir papel ou quiser mais reflexão sobre as tarefas. Método de Ryder Carroll. Teoria: [[Bullet Journal]].

1. Separe um caderno e reserve as primeiras páginas para o **índice**.
2. Crie o **registro futuro** com os próximos meses.
3. Crie o **registro mensal**: calendário de um lado, tarefas do outro.
4. Faça o **registro diário** com frases curtas: `•` tarefa, `○` evento e `–` nota.
5. Marque `×` para feito, `>` para migrado e risque o que deixou de importar.
6. No fim do mês, **migre** à mão só o que ainda vale a pena.

**Melhor forma:** o valor está na migração. Reescrever à mão força a pergunta "isso ainda importa?".
**Evite:** transformar em projeto de arte, ou manter tarefas em dois sistemas ao mesmo tempo.
**Teste:** troque o sistema digital pelo papel por 2 semanas. Quantas tarefas você abandonou de propósito?

## Kanban pessoal
**Use quando:** começar muita coisa e terminar pouca. Método de Jim Benson e Tonianne DeMaria Barry.

1. Crie um quadro com o plugin Kanban (já instalado).
2. Use três colunas: `A fazer`, `Fazendo` e `Feito`.
3. Coloque em cartões as tarefas de um único fluxo, como os vídeos do canal.
4. **Limite `Fazendo` a 2 ou 3 itens.**
5. Só puxe algo novo quando um item terminar.
6. Uma vez por semana, veja onde os cartões ficam presos.

Para vídeos, as colunas podem ser: `Ideia`, `Roteiro`, `Gravação`, `Edição` e `Publicado`.

**Melhor forma:** o limite é o método. Sem ele, o quadro é só uma lista bonita.
**Evite:** duplicar no quadro as tarefas que já estão no Tasks. Use o quadro para fluxos e o Tasks para ações soltas.
**Teste:** 2 semanas com limite de 2. Mais coisas chegaram a `Feito`?

## Interstitial Journaling
**Use quando:** o dia passar sem que você saiba o que fez, ou quando for difícil voltar ao foco. Ideia de Besher Al Maleh.

1. Na Daily Note, crie uma seção `## Registro`.
2. **Sempre que trocar de tarefa**, escreva a hora e uma linha.
3. Registre o que terminou, como foi e o que vem a seguir.
4. Capture as ideias soltas ali mesmo, e processe tudo no fim do dia.

```markdown
## Registro
- 09:10 Terminei o bug do login. Era o cache da sessão. Agora: revisar PR.
- 10:25 PR revisado. Estou disperso; vou fazer uma pausa de 10 min.
- 10:40 Voltei. Próximo: escrever o teste da fila.
```

**Melhor forma:** escreva o que vem a seguir **antes** de abrir qualquer outra coisa.
**Evite:** registrar cada minuto. Basta uma linha nas transições.
**Teste:** 5 dias úteis. Ao final, leia os registros e procure um padrão.

## Time Blocking
**Use quando:** tiver tempo para estudar em tese, mas nunca na prática. Popularizado por Cal Newport.

1. Antes de começar o dia, liste o que precisa acontecer.
2. Divida o dia em blocos na Daily Note ou no calendário.
3. Coloque a tarefa mais difícil no seu melhor horário.
4. Agrupe as tarefas pequenas, como e-mail e mensagens, em um só bloco.
5. Deixe uma folga para imprevistos.
6. Quando o plano quebrar, **refaça o resto do dia** sem culpa.
7. Termine o dia com um ritual: revise as tarefas e planeje o amanhã.

**Melhor forma:** reserve antes os blocos de estudo do seu plano, como se fossem reuniões.
**Evite:** planejar sem folga, ou desistir no primeiro imprevisto.
**Teste:** planeje os blocos por 2 semanas. Compare o planejado e o realizado, e corrija sua estimativa.

## Como eles convivem
| Pergunta | Ferramenta |
|---|---|
| Quais são todas as minhas ações? | GTD (Tasks) |
| Em que etapa está cada vídeo? | Kanban |
| Quando vou fazer isso hoje? | Time Blocking |
| O que aconteceu hoje? | Interstitial Journaling |

## Ver também
- [[Fluxograma de Processamento da Inbox]]
- [[Rotina Integrada - Diária Semanal Mensal]]
- [[Guia Passo a Passo]]
