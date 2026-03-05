<div align="center">

# Página de Receitas

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

Página de receita do **Cupcake de café com chantilly**, desenvolvida como projeto da trilha FullStack da [RocketSeat](https://www.rocketseat.com.br/). O projeto original era bem simples, então aproveitei para adicionar um desafio pessoal: estilizar tudo com **Tailwind CSS** ao invés do CSS convencional.

[**Ver projeto online**](https://pagina-de-receitas-psi.vercel.app/)

</div>

---

## Preview

<div align="center">
  <img src="public/assets/main-image.png" alt="Cupcake de café com chantilly" width="420" />
</div>

---

## Sobre o Projeto

Esse projeto faz parte da trilha FullStack da **RocketSeat** e consiste em uma página de receita culinária — um **Cupcake de café com chantilly**.

Sinceramente achei bem simples, já que geralmente crio coisas mais dinâmicas, mas "dificultei" usando **Tailwind CSS** no lugar do CSS convencional pra já ir praticando a ferramenta antes de avançar pros próximos projetos mais aprofundados.

A página apresenta:

- Descrição da receita com tempo de preparo, rendimento e dificuldade
- Lista completa de ingredientes
- Modo de preparo detalhado — massa, recheio e montagem
- Design responsivo com tons quentes
- Imagem de fundo decorativa com blend de cores

---

## Stack

| Tecnologia         | Uso                               |
| ------------------ | --------------------------------- |
| **React 18**       | Construção da interface           |
| **Vite 5**         | Build tool e dev server           |
| **Tailwind CSS 4** | Estilização utility-first         |
| **Vercel**         | Deploy e hospedagem               |
| **Google Fonts**   | Tipografia (_Alice_, _Fira Code_) |

---

## O que fiz de diferente

O projeto original usava CSS convencional, mas resolvi ir além e estilizar tudo com **Tailwind CSS**, praticando classes utilitárias direto no HTML.

Alguns destaques técnicos:

- **Background com blend mode:** `bg-[url('assets/bg-image.jpg')] bg-yellow-200/10 bg-blend-multiply`
- **Tema customizado:** paleta `tcpi` definida em [`src/index.css`](src/index.css) via o bloco `@theme`
- **Responsividade:** layout adaptável com `md:py-12 md:px-60` e `md:p-24`
- **Compressão Gzip:** configurada no build via [`vite.config.js`](vite.config.js) com `vite-plugin-compression`

Que venham os próximos projetos mais aprofundados e que venha o Back.

---

## Como rodar localmente

**Pré-requisitos:** Node.js v18+ e npm ou yarn.

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/pagina-de-receitas.git

# Acesse a pasta do projeto
cd pagina-de-receitas

# Instale as dependências
npm install

# Inicie o servidor de desenvolvimento
npm run dev
```

O projeto estará disponível em `http://localhost:5378`.

### Scripts

| Comando           | Descrição                                         |
| ----------------- | ------------------------------------------------- |
| `npm run dev`     | Inicia o servidor de desenvolvimento              |
| `npm run build`   | Gera a build de produção em `/dist`               |
| `npm run preview` | Pré-visualiza a build de produção na porta `4173` |

---

## Estrutura

```
├── public/
│   └── assets/              # Imagens (background, imagem principal, favicon)
├── src/
│   ├── App.jsx              # Componente principal React
│   ├── main.jsx             # Entry point da aplicação
│   └── index.css            # Importação do Tailwind e tema customizado
├── index.html               # Página principal com a receita e classes Tailwind
├── styles.css               # Importação base do Tailwind
├── vite.config.js           # Configuração do Vite, aliases, plugins e build
├── vercel.json              # Configuração de deploy na Vercel
├── posbuild.js              # Script pós-build para limpeza de assets
├── package.json             # Dependências e scripts
└── README.md
```

---

## Paleta de cores

| Cor           | Hex                | Uso                   |
| ------------- | ------------------ | --------------------- |
| Marrom escuro | `#291B1A`          | Títulos               |
| Marrom médio  | `#573A37`          | Textos e bordas       |
| Bege dourado  | `#F6E9B2`          | Fundo do card         |
| Amarelo suave | `bg-yellow-200/10` | Overlay do background |
| Azul TCPI     | `#557AA1`          | Cor tema customizada  |

---

## Próximos passos

- [ ] Componentizar a receita em componentes reutilizáveis
- [ ] Adicionar mais receitas com navegação entre páginas
- [ ] Implementar backend com API de receitas
- [ ] Adicionar busca e filtros
- [ ] Sistema de cadastro de receitas pelo usuário

---

## Autor

**Pedro Paulo** — desenvolvido como parte da trilha FullStack da RocketSeat.

---

## Licença

Este projeto é de uso livre para fins educacionais.
