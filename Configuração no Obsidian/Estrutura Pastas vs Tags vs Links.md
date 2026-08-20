---
tags:
  - ZettelkastenMethod/ObsidianSetup/FoldersTagsLinks
category: ZettelkastenMethod/ObsidianSetup
created: 2026-08-19
---
> [!summary] Em uma frase
> No Zettelkasten, **links** (`[[wikilink]]`) fazem o trabalho estrutural principal; **tags** classificam por dimensão transversal (tipo, status, projeto); e **pastas** são só um detalhe de organização de arquivo no disco, sem peso conceitual — nunca o mecanismo primário de conexão.

## Por que link > pasta > tag nessa ordem, no Zettelkasten

Uma nota só pode estar em **uma** pasta, mas uma ideia real se conecta a N outras ideias em N "dimensões" diferentes. Forçar hierarquia de pasta obriga você a escolher uma única categoria "principal" para cada nota — o que é exatamente o problema que o método existe para resolver (ver [[O que é Zettelkasten]]).

| Mecanismo | Cardinalidade | Papel no Zettelkasten |
|---|---|---|
| Pasta | 1 nota → 1 pasta | Organização física opcional, zero peso conceitual |
| Tag | 1 nota → N tags | Classificação transversal leve (tipo de nota, status, projeto) |
| Link `[[ ]]` | 1 nota → N notas, bidirecional via backlink | **O mecanismo estrutural real** — é o que forma a rede |

## A convenção de tags usada neste vault

Todas as notas deste vault usam tags hierárquicas PascalCase (ex: `ZettelkastenMethod/Fundamentals/CorePrinciples`) + `category` = a mesma tag sem o último segmento. Isso funciona bem como classificação leve porque cada nota tem um tema "dono" natural — mas repare que é só isso, classificação; quem conecta as ideias de verdade continua sendo os wikilinks dentro do corpo de cada nota, não a tag.

Para as **notas permanentes do Zettelkasten**, a mesma convenção de tag continua útil como classificação leve (ex: `ZettelkastenMethod/NoteTypes/PermanentNotes` neste próprio arquivo), mas o que efetivamente conecta as ideias entre si são os links dentro do corpo da nota (seção `## Ver também` e links inline), não a tag. Duas notas com a mesma tag não estão necessariamente relacionadas; duas notas linkadas estão, por definição.

## Pastas: use para navegação de arquivo, não para significado

Esta própria pasta (`Zettelkasten Method/Fundamentos/`, `.../Tipos de Notas/`, etc.) existe só para não deixar 20 arquivos soltos numa pasta só e facilitar navegar pelo explorador de arquivos do Obsidian. Ela **não** define a rede de ideias — quem faz isso são os wikilinks dentro de cada nota. Uma alternativa igualmente válida (e mais "pura" ao método original) seria colocar todas as notas permanentes numa única pasta flat e deixar 100% do trabalho de organização para tags + links + grafo.

> [!tip] Se o vault crescer muito
> Pastas ajudam performance de busca/visualização em vaults com milhares de notas. Não é contraindicação usar pastas — só não deixe a pasta virar decisão sobre "para que serve" a nota.

## Ver também
- [[IDs Únicos e Convenção de Nomenclatura]]
- [[Backlinks Grafo e Descoberta de Conexões]]
- [[Notas Estruturais e MOCs]]
