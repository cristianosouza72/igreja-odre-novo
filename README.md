# Site — Igreja Batista Odre Novo

Site estático (HTML + CSS + JS puros). Não precisa de instalação: basta abrir `index.html` no navegador.

```
index.html      página única com todas as seções
css/style.css   estilos (cores no topo do arquivo, em :root)
js/main.js      menu mobile, cabeçalho ao rolar, animações, ano do rodapé
assets/         logo, fotos e favicon (veja assets/LEIA-ME.txt)
```

## 1. Preencher os dados que faltam

Todos os campos a preencher estão entre colchetes. Para listá-los:

```sh
grep -n "\[" index.html
```

| Placeholder | Onde aparece |
|---|---|
| `[NOME DO PASTOR]` e texto de apresentação | seção Liderança |
| `[DDD][NUMERO]` | link do WhatsApp, só dígitos, ex.: `https://wa.me/5511999998888` |
| `([DDD]) [NÚMERO]` | número exibido no cartão do WhatsApp |
| `[EMAIL]` | cartão de e-mail (aparece 2 vezes) |
| `[URL DO SITE]` | dados estruturados, depois de publicar |

Textos de Missão, Visão, Valores e Ministérios também podem ser ajustados livremente em `index.html`.

## 2. Imagens

Coloque as imagens em `assets/` com os nomes indicados em `assets/LEIA-ME.txt`. Tudo funciona mesmo sem elas.

## 3. Cores

Edite as variáveis no início de `css/style.css` (`--wine`, `--gold`, `--cream` etc.).

## 4. Publicar (grátis)

- **Netlify Drop**: acesse app.netlify.com/drop e arraste a pasta `site-on`.
- **GitHub Pages**: crie um repositório, envie os arquivos e ative Pages em *Settings → Pages*.
- **Cloudflare Pages / Vercel**: importe a pasta como site estático, sem comando de build.
