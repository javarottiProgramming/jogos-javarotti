# Jogos do Javarotti 🎮

Portfólio rápido dos jogos do Pedro Javarotti: um painel para escolher o jogo e jogar direto no navegador (GitHub Pages).

| Jogo | Versão | Pasta |
|---|---|---|
| **Kuku e a Semente do Sol** (plataforma 2D) | 2.8 | `jogos/kuku/` |
| **Pedrada de Palito** (FPS de estilingue) | 1.0.7 | `jogos/pedrada/` |

Cada jogo é **um único arquivo HTML** (o `releases/*.html` do repositório original), copiado sem alteração para `jogos/<id>/index.html`.
Os códigos-fonte continuam nos repositórios dos próprios jogos.

## Como atualizar um jogo
Copie o novo HTML de release por cima de `jogos/<id>/index.html`, ajuste a versão no `badge` do `index.html` e faça push na `main`.

## Como adicionar um jogo novo
1. `jogos/<id>/index.html` com o HTML do jogo.
2. `assets/<id>.jpg` com a capa (960×540).
3. Um `<article class="game">` novo no `index.html` (copie um dos dois) e uma linha no objeto `GAMES` do script.

## Publicação
GitHub Pages, fonte: branch `main`, pasta `/ (root)`. Sem build.

## Fontes
`fonts/` guarda Permanent Marker, Lilita One e Nunito (todas SIL OFL), servidas pelo próprio site, sem depender do Google Fonts.
Os textos sobre o Pedro e o time estão no `index.html`; edite lá.
