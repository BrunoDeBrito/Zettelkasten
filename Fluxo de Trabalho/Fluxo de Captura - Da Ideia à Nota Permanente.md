---
tags:
  - ZettelkastenMethod/Workflow/CaptureToPermanent
category: ZettelkastenMethod/Workflow
created: 2026-08-19
---
> [!summary] Em uma frase
> Toda ideia percorre o mesmo funil de 4 estágios — captura, literatura, permanente, estrutura — nunca pulando etapa direto para "permanente", porque é a passagem por cada estágio que faz o processamento cognitivo acontecer.

## O funil completo

```
[Fonte externa: livro, curso, conversa, ideia solta]
        │
        ▼
1. FLEETING NOTE  ──── captura rápida, sem filtro, sem formatação
   [[Notas Fugazes (Fleeting Notes)]]
        │  (processamento em até poucos dias)
        ▼
2. LITERATURE NOTE  ── resumo com suas palavras, ainda preso à fonte
   [[Notas de Literatura (Literature Notes)]]
        │  (extrair cada ideia relevante, uma de cada vez)
        ▼
3. PERMANENT NOTE  ─── atômica, autônoma, conectada à rede
   [[Notas Permanentes (Permanent Notes)]]
        │  (quando um cluster de permanentes emerge)
        ▼
4. STRUCTURE NOTE / MOC  ─ ponto de entrada navegável do assunto
   [[Notas Estruturais e MOCs]]
```

## Por que não pular etapas

Ir direto de "livro" para "nota permanente" é o erro mais silencioso do método: parece economia de tempo, mas produz notas que são na verdade resumos de literatura disfarçados (título com nome do autor, não fazem sentido fora do contexto do livro) — ver o teste de autonomia em [[Princípios Fundamentais do Zettelkasten]]. O funil de 4 etapas força a reformulação a acontecer **duas vezes** (uma na nota de literatura, outra na permanente), e é essa segunda reformulação — já sem o livro aberto do lado — que produz a versão realmente atômica e independente da ideia.

## Este vault, estágio por estágio

| Estágio | Onde mora | Ferramenta |
|---|---|---|
| Fleeting | Daily Note do dia (Calendar plugin) ou uma `Inbox.md` na raiz | Captura rápida, texto solto |
| Literature | Uma pasta de referência (aqui ou em outro vault de PARA) | `Templates/Zettelkasten - Literature Note.md` |
| Permanent | Pasta temática dentro deste vault (`Fundamentos/`, `Estratégia/`, ou uma nova por assunto) | `Templates/Zettelkasten - Permanent Note.md` |
| Structure/MOC | Raiz do assunto (ex: `Zettelkasten Method.md`) | `Templates/Zettelkasten - MOC Template.md` |

## Tempo esperado por etapa (calibre a expectativa)

- Fleeting → Literature: minutos por item, mas processado em lote (ver [[Rotina Diária e Semanal de Manutenção]]).
- Literature → Permanent: **é aqui que mora o trabalho de verdade** — 10 a 30 minutos por nota permanente bem-feita não é incomum. Não é um sistema de "anotação rápida"; é um sistema de "pensamento devagar e registrado".
- Permanent → MOC: acontece raramente, só quando um cluster temático amadurece (podem passar semanas/meses entre a criação de uma MOC e outra).

> [!important] Não é uma esteira de produção
> A meta não é "processar 100% das fleeting notes". A maioria delas será descartada no estágio 1→2, e está tudo certo — o funil é um filtro de qualidade, não uma fila que precisa zerar.

## Ver também
- [[Rotina Diária e Semanal de Manutenção]]
- [[Como Escrever uma Boa Nota Permanente]]
- [[Do Zettelkasten à Criação - Escrita Estudo e Decisões]]
