---
description: Gera o README de exibição da organização no GitHub seguindo layout e regras do projeto
---

Use o subagente **github-org-readme** e a skill **org-readme-layout** para gerar o README da organização.

**Antes de gerar:**
1. Pergunte ao usuário qual logo usar: **notext** (logo sem texto) ou **text** (logo com texto). As opções ficam em `assets/logo/`.
2. Se o usuário já tiver informado a escolha, use direto.
3. **Nome do arquivo da logo:** listar o conteúdo de `assets/logo/` e identificar o arquivo que corresponda à escolha (ex.: se escolheu "text", usar o arquivo cujo nome contém "text", como `logo-text.jpg` ou `logo-text.png`). Usar sempre o **nome completo do arquivo com a extensão real** (`.jpg`, `.png`, `.webp`, etc.) no `src` da imagem no README — não assumir `.png`.

**Ao gerar:**
- Siga o passo a passo da skill org-readme-layout (logo centralizada 200px, nome da organização, divisória, resumo, footer).
- Respeite a regra org-readme-github: nenhum dado sensível, só conteúdo público.
- Escreva o conteúdo em `README.md` (ou no arquivo que for o README de exibição da organização).

**Depois de gerar:**
- Confirme que o checklist da regra e da skill foi atendido (logo, estrutura, sem dados sensíveis).
