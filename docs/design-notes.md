# Design Notes — Pedro Henrique GitHub Profile

## Identidade Visual

### Paleta de Cores
| Cor | Hex | Uso |
|-----|-----|-----|
| Background Principal | `#050510` | Fundo geral |
| Background Card | `#0a0a1a` | Cards e painéis |
| Background Left Panel | `#0d0d2b` | Painel esquerdo pixel art |
| Roxo Neon | `#7b2ff7` | Bordas, acentos primários |
| Roxo Claro | `#a855f7` | Texto destaque, ícones |
| Roxo Pastel | `#c084fc` | Labels, subtítulos |
| Azul Elétrico | `#38bdf8` | Acentos secundários, tech |
| Cyan | `#06b6d4` | Database, terceiros |
| Texto Primário | `#e2e8f0` | Texto principal |
| Texto Secundário | `#94a3b8` | Texto de suporte |
| Texto Muted | `#64748b` | Texto discreto |

### Tipografia
- **Fonte principal**: `'Courier New', monospace` — para títulos e identidade
- **Badges**: `monospace` — para tech labels
- **Estilo**: Monospace para manter o look de terminal/código

### Estilo Visual
- **Pixel Art RPG** no painel esquerdo (personagem pixel art + barras de atributos)
- **Dark Cyberpunk** no layout geral (bordas neon, gradientes, elementos futuristas)
- **Cantos decorativos** com linhas neon nos quatro cantos do card
- **Divisória vertical** com gradiente roxo→azul e dots brilhantes
- **Scan lines** sutis para efeito retro-futurista
- **Floating pixels** decorativos espalhados pelo painel direito

## Arquivos Criados

| Arquivo | Tipo | Descrição |
|---------|------|-----------|
| `README.md` | Markdown | README principal do perfil |
| `assets/profile-card.svg` | SVG | Cartão principal pixel art (860×400) |
| `assets/profile-banner.svg` | SVG | Banner/footer do perfil (800×200) |
| `assets/taskflow-preview.svg` | SVG | Card de apresentação do TaskFlow (800×320) |
| `docs/design-notes.md` | Markdown | Este arquivo de anotações |

## Estrutura do README

1. **Cartão Principal** — SVG pixel art com personagem, atributos e info
2. **Sobre Mim** — Tabela + texto profissional
3. **Tech Stack** — Badges organizados por categoria (Back-End / Front-End / Database / Data / Tools)
4. **Projetos em Destaque** — Card especial TaskFlow com preview SVG
5. **GitHub Stats** — Stats card + Top Languages + Streak + Activity Graph
6. **Contato** — Botões GitHub, LinkedIn, E-mail

## Serviços Externos Utilizados
- `github-readme-stats.vercel.app` — Estatísticas do GitHub (legítimas, da conta real)
- `github-readme-streak-stats.herokuapp.com` — Streak de contribuições
- `github-readme-activity-graph.vercel.app` — Gráfico de atividade
- `img.shields.io` — Badges de tecnologias

## Notas de Compatibilidade GitHub
- Todo HTML utilizado é compatível com renderização do GitHub
- SVGs não contêm JavaScript (compatível com GitHub)
- Imagens referenciadas via caminhos relativos do repositório
- Badges via shields.io (serviço confiável e amplamente utilizado)
- Sem dependência de CSS externo ou frameworks

## Pixel Art Character
O personagem pixel art foi criado manualmente em SVG com:
- Paleta de pele (`#c8956c`, `#b07d58`)
- Cabelo escuro (`#2d1b0e`)
- Roupa em dark blue/navy (`#1a1a3e`) com acentos roxo neon (`#7b2ff7`)
- Olhos pixel (`#1a1a2e`)
- Dimensão: 8×8px por pixel, escala visual compatível

## Publicação
Para publicar no GitHub:
```bash
cd /caminho/para/pedro-henrique-silva-dev
git init
git remote add origin https://github.com/pedro-henrique-silva-dev/pedro-henrique-silva-dev.git
git add .
git commit -m "feat: add professional GitHub profile README with pixel art design"
git branch -M main
git push -u origin main
```

> O repositório especial do perfil deve ter o mesmo nome do usuário: `pedro-henrique-silva-dev`
