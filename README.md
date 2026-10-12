# LoyfusAnime · front

Interface em React para a [API de animes](https://github.com/loyfus/animeBackEnd):
lista dos mais populares, busca e detalhe com link de streaming.

![React](https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-F05138?style=flat-square)

Demo: [loyfus-anime-frontend.vercel.app](https://loyfus-anime-frontend.vercel.app)

## O que faz

- Lista paginada dos animes em alta
- Busca por título
- Página de detalhe com sinopse, nota e link de streaming
- Layout responsivo, com NavigationBar e rodapé

## Decisões

**CSS Modules, não Tailwind.** Cada componente tem seu próprio `.css` com
escopo automático. Num front pequeno, o arquivo ao lado do componente é mais
fácil de achar do que uma classe utilitária em outro lugar.

**A URL da API fica em um arquivo só.** `src/api/api.js` concentra o base URL,
então apontar para uma instância local ou outro ambiente é uma edição de uma
linha.

## Rodar

```bash
npm install
npm start
```

Ajuste o base URL em `src/api/api.js` para apontar para a sua instância da API.
Para gerar build de produção: `npm run build`.

## Limite de taxa

Os dados vêm do AniList, que tem limite de taxa. Respeite os
[Termos de Uso](https://anilist.co/terms).

## Stack

| | |
| --- | --- |
| Biblioteca | React 18 |
| HTTP | Axios |
| Rotas | React Router |
| Estilo | CSS Modules |
| Build | Create React App |

## Licença

MIT — [LICENSE](LICENSE).
