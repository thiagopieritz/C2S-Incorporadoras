# C2S — Design System (Incorporadoras LP)

Documento de registro da identidade visual do C2S usada na landing page "C2S Incorporadoras", consolidando os arquivos de marca recebidos. Sempre que um novo arquivo de marca for enviado, atualizar este documento.

**Fontes usadas para montar este documento:**
- `Marca C2S 2026 (1).pptx` — guia de evolução de marca (nomes, logotipo, cor, degradê)
- `Tipografia_C2S.pdf` — escala tipográfica oficial
- `Cores_C2S.pdf` — escalas de cor oficiais (Blue e Grey, com ratios de contraste WCAG)
- Logos enviadas em 24/09: `Logo_Cury.png`, `Logo_Direcional.svg`, `Logo_Plano&Plano.svg`, `Logo_RIVA.svg`, `Logo_Vibra.svg`, `Econ_logo_branco` (WebP)

---

## 1. Cor

### Escalas oficiais (fonte: `Cores_C2S.pdf`)

Escalas de acessibilidade da marca, com ratio de contraste (WCAG) já calculado contra branco e preto. `Principal` é o token de uso primário dentro da escala Blue.

**Blue**

| Token | Hex | RGB |
|---|---|---|
| blue-50 | `#E9F1FD` | 233, 241, 253 |
| blue-100 | `#BAD3F8` | 186, 211, 248 |
| blue-200 | `#98BEF5` | 152, 190, 245 |
| blue-300 | `#69A1F1` | 105, 161, 241 |
| blue-400 | `#4C8EEE` | 76, 142, 238 |
| **Principal (blue-500)** | **`#1F72EA`** | 31, 114, 234 |
| blue-600 | `#1C68D5` | 28, 104, 213 |
| blue-700 | `#1651A6` | 22, 81, 166 |
| blue-800 | `#113F81` | 17, 63, 129 |
| blue-900 | `#0D3062` | 13, 48, 98 |

**Grey**

| Token | Hex | RGB |
|---|---|---|
| grey-50 | `#E9E9E9` | 233, 233, 233 |
| grey-100 | `#BCBCBC` | 188, 188, 188 |
| grey-200 | `#9B9B9B` | 155, 155, 155 |
| grey-300 | `#6E6E6E` | 110, 110, 110 |
| grey-400 | `#515151` | 81, 81, 81 |
| grey-500 | `#262626` | 38, 38, 38 |
| grey-600 | `#232323` | 35, 35, 35 |
| grey-700 | `#1B1B1B` | 27, 27, 27 |
| grey-800 | `#151515` | 21, 21, 21 |
| grey-900 | `#101010` | 16, 16, 16 |

Aplicado na LP como `--blue-50` … `--blue-900` e `--grey-50` … `--grey-900`. Os papéis semânticos (`--ink`, `--ink-soft`, `--ink-faint`, `--line`, `--line-strong`, `--blue-mid`, `--blue-pale`) agora referenciam essa escala:

| Papel semântico | Token oficial |
|---|---|
| `--ink` (texto principal) | `grey-900` |
| `--ink-soft` (texto secundário) | `grey-400` |
| `--ink-faint` (legendas/meta) | `grey-300` |
| `--line` (borda clara) | `grey-50` |
| `--line-strong` (borda forte) | `grey-100` |
| `--blue-mid` | `blue-200` |
| `--blue-pale` | `blue-50` |

No modo escuro, a mesma escala é usada de forma invertida (`--ink: grey-50`, `--paper: grey-900`, `--blue-pale: blue-900` etc.), mantendo os dois temas na mesma fonte de verdade.

### Paleta complementar (fonte: `Marca C2S 2026.pptx`, slides 06–08)

`--blue-dark` (`#0D2A54`) e `--blue-deep` (`#0B2D5F`) **não fazem parte da escala oficial de `Cores_C2S.pdf`** — vêm do guia de evolução de marca e têm uso específico documentado (cor do nome do produto sobre fundo branco, e extremo do degradê institucional). Mantidos como tokens à parte; ver tabela abaixo.

