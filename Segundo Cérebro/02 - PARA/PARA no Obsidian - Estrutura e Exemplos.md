---
title: "PARA no Obsidian - Estrutura e Exemplos"
author: Bruno De Brito
tags:
  - SecondBrain/PARA/ObsidianSetup
category: SecondBrain/PARA
created: 2026-10-13
---
> [!info] Contexto desta nota
> Copiada do vault `SecondBrainObsidian` em 2026-11-02. Onde aparecem "este vault" e caminhos como `1 - Projects/`, a nota descreve aquele vault, não este.

> [!summary] Em uma frase
> No Obsidian, PARA vira **4 pastas numeradas na raiz** (mais uma Inbox), com no máximo 2 níveis abaixo. O resto da organização fica por conta de links, tags e Dataview.

## Estrutura padrão
```
0 - Inbox/
1 - Projects/
    Candidatura Stripe/
    Vídeo Docker/
2 - Areas/
    Carreira/
    Finanças/
    Saúde/
    Vida Espiritual/
    YouTube Channel/
3 - Resources/
    Livros/
    Cursos/
    Programação/
    Templates/
4 - Archive/
    2026/
```

## Convenções de formato
- **Números na frente** (`1 - Projects`) para forçar a ordem P-A-R-A no explorador.
- **Um projeto = uma pasta** (ou uma nota, se for pequeno).
- **Campo `status`** em notas de projeto: `ativo`, `pausado`, `concluído`, `cancelado`.
- **Campo `deadline`** em projetos (tipo `date`).
- **Arquivo por ano** (`4 - Archive/2026/`) facilita achar depois.

## Exemplo: nota-índice de projeto
```markdown
---
title: "Candidatura Stripe"
tags:
  - Projects/StripeApplication
category: Projects
status: ativo
deadline: 2026-11-15
area: "[[Carreira]]"
---
> [!summary] Objetivo
> Enviar candidatura completa para a vaga Backend Engineer e chegar à entrevista técnica.

## Material
- [[appl]]: checklist de currículo
- [[Trimodal Nature of Tech Compensation Revisited]]: faixa salarial de referência

## Próximas ações
- [ ] Ajustar currículo para a vaga 📅 2026-10-20
- [ ] Pedir indicação no LinkedIn 📅 2026-10-22

## Log
- 2026-10-13: projeto criado
```

## Exemplo: nota-índice de área
````markdown
---
title: "Carreira"
tags:
  - Areas/Career
category: Areas
---
> [!summary] Padrão a manter
> Currículo atualizado a cada 3 meses. 1 curso ativo. Inglês diário.

## Projetos ativos desta área
```dataview
LIST FROM "1 - Projects" WHERE area = [[Carreira]] AND status = "ativo"
```
````

## Exemplo: painel geral (Home)
````markdown
## Projetos ativos
```dataview
TABLE deadline, area FROM "1 - Projects"
WHERE status = "ativo" SORT deadline ASC
```

## Projetos parados há mais de 30 dias
```dataview
LIST FROM "1 - Projects"
WHERE status = "ativo" AND file.mtime < date(today) - dur(30 days)
```
````

## Como fica com as convenções deste vault
Este vault usa tags hierárquicas em inglês e `category` (ver [[Vault Meta]]). Em PARA, a convenção natural é: primeiro segmento da tag = categoria PARA (`Projects/...`, `Areas/...`, `Resources/...`). Uma proposta concreta de migração das pastas atuais está em [[Como Aplicar Neste Vault - Plano de Migração]].

## Ver também
- [[Manutenção e Revisão do PARA]]
- [[BASB na Prática - Exemplos no Obsidian]]
- [[ACE - Atlas Calendar Efforts]]: uma alternativa de pastas pensada para Obsidian
