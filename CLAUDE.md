# CLAUDE.md — GUYRESTAURANTE

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** GUYRESTAURANTE
**Nicho:** Gastronomia
**Keywords:** Bem vindo ao restaurante GUY Nossos chefs de cozinha sao especialistas em
**Paleta de cores:** slate | **Fonte:** lora

Bem vindo ao restaurante GUY Nossos chefs de cozinha são especialistas em transformar ingredientes frescos e saborosos em pratos deliciosos. Com anos de experiência em cozinhas de todo o mundo, nossos chefs trazem uma abordagem única para cada refeição que preparam. Eles combinam técnicas clássicas com novas ideias culinárias para criar pratos únicos e memoráveis que irão encantar seus paladares. Nossos chefs são verdadeiros mestres em suas áreas de especialização, sejam elas culinária internacional, pratos vegetarianos ou opções veganas.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-J |
| Hero | Hero-E |
| Features | Features-D |
| About Section | About-G |
| Posts | Posts-D |
| Footer | Footer-A |
| Página Sobre | Sobre-I |
| Página Contato | Contato-A |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