| Token | Hex | Uso |
|---|---|---|
| Azul C2S (novo) | `#1F72EA` | Cor primária da marca. Substitui o azul antigo `#3D9BE9`. |
| Azul profundo | `#0B2D5F` | Extremo escuro do degradê institucional. |
| Azul navy | `#0D2A54` | Nome do produto sobre fundo branco (ex.: "Leads" em "C2S Leads"). |
| Azul médio | `#9AB9E4` | Tom intermediário do degradê / detalhes claros. |
| Azul claro | `#E3E9F2` | Fundo tintado / fim do degradê antes do branco. |
| Tinta (texto) | `#0E1116` | Texto principal, títulos. |
| Cinza texto | `#6B6F76` | Texto secundário / corpo. |
| Papel | `#FFFFFF` | Fundo padrão. |
| Papel alternativo | `#FAFAF7` | Fundo de seções alternadas / cards neutros. |
| Linha | `#E2E2DC` | Bordas e divisores claros. |
| Linha forte | `#B7C3D6` | Bordas sobre fundo azulado. |

**Degradê institucional** (slide 08, "Profundidade → Luz"):
`#0B2D5F → #0B48A1 → #1F72EA → #9AB9E4 → #E3E9F2 → #FFFFFF`

Usado na LP em: `--gradient: linear-gradient(135deg, #0B2D5F 0%, #0B48A1 45%, #1F72EA 80%, #4FA8E8 100%)` (hero visual e CTA final).

### Regra de aplicação do logotipo (slide 06)

| Fundo | Símbolo C2S | Nome do produto |
|---|---|---|
| Preto / escuro | Branco | `#1F72EA` |
| Branco / claro | `#1F72EA` | `#0D2A54` |

---

## 2. Tipografia

**Fonte oficial: Sora** (fonte: `Tipografia_C2S.pdf`). Uso secundário observado no PPTX: **IBM Plex Mono** para labels/eyebrows em caixa alta e **IBM Plex Sans** especificamente no wordmark "C2S" (slide 05, "Wordmark sans · IBM Plex Sans"). **Ubuntu** aparece em uso pontual no PPTX, não adotado na LP.

### Escala tipográfica oficial (`Tipografia_C2S.pdf`)

| Estilo | Font-size | Line-height | Letter-spacing |
|---|---|---|---|
| heading/h1 | 64px | 110% | 0px |
| heading/h2 | 56px | 110% | 0px |
| heading/h3 | 48px | 110% | 0px |
| heading/h4 | 40px | 110% | 0px |
| heading/h5 | 32px | 110% | 0px |
| heading/h6 | 24px | 110% | 0px |
| body/large | 18px | 150% | 0px |
| body/body | 16px | 150% | 0px |
| body/small | 14px | 150% | 0px |
| body/extra-small | 12px | 150% | 0px |

Aplicado na LP como tokens CSS (`--fs-h1` … `--fs-h6`, `--fs-body-lg` … `--fs-body-xs`), com headings em `line-height: 1.1` / `letter-spacing: 0` e corpo em `line-height: 1.5`.

Mapeamento de uso na LP:
- Hero `<h1>`: `--fs-h1` (64px no desktop, responsivo em telas menores)
- Títulos de seção (`.section-head h2`): `--fs-h3` (48px)
- Subtítulos (IA, CTA final): `--fs-h4` / `--fs-h5`
- Corpo de destaque (hero-sub, section-head p): `--fs-body-lg` (18px)
- Corpo padrão: `--fs-body` (16px)
- Legendas/metadados: `--fs-body-sm` / `--fs-body-xs`

---

## 3. Arquitetura de marca / produtos

Fonte: `Marca C2S 2026.pptx`, slides 02–04.

C2S é uma marca guarda-chuva ("casa") com três produtos, todos renomeados em 2026 para carregar o nome C2S:

