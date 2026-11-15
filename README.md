# Jogos do Javarotti 🎮

Portfólio rápido dos jogos do Pedro Javarotti: um painel para escolher o jogo e jogar direto no navegador (GitHub Pages).

| Jogo | Versão | Pasta |
|---|---|---|
| **Kuku e a Semente do Sol** (plataforma 2D) | 2.8 | `jogos/kuku/` |
| **Pedrada de Palito** (FPS de estilingue) | 1.1.5 | `jogos/pedrada/` |
| **Cacos de Sol** (RPG de ação 3D) | 1.0.3 | `jogos/cacos-de-sol/` |
| **Java's Brick** (quebra-tijolos) | 1.0.15 | `jogos/javas-brick/` |

Cada jogo é **um único arquivo HTML** (o `releases/*.html` do repositório original), copiado sem alteração para `jogos/<id>/index.html`.
Os códigos-fonte continuam nos repositórios dos próprios jogos.

## Como atualizar um jogo
Copie o novo HTML de release por cima de `jogos/<id>/index.html`, ajuste a versão no `badge` do `index.html` e faça push na `main`.

## Como adicionar um jogo novo
1. `jogos/<id>/index.html` com o HTML do jogo.
2. `assets/<id>.jpg` com a capa (960×540).
3. Um `<article class="game">` novo no `index.html` (copie um dos dois) e uma linha no objeto `GAMES` do script.

## Ligar e desligar o link
O site só vai ao ar quando você manda, pelo workflow **Ligar ou desligar o site**:

1. Uma vez só: Settings → Pages → Source: **GitHub Actions**.
2. Aba **Actions** → *Ligar ou desligar o site* → **Run workflow** → escolha `ligar` ou `desligar`.
   Funciona também pelo app do GitHub no celular.

`ligar` publica o portfólio e os jogos. `desligar` publica só `fora-do-ar.html`, e os jogos saem do ar em 1 ou 2 minutos
(cópias em cache podem durar um pouco mais). Mudar o conteúdo do repositório **não** liga o site sozinho.

Atenção: o repositório é público, então os arquivos dos jogos continuam visíveis em `jogos/` mesmo com o link desligado.
Só um repositório privado esconderia isso.

## Fontes
`fonts/` guarda Permanent Marker, Lilita One e Nunito (todas SIL OFL), servidas pelo próprio site, sem depender do Google Fonts.
Os textos sobre o Pedro e o time estão no `index.html`; edite lá.
