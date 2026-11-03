---
title: "Como Aplicar Neste Vault - Plano de Migração"
author: Bruno De Brito
tags:
  - SecondBrain/Choice/MigrationPlan
category: SecondBrain/Choice
created: 2026-10-13
---
> [!info] Contexto desta nota
> Copiada do vault `SecondBrainObsidian` em 2026-11-02. Onde aparecem "este vault" e caminhos como `1 - Projects/`, a nota descreve aquele vault, não este.

> [!summary] Em uma frase
> Registro da migração do vault para o [[Setup Recomendado - O Híbrido PARA + Zettelkasten + GTD|setup híbrido]], **executada em 2026-10-13**: o que foi movido, o que foi ajustado para nada quebrar e o que ainda depende de você.

## Como ficou
```
0 - Inbox/              ← daily notes + capturas (inbox única)
1 - Projects/           ← Projects.md (painel) + um arquivo por projeto
2 - Areas/
    Routine/
    Spiritual Life/     ← Biblical Year/ + Sabbath School Lesson/
    YouTube Channel/
3 - Resources/
    Clippings/  Courses/  IA/  Learn/
    Library and Highlights/
    Second Brain/       ← 00 - Zettelkasten/ (manual do método) + 01 a 06
4 - Archive/            ← vazio por enquanto
Zettelkasten/           ← SUAS notas permanentes (+ Literatura/), FORA do PARA
Map/  Templates/  Vault Meta/  Basics.md  README.md   ← sistema
```

## O que foi movido
| Antes | Depois |
|---|---|
| `Zettelkasten/Inbox/` | `0 - Inbox/` |
| `Routine/` | `2 - Areas/Routine/` |
| `YouTube Channel/` | `2 - Areas/YouTube Channel/` |
| `Biblical Year/` | `2 - Areas/Spiritual Life/Biblical Year/` |
| `Sabbath School Lesson/` | `2 - Areas/Spiritual Life/Sabbath School Lesson/` |
| `Courses/`, `Learn/`, `Library and Highlights/`, `Clippings/`, `IA/`, `Second Brain/` | `3 - Resources/...` (mesmo nome) |
| `Zettelkasten/` (documentação do método) | `3 - Resources/Second Brain/00 - Zettelkasten/` (2ª passada, mesmo dia) |
| *(nova)* | `Zettelkasten/` na raiz, só para as suas notas: [[Rede de Ideias]] |

Feito com `git mv` (o histórico de cada arquivo foi preservado). Há um commit de segurança imediatamente antes da migração ("vault backup: antes da migração para PARA"), caso precise voltar.

## O que foi ajustado para nada quebrar
- **Links `[[...]]`:** nenhum precisou mudar. O Obsidian resolve pelo nome do arquivo, não pela pasta.
- **Consultas Dataview com caminho fixo:** atualizadas em `Biblical Year.md`, `Clippings.md`, `Youtube Learn Programming.md`, `Design Pattern.md` e `Second Brain.md`. Os índices com o bloco `dataviewjs` genérico detectam a própria pasta e não precisaram de ajuste.
- **`Book view.base`:** filtros de pasta atualizados.
- **Plugins:** Kindle (pasta de highlights), Book Search (pasta de livros), Daily Notes (agora cria em `0 - Inbox/`) e Icon Folder (ícones seguiram as pastas; as pastas novas ganharam ícones).
- **Tags e `category`: não mudaram.** A tag segue o **assunto** e a pasta segue a **ação**. É a ideia do PARA: mover uma nota de Recursos para o Arquivo não muda do que ela trata.

## O que depende de você
Está como próximas ações em [[Implantar o Segundo Cérebro]]:
- [ ] **Obsidian Web Clipper** (extensão do navegador): mudar a pasta de destino de `Clippings` para `3 - Resources/Clippings`. Senão ele recria `Clippings/` na raiz.
- [ ] Criar uma nota de projeto para cada coisa com prazo em andamento.
- [ ] Preencher o "padrão a manter" de cada área em [[Areas]].

## Regras daqui para frente
- **Mova arquivos pelo Obsidian** (arrastar ou "Move file to..."), não pelo gerenciador de arquivos.
- Ao criar consulta Dataview, prefira `WHERE file.folder = this.file.folder` a caminho fixo.
- Projeto concluído → `4 - Archive/2026/`.

## Ver também
- [[PARA no Obsidian - Estrutura e Exemplos]]
- [[Rotina Integrada - Diária Semanal Mensal]]
