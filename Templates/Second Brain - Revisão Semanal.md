---
title: "<% tp.file.title %>"
author: Bruno De Brito
tags:
  - SecondBrain/WeeklyReview
category: SecondBrain
created: <% tp.date.now("YYYY-MM-DD") %>
---
%%
Revisão semanal integrada (GTD + PARA + BASB + Zettelkasten).
Ver "Segundo Cérebro/06 - Escolha - Melhor Padrão/Rotina Integrada - Diária Semanal Mensal.md".
Mínimo em 15 min: só as seções 1 e 2.
%%
# Revisão da semana <% tp.date.now("YYYY-[W]WW") %>

## 1. Limpar (GTD: Get Clear)
- [ ] Processar as Daily Notes da semana (tarefa → projeto, material → PARA, ideia → `#processar`)
- [ ] Zerar `0 - Inbox/`
- [ ] Zerar e-mail, downloads, anotações do celular
- [ ] Esvaziar a cabeça: o que ainda não foi capturado?

## 2. Projetos (GTD + PARA)
- [ ] Todo projeto ativo tem uma próxima ação?
```dataviewjs
for (const p of dv.pages('"1 - Projects"').where(p => p.status === "ativo")) {
  const open = p.file.tasks.where(t => !t.completed);
  dv.paragraph((open.length === 0 ? "⚠️ " : "✅ ") + p.file.link + " — " + open.length + " abertas");
}
```
- [ ] Algum projeto terminou? → checklist de fim + `4 - Archive/`
- [ ] Algum projeto novo surgiu? → criar com `Templates/Second Brain/Second Brain - Projeto.md`

## 3. Agenda e aguardando (GTD: Get Current)
- [ ] Agenda da semana passada: sobrou algo?
- [ ] Agenda das próximas 2 semanas: algo a preparar?
```tasks
not done
tags include #aguardando
```

## 4. Ideias (Zettelkasten)
- [ ] Processar notas marcadas `#processar`
- [ ] Escrever 1 a 3 notas permanentes
- [ ] Linkar notas órfãs
- [ ] Abrir 2 notas aleatórias: conecta com algo desta semana?

## 5. Destilar (BASB)
- [ ] Uma nota de livro/curso usada esta semana ganha mais uma camada (negrito → destaque → resumo)

## 6. Criativo (GTD: Get Creative)
- [ ] Revisar "algum dia/talvez"
- [ ] Ideias novas:
  - 

## Notas da semana
- O que funcionou:
- O que travou:
