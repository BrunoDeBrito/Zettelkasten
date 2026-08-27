---
tags:
  - ZettelkastenMethod/Strategy/MetricsAndReview
category: ZettelkastenMethod/Strategy
created: 2026-08-19
---
> [!summary] Em uma frase
> Meça a saúde do Zettelkasten pela densidade de conexão da rede, não pelo número total de notas — um vault com 200 notas bem linkadas vale mais que um com 2000 notas órfãs.

## Métricas que importam

| Métrica | Como medir (Dataview) | O que indica |
|---|---|---|
| **% de notas órfãs** (sem link de saída) | Query abaixo | Alta % = capturando sem processar de verdade (ver [[Erros Comuns e Como Evitá-los]] #6) |
| **Média de links por nota** | Contar `file.outlinks` por nota | Abaixo de 2 sugere notas isoladas; não existe número "certo", mas tendência de queda ao longo do tempo é sinal de alerta |
| **Notas permanentes criadas por semana** | Contar arquivos criados na pasta, por `created` | Serve para ver consistência de rotina (ver [[Como Manter o Hábito a Longo Prazo]]), não para maximizar |
| **Idade média das MOCs sem atualização** | Comparar `created`/última edição das MOCs vs. notas permanentes novas linkadas a elas | MOC muito desatualizada em relação ao conteúdo novo é sinal de revisar a estrutura |

## Query Dataview para notas órfãs (saída zero)

```dataview
TABLE length(file.outlinks) AS "Links de saída"
FROM "" AND -"Templates"
WHERE length(file.outlinks) = 0
SORT file.name ASC
```

## Query Dataview para volume por semana

```dataview
TABLE created
FROM "" AND -"Templates"
SORT created DESC
```

## Cadência de revisão recomendada

- **Semanal:** operacional — processar inbox, checar órfãs recentes (já coberto em [[Rotina Diária e Semanal de Manutenção]]).
- **Trimestral:** estrutural — rodar as queries acima, ler 3–5 notas antigas ao acaso e avaliar se ainda representam bem o que você pensa hoje (atualizar se não), revisar se alguma tag/categoria parou de fazer sentido.
- **Anual:** estratégica — perguntar se o sistema está de fato sendo usado nos três casos de [[Do Zettelkasten à Criação - Escrita Estudo e Decisões]] (escrita, estudo, decisão). Se não está sendo usado para nenhum output há um ano, vale revisar se o esforço de manutenção está proporcional ao valor extraído.

## O que NÃO otimizar

- **Número total de notas** — não é uma métrica de qualidade, só de volume.
- **Perfeição retroativa** — não é preciso "corrigir" todas as notas antigas toda vez que o padrão evolui; aplique o padrão novo para frente e ajuste as antigas só quando for revisitá-las naturalmente.
- **Cobertura de assunto** — o Zettelkasten não precisa (e não deveria tentar) cobrir todo assunto que você já estudou; ele cresce em torno do que você realmente processa, não do que você "deveria" ter processado.

## Ver também
- [[Backlinks Grafo e Descoberta de Conexões]]
- [[Erros Comuns e Como Evitá-los]]
- [[Como Manter o Hábito a Longo Prazo]]