| Produto | Antigo nome | Frente |
|---|---|---|
| **C2S Leads** | Gestor de Leads | Vendas — gestão de leads |
| **C2S Imob** | C2S CRM | Imóveis — gestão de imóveis |
| **C2S IA** | Vetra | Inteligência — IA no atendimento |

Essência da marca (slide 04 / 09): **simplicidade · tecnologia · resultado**.

Isso NÃO é um rebranding — é a marca amadurecendo sobre o que já é reconhecido no mercado (slide 02, decisão estratégica de fortalecer o C2S em vez de criar marcas novas).

---

## 4. Ativos de autoridade / prova social

Fonte: contexto de negócio passado pelo usuário (22/09), a confirmar formalmente antes de publicar.

- 2.000+ clientes
- 40 mil+ corretores/usuários na plataforma
- 80+ colaboradores
- Presença no Brasil e em Portugal
- Avaliação 4,8–4,9 nas lojas (App Store / Google Play)

**Incorporadoras citadas como possível prova social** (uso pendente de aprovação de marca): Cury, Direcional, Plano&Plano, Econ, Riva, Vibra, Mundo Apto.

---

## 5. Logos de clientes recebidas

Armazenadas em `scratchpad/logos/` e publicadas como arquivos do artifact (`logos/*`).

| Marca | Arquivo | Formato | Observação |
|---|---|---|---|
| Cury | `cury.png` | PNG (raster) | Único não-vetorial recebido até agora. |
| Direcional | `direcional.svg` | SVG | — |
| Plano&Plano | `planoeplano.svg` | SVG | — |
| Riva | `riva.svg` | SVG | — |
| Vibra | `vibra.svg` | SVG | — |
| Econ | `econ.webp` | WebP (raster) | Variante **branca** — precisa de fundo escuro para ficar visível (aplicado sobre chip `#0D2A54` na LP). |
| Mundo Apto | — | — | **Pendente**: arquivo ainda não enviado; LP usa texto como placeholder. |

**Uso na LP**: carrossel horizontal infinito ("marquee") na 2ª dobra, replicando a animação do site da Lais (`https://lais.ai`) — trilha duplicada, `translateX(0 → -50%)`, `linear`, loop contínuo, fade nas bordas, pausa no hover. Logos em cor original (não grayscale), todas normalizadas para a mesma caixa (128×48px, `object-fit: contain`).

⚠️ **Pendência formal**: o uso de qualquer logo, número ou case de cliente precisa de confirmação/autorização interna antes de publicação em produção (regra definida no briefing original do projeto).

---

## 6. Componentes — decisões de UI aplicadas na LP

| Componente | Especificação |
|---|---|
| Botão (`.btn`) | `border-radius: 12px`, `padding-inline: 16px`, `padding-block: 14px`, fonte Sora 600 |
| Botão pequeno (`.btn-sm`) | `padding-inline: 16px`, `padding-block: 10px` |
| Wordmark | "C2S" em IBM Plex Sans 700, cor `#1F72EA` |
| Eyebrow/label | IBM Plex Mono 500, uppercase, `letter-spacing: 0.12em` |

---

## 7. Itens em aberto (FATO × HIPÓTESE × DECISÃO)

- **FATO**: cores, degradê, tipografia (Sora) e regra de aplicação do logo — confirmados pelos arquivos de marca.
- **FATO**: números de autoridade (clientes, usuários, colaboradores, nota do app) — confirmados pelo usuário como liberados para comunicação.
- **HIPÓTESE / PENDENTE**: uso das logos de Cury, Direcional, Plano&Plano, Econ, Riva, Vibra, Mundo Apto como prova social — precisa de aprovação formal de uso de marca antes de publicar.
- **PENDENTE**: logo da Mundo Apto ainda não recebida.
- **HIPÓTESE**: posicionamento "sistema operacional da venda imobiliária" — não é decisão aprovada, não deve virar headline definitiva sem validação.
- **PENDENTE**: case/depoimento de incorporadora e indicador de resultado comprovado (tempo de 1º atendimento, % de leads distribuídos) — LP mantém placeholders `[Inserir ...]`.
