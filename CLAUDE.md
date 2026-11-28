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

## Pull Request: SEMPRE pela skill `PullRequest_Description` (regra do Pedro, reforçada em 2026-11-28)
- Para **escrever, descrever ou abrir** qualquer PR (jogo, portfólio, Persona, qualquer repositório), seguir a skill `PullRequest_Description`: `perfil/skills/PullRequest_Description/SKILL.md` no repositório `claude-code-persona`. **Em sessão em nuvem a skill pode não aparecer na lista: leia o arquivo antes de escrever o corpo.** Nunca inventar formato próprio.
- **Formato ESTILIZADO** (padrão, não perguntar): `🎯 Contexto` · `✅ O que entra` (por área, sem nome de arquivo) · `🐛 Bugs pré-existentes` (se houver) · `🔧 Decisões` · `✔️ Validação` · rodapé `🤖 Gerado com [Claude Code](https://claude.com/claude-code)` + URL da sessão. PR referenciado como `PR 123`, sem `#`. Título curto que resuma a entrega.
- **Mostrar o corpo completo ao Pedro e esperar o OK antes de abrir** (e a mensagem de commit antes de commitar, em pt-BR e amigável). Branch de feature, nunca `main`; nunca merge; nunca `--force`. Trailer do commit sem nome de modelo: `Co-Authored-By: Claude <noreply@anthropic.com>` e `Claude-Session: <URL>`.
- **O PR sai com corpo e conferido depois de criado** (corpo não pode ficar vazio nem curto). Texto público de jogo (README, PR, portfólio) nunca cita outros jogos.
