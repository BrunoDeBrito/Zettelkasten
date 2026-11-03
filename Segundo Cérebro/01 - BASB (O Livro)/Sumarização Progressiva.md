---
title: "Sumarização Progressiva"
author: Bruno De Brito
tags:
  - SecondBrain/BASB/ProgressiveSummarization
category: SecondBrain/BASB
created: 2026-10-13
---
> [!summary] Em uma frase
> Sumarização Progressiva é destacar uma nota em **camadas**, cada uma mais curta que a anterior. A próxima camada só é feita **quando você volta a usar a nota**, de forma que o esforço vai para o que é realmente útil.

## As camadas

| Camada | O que fazer | Formatação | Quando |
|---|---|---|---|
| **0** | O texto original completo | — | Fica na fonte (livro, site) |
| **1** | Os trechos que você capturou | Texto normal | Na captura |
| **2** | As partes mais importantes da camada 1 | **Negrito** | Na 1ª vez que reabrir a nota |
| **3** | O melhor do negrito | ==Destaque== | Na 2ª vez que reabrir |
| **4** | Resumo com suas palavras | Bullet points no topo | Só se a nota for muito usada |
| **5** | Remix: a nota vira algo seu | Post, aula, código, nota permanente | Quando for expressar |

> [!important] A regra de ouro
> **Nunca destile tudo na captura.** Destilar é trabalho, e só vale o trabalho para notas que provaram ser úteis (você voltou a elas). A maioria das notas fica para sempre na camada 1, e tudo bem.

## Exemplo visual (como fica a nota)

```markdown
## Resumo (camada 4)
- Aprendizado validado vale mais que funcionalidades entregues.
- MVP serve para testar hipótese, não para lançar produto.

## Trechos (camadas 1 a 3)
"O MVP é aquela versão do produto que permite uma volta completa do
ciclo construir-medir-aprender, com o **mínimo de esforço e o menor
tempo de desenvolvimento**." Isso ajuda equipes a ==validar
hipóteses antes de gastar meses construindo==.
```

No Obsidian, `==texto==` gera o destaque amarelo. O Kindle plugin já entrega a camada 1 pronta.

## Por que funciona
- **Descoberta rápida:** em 5 segundos você sabe se uma nota serve para o que precisa agora (lê só o destaque ou o resumo).
- **Esforço proporcional ao valor:** notas usadas muitas vezes ficam mais destiladas, as nunca usadas não custam nada.
- **Sem perder contexto:** a camada 1 continua lá se você precisar do detalhe.

## Diferença para a nota de literatura do Zettelkasten
| | Sumarização Progressiva | [[Notas de Literatura (Literature Notes)]] |
|---|---|---|
| Texto | Mantém palavras do autor e destaca | Reescreve com suas palavras |
| Quando | Aos poucos, quando reabre | De uma vez, logo após ler |
| Objetivo | Achar rápido o que importa | Entender e reformular |
| Resultado | Nota-fonte destilada | Ideia pronta para virar permanente |

**Combinação recomendada:** use sumarização progressiva nos highlights e, quando chegar na camada 4, transforme cada bullet do resumo numa [[Notas Permanentes (Permanent Notes)|nota permanente]]. Ver [[Setup Recomendado - O Híbrido PARA + Zettelkasten + GTD]].

## Ver também
- [[O Método CODE - Capturar Organizar Destilar Expressar]]
- [[BASB na Prática - Exemplos no Obsidian]]
