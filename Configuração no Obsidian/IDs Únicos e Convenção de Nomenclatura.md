---
tags:
  - ZettelkastenMethod/ObsidianSetup/UniqueIDsNaming
category: ZettelkastenMethod/ObsidianSetup
created: 2026-08-19
---
> [!summary] Em uma frase
> Luhmann precisava de IDs alfanuméricos (`21a3`) porque fichas de papel não têm busca nem link automático. No Obsidian isso é resolvido pelo próprio nome do arquivo + wikilink — então **use IDs só se você tiver um motivo concreto**, não por tradição.

## Por que Luhmann precisava de ID e você provavelmente não precisa

O ID físico resolvia dois problemas que não existem em texto digital:
1. **Posição física** — em papel, a ficha precisa estar em algum lugar fisicamente; o ID definia isso.
2. **Referência estável** — sem busca full-text, o único jeito de apontar "veja a nota tal" era por um código.

No Obsidian, o **título do arquivo já é o identificador único**, a busca é instantânea, e o link `[[Nome da Nota]]` sobrevive a renomeação (o Obsidian atualiza os links automaticamente ao renomear um arquivo). Ou seja: os dois problemas que o ID resolvia já estão resolvidos por recursos nativos do app.

## Quando usar ID mesmo assim

- **Zettelkasten "folgezettel"** (sequência de notas que devem ser lidas em ordem, tipo uma trilha de raciocínio) — um prefixo tipo `1.1`, `1.2`, `1.2a` no início do nome do arquivo comunica ordem de leitura de um jeito que puro link não comunica.
- **Times/vaults compartilhados** onde nomes de nota podem colidir ou mudar de forma imprevisível e você quer uma referência estável independente do título.
- Preferência estética/histórica pessoal — válido, mas é escolha de estilo, não necessidade técnica.

Se nenhum desses casos se aplica, **pule o ID** e use só o título-frase (ver [[Notas Permanentes (Permanent Notes)]]) como nome de arquivo — é mais legível no grafo, na busca e nos backlinks.

## Convenção recomendada para nomes de arquivo neste vault

- **Nome do arquivo = título-frase da ideia**, sem prefixo numérico. Ex: `Fricção na captura elimina ideias antes de serem avaliadas.md`.
- Evite nomes genéricos (`Ideia 1.md`, `Nota sobre produtividade.md`) — o nome do arquivo é o que aparece no link, na busca e no grafo; ele precisa carregar significado sozinho.
- `tags` hierárquica PascalCase (`ZettelkastenMethod/Fundamentals/CorePrinciples`) + `category` = a mesma tag sem o último segmento — é a convenção já usada em todas as notas deste vault; mantenha-a ao criar notas novas em vez de inventar um esquema paralelo.

## Sobre unlinked mentions e aliases

Se duas notas usam frases um pouco diferentes para a mesma ideia (ex: "Atomicidade" vs "uma nota, uma ideia"), use o campo `aliases` no frontmatter do Obsidian para que ambos os termos resolvam para a mesma nota, e cheque periodicamente o painel **"Unlinked Mentions"** (menções não linkadas) no final de cada nota — ele mostra onde o título da nota aparece em texto solto no vault sem ter virado link, um jeito rápido de achar conexões perdidas.

## Ver também
- [[Estrutura Pastas vs Tags vs Links]]
- [[Backlinks Grafo e Descoberta de Conexões]]
- [[Niklas Luhmann e a História do Método]]
