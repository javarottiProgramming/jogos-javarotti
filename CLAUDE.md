# Instruções para agentes neste repositório

Este é o portfólio dos jogos (GitHub Pages). Leia o `README.md` antes de mexer.

## Horário das versões é sempre o de Brasília

- O objeto `HIST` do `index.html` guarda cada versão como `'AAAA-MM-DDThh:mm'` no horário de **Brasília (UTC−3)**, nunca UTC.
- Este ambiente roda em UTC. Para a hora atual de Brasília use `TZ=America/Sao_Paulo date '+%Y-%m-%dT%H:%M'`.
- Quando a hora vier de um commit, converta o horário do commit para Brasília antes de gravar.
- Brasília não tem horário de verão desde 2019: a conversão é sempre −3 h.
- Vale também para PRs de outros repositórios que atualizam a versão de um jogo.

## Atualizar a versão de um jogo

1. Copie o HTML de release para `jogos/<id>/index.html`.
2. Atualize o selo (`badge`) no `index.html`, o campo `v` no objeto `GAMES` e a tabela do `README.md`.
3. Acrescente uma linha **no topo** da lista do jogo em `HIST`, com o horário de Brasília.
