---
tags:
  - ZettelkastenMethod/ObsidianSetup/EssentialPlugins
category: ZettelkastenMethod/ObsidianSetup
created: 2026-08-19
---
> [!summary] Em uma frase
> Nenhum plugin é obrigatório para Zettelkasten funcionar — links + busca nativos já bastam — mas um punhado de plugins reduz fricção de captura e revisão. Este vault já vem com o trio essencial pré-instalado (`.obsidian/plugins/`), só falta habilitar em **Configurações → Plugins da comunidade**.

## Já vêm com este vault — como usar para Zettelkasten

| Plugin | Para que serve aqui |
|---|---|
| **Dataview** | Alimenta as queries de "notas órfãs" e volume por semana usadas em [[Backlinks Grafo e Descoberta de Conexões]] e [[Métricas e Revisão Periódica do Sistema]], e a tabela auto-gerada em [[Zettelkasten Method]] |
| **Templater** | Cria fleeting/literature/permanent notes com data automática — os 4 templates em `Templates/Zettelkasten - *.md` já usam a sintaxe dele (`<% tp.date.now(...) %>`); configure a pasta de templates em **Configurações → Templater → Template folder location** → `Templates` |
| **Calendar** + Daily Notes (core) | A nota diária é o lugar natural para a **inbox de fleeting notes** do dia — ver [[Fluxo de Captura - Da Ideia à Nota Permanente]] |

> [!important] Primeiro passo ao abrir este vault
> Os três plugins acima estão nos arquivos do vault mas o Obsidian pede confirmação de segurança na primeira vez — vá em **Configurações → Plugins da comunidade** e habilite os três manualmente.

## Plugins não incluídos neste vault (considere instalar depois, se sentir falta)

| Plugin (community) | Por quê |
|---|---|
| **obsidian-tasks-plugin** | Separar claramente "isso é tarefa" de "isso é conhecimento" — evita o erro descrito em [[Zettelkasten vs PARA vs GTD vs Notion]] |
| **obsidian-git** | Backup/versionamento automático — histórico de como uma nota permanente evoluiu ao longo de anos |
| **extract-highlights-plugin** | Extrair grifos de PDF/livro direto para [[Notas de Literatura (Literature Notes)]] |
| **Juggl** ou o **Grafo nativo com filtros por tag/cor** | Visualizar clusters temáticos da rede — o grafo nativo já serve, mas fica melhor com cor por tag (Configurações → Grafo → Grupos) |
| **Various Complements** / **Omnisearch** | Busca mais rápida ao decidir "com que nota antiga isso se conecta" durante a escrita |
| **Excalidraw** | Alguns praticantes fazem mapas mentais de uma MOC antes de formalizá-la em texto — opcional |

## Plugins nativos (core) do Obsidian — dois valem habilitar

- **`random-note`** (Nota aleatória) — abre uma nota qualquer do vault ao acionar. Serve como "gerador de serendipidade": abrir uma nota antiga ao acaso de vez em quando é uma técnica real usada por praticantes de Zettelkasten para redescobrir conexões esquecidas. Habilite em **Configurações → Plugins principais**.
- **`zk-prefixer`** (Zettelkasten Prefixer) — gera automaticamente um prefixo numérico/timestamp ao criar nota nova. Só vale habilitar se você decidir usar IDs (ver [[IDs Únicos e Convenção de Nomenclatura]]); do contrário, deixe desligado.

> [!tip] Não instale tudo de uma vez
> O risco real em Obsidian não é falta de plugin, é excesso de configuração virando procrastinação disfarçada de produtividade ("plugin shopping"). Comece só com o que já está instalado + `random-note` habilitado; adicione o resto só quando sentir a fricção específica que aquele plugin resolve.

## Ver também
- [[Backlinks Grafo e Descoberta de Conexões]]
- [[Fluxo de Captura - Da Ideia à Nota Permanente]]
- Templates prontos: `Templates/Zettelkasten - Fleeting Note.md`, `Templates/Zettelkasten - Literature Note.md`, `Templates/Zettelkasten - Permanent Note.md`, `Templates/Zettelkasten - MOC Template.md`
