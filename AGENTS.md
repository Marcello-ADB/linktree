# Linktree

Siga primeiro as instruções compartilhadas em `../AGENTS.md`.

Página de links própria (alternativa caseira ao Linktree). Referência de layout, tema e conteúdo de exemplo: `linktr.ee/pecattosp_` (Pecatto Bar e Restaurante). Repositório público `Marcello-ADB/linktree` (conta particular do GitHub).

## Comandos

Sem build, dependências ou suíte de testes. Para visualizar, abra `index.html` no navegador (funciona via `file://`). Publicação: GitHub Pages servindo a raiz da branch `main` em https://marcello-adb.github.io/linktree/; todo push na `main` publica. O push usa a conta ativa do `gh`, que deve ser `Marcello-ADB` (`gh auth switch -u Marcello-ADB`).

## Arquitetura

- `index.html` é a página inteira: CSS embutido, sem JavaScript. Ícones Tabler (MIT) em SVG inline; fonte Manrope via Google Fonts.
- Tema: as quatro variáveis em `:root` (`--bg`, `--text`, `--button`, `--button-text`) reproduzem o tema da referência.
- Cada link é um `<a class="link">` com SVG + texto dentro de `.links`. Grupo com título (o "group" do Linktree) é um `<section>` com `<h2>`.
- O `div.avatar` com a inicial é provisório; trocar por `<img class="avatar">` quando houver logo.

## Conteúdo

A página é do Pecatto (confirmado em 2026-11-18). Links copiados da referência nessa data, com três correções: WhatsApp com DDI 55 (o original estava sem), delivery em `https` e reservas apontando direto para o widget TagMe (o original passava por um segundo Linktree, `linktr.ee/pecattorestaurante`). O número do WhatsApp com DDI ainda não foi confirmado com o restaurante.
