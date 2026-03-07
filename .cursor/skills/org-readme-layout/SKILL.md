---
name: org-readme-layout
description: Organiza o README de exibição da organização no GitHub com logo, nome, resumo e footer. Usar ao criar ou editar README.md do perfil da organização, ao estruturar o layout do readme ou quando o usuário pedir passo a passo do readme.
---

# Organização do README da Organização

Passo a passo para montar o README de exibição da organização no GitHub.

## 1. Logo (topo, centralizada)

- **Local**: `assets/logo/` (na raiz do repositório) — usar um dos arquivos:
  - nome contendo `notext` — logo sem texto (ex.: `logo-notext.jpg`, `logo-notext.png`)
  - nome contendo `text` — logo com texto (ex.: `logo-text.jpg`, `logo-text.png`)
- **Extensão**: não assumir `.png`. Verificar o conteúdo da pasta `assets/logo/` e usar o **nome completo do arquivo** (com a extensão real: `.jpg`, `.png`, `.webp`, etc.) que corresponda à escolha do usuário.
- **Estilo**: largura 200px, bordas arredondadas, centralizada.
- **Caminho no README**: o README fica em **`profile/README.md`**; a imagem fica em `assets/logo/` na raiz. Usar o caminho relativo **`../assets/logo/<nome-do-arquivo>`** no `src` da tag `<img>`.

Exemplo em Markdown (substituir `logo-text.jpg` pelo nome real do arquivo encontrado em `assets/logo/`):

```markdown
<p align="center">
  <img src="../assets/logo/logo-text.jpg" width="200" style="border-radius: 8px;" alt="ProfitAI" />
</p>
```

O usuário escolhe **notext** ou **text**; o caminho da imagem deve ser **`../assets/logo/<nome-do-arquivo>`** onde `<nome-do-arquivo>` é o arquivo real na pasta (ex.: `logo-text.jpg`, `logo-notext.png`).

## 2. Nome da organização

Logo abaixo da logo, o nome **ProfitAI** (ou o nome da organização), em destaque.

```markdown
<p align="center"><strong>ProfitAI</strong></p>
```

## 3. Linha divisória

Uma linha horizontal separando o cabeçalho do conteúdo.

```markdown
---
```

## 4. Resumo da organização

Texto explicando o que é a organização. Para a ProfitAI:

- **Foco**: restaurantes.
- **Uso do sistema**: gerenciar gastos, ver o que pode melhorar, margem de lucros.
- **Alertas**: resumo de faturamento via WhatsApp.
- **Objetivo**: o dono do restaurante saber como está indo o negócio.

Incluir também que o **desenvolvimento** é focado em IA, em especial **agentes de IA**.

Manter linguagem clara e sem dados sensíveis.

## 5. Footer

- Linha divisória acima do footer.
- Texto centralizado: **@ProfitAI 2026** (ou ano atual).
- Tudo centralizado.

```markdown
---
<p align="center">@ProfitAI 2026</p>
```

---

## Template completo

Usar esta estrutura ao montar o README em **`profile/README.md`**. O caminho da logo deve ser **`../assets/logo/<nome-do-arquivo>`** com o nome real do arquivo (ex.: `logo-notext.jpg`, `logo-text.png`). Listar a pasta `assets/logo/` para obter o nome e extensão corretos.

```markdown
<p align="center">
  <img src="../assets/logo/logo-notext.jpg" width="200" style="border-radius: 8px;" alt="ProfitAI" />
</p>

<p align="center"><strong>ProfitAI</strong></p>

---

A **ProfitAI** é focada em restaurantes. Os estabelecimentos usam nosso sistema para gerenciar gastos, identificar o que pode melhorar e acompanhar a margem de lucro. Os donos recebem alertas via WhatsApp com o resumo do faturamento, para saber como o negócio está indo.

No desenvolvimento do sistema, priorizamos o uso de **IA**, com foco em **agentes de IA**.

---

<p align="center">@ProfitAI 2026</p>
```

## Checklist antes de finalizar

- [ ] README escrito em **`profile/README.md`**. Logo referenciada com `../assets/logo/<arquivo>`; nome do arquivo verificado em `assets/logo/` (extensão real: .jpg, .png, etc., não assumir .png).
- [ ] Logo com `width="200"` e bordas arredondadas.
- [ ] Nome da organização abaixo da logo.
- [ ] Divisória entre cabeçalho e resumo.
- [ ] Resumo com foco em restaurantes, gestão, alertas WhatsApp e desenvolvimento em IA/agentes.
- [ ] Footer com divisória e "@ProfitAI 2026" centralizado.
- [ ] Nenhum dado sensível (e-mails, tokens, URLs internas, etc.).
