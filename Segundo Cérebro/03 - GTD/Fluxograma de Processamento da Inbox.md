---
title: "Fluxograma de Processamento da Inbox"
author: Bruno De Brito
tags:
  - SecondBrain/GTD/InboxFlowchart
category: SecondBrain/GTD
created: 2026-10-13
---
> [!summary] Em uma frase
> O fluxograma do GTD transforma cada item da inbox numa **decisão**: lixo, referência, algum dia, faça agora, delegue ou agende. Nada volta para a inbox.

## O fluxograma

```mermaid
flowchart TD
    I[Item na inbox] --> Q1{O que é?<br/>É acionável?}
    Q1 -- Não --> N1[Lixo]
    Q1 -- Não --> N2[Algum dia / talvez]
    Q1 -- Não --> N3[Referência<br/>PARA / Zettelkasten]
    Q1 -- Sim --> Q2{Mais de uma ação<br/>para concluir?}
    Q2 -- Sim --> P[Lista de Projetos<br/>+ definir próxima ação]
    P --> Q3
    Q2 -- Não --> Q3{Qual a próxima ação?<br/>Leva menos de 2 min?}
    Q3 -- Sim --> D[FAÇA AGORA]
    Q3 -- Não --> Q4{Sou eu quem<br/>deve fazer?}
    Q4 -- Não --> W[Delegue<br/>lista Aguardando]
    Q4 -- Sim --> Q5{Tem dia/hora<br/>específicos?}
    Q5 -- Sim --> C[Agenda]
    Q5 -- Não --> NA[Próximas Ações<br/>por contexto]
```

## As regras do processamento
1. **De cima para baixo**, um item por vez. Não escolha o mais fácil primeiro.
2. **Nada volta para a inbox.** Cada item sai com uma decisão.
3. **Regra dos 2 minutos:** se fazer leva menos que organizar, faça.
4. Se o item é **informação** (não ação), ele sai do GTD e vai para o [[PARA]] ou para o [[Zettelkasten Method]]. Aqui os sistemas se encontram.

## Exemplos de decisões
| Item | Decisão |
|---|---|
| "Responder e-mail do recrutador" (1 min) | Faça agora |
| "Ideia: vídeo sobre Xdebug" | Algum dia/talvez (ou projeto, se for fazer este mês) |
| "Highlight de A Arte da Guerra" | Referência → Recursos/Livros |
| "Pedir pro colega revisar o PR" | Delegue → Aguardando |
| "Dentista terça 14h" | Agenda |
| "Configurar CI do projeto pessoal" | Próximas ações `@computador` |
| "Insight: atomicidade vale para funções também" | Referência → nota fugaz do Zettelkasten |

## Ver também
- [[As 5 Etapas do GTD]]
- [[Como Decidir Onde uma Nota Vai]]: a árvore do PARA, que entra no galho "Referência"
- [[Notas Fugazes (Fleeting Notes)]]: o galho "insight" vai para o Zettelkasten
