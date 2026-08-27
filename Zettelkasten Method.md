---
tags:
  - ZettelkastenMethod/Index
category: ZettelkastenMethod
created: 2026-08-19
---
> [!summary] Sobre
> MOC (Map of Content) do método Zettelkasten aplicado neste vault com Obsidian — teoria completa, tipos de nota, configuração prática e um modelo de uso (rotina + fluxo de captura). Comece por [[O que é Zettelkasten]] se for a primeira leitura.

## Fundamentos (teoria e princípios)
- [[O que é Zettelkasten]] — definição e mecanismo central
- [[Niklas Luhmann e a História do Método]] — origem, o sistema físico original
- [[Princípios Fundamentais do Zettelkasten]] — os 5 princípios que sustentam tudo
- [[Zettelkasten vs PARA vs GTD vs Notion]] — como isso se encaixa (ou não) com outros métodos

## Tipos de Nota (o vocabulário operacional)
- [[Notas Fugazes (Fleeting Notes)]] — captura rápida e descartável
- [[Notas de Literatura (Literature Notes)]] — resumo de uma fonte, com suas palavras
- [[Notas Permanentes (Permanent Notes)]] — a unidade de valor do sistema
- [[Notas Estruturais e MOCs]] — pontos de entrada que emergem depois do conteúdo

## Configuração no Obsidian (a parte técnica)
- [[Estrutura Pastas vs Tags vs Links]] — por que link é o mecanismo primário
- [[IDs Únicos e Convenção de Nomenclatura]] — quando (não) usar IDs no digital
- [[Plugins Essenciais para Zettelkasten no Obsidian]] — o que já está instalado e o que falta
- [[Backlinks Grafo e Descoberta de Conexões]] — como usar os painéis nativos

## Fluxo de Trabalho — o Modelo de Uso
- [[Fluxo de Captura - Da Ideia à Nota Permanente]] — o funil de 4 estágios completo
- [[Rotina Diária e Semanal de Manutenção]] — quando fazer cada parte, na prática
- [[Como Escrever uma Boa Nota Permanente]] — checklist passo a passo
- [[Do Zettelkasten à Criação - Escrita Estudo e Decisões]] — os 3 usos práticos: escrever, estudar, decidir

## Estratégia (sustentar o sistema no longo prazo)
- [[Erros Comuns e Como Evitá-los]] — os 7 erros que matam a maioria dos Zettelkasten
- [[Como Manter o Hábito a Longo Prazo]] — a curva de valor atrasada e como não desistir antes dela
- [[Métricas e Revisão Periódica do Sistema]] — o que medir (e o que não medir)

## Templates prontos (`Templates/`)
- `Zettelkasten - Fleeting Note.md`
- `Zettelkasten - Literature Note.md`
- `Zettelkasten - Permanent Note.md`
- `Zettelkasten - MOC Template.md`

## Por onde começar, na prática

1. Leia [[O que é Zettelkasten]] e [[Princípios Fundamentais do Zettelkasten]] (10 min).
2. Habilite o plugin nativo `random-note` (ver [[Plugins Essenciais para Zettelkasten no Obsidian]]).
3. Comece a rotina diária de captura descrita em [[Rotina Diária e Semanal de Manutenção]] — só isso, por 1–2 semanas, sem se cobrar notas permanentes ainda.
4. Depois de ter algumas fleeting notes acumuladas, processe a primeira usando [[Como Escrever uma Boa Nota Permanente]] como checklist.

## Todas as notas desta pasta (auto-gerado)

```dataview
TABLE category AS "Categoria"
FROM "" AND -"Templates"
WHERE file.name != "Zettelkasten Method"
SORT category ASC, file.name ASC
```
