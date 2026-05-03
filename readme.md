<div align="center">

# Recipes Page

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

Recipe page for a **Coffee Cupcake with Whipped Cream**, developed as a project from the [RocketSeat](https://www.rocketseat.com.br/) FullStack track. The original project was quite simple, so I took it as a personal challenge: style everything with **Tailwind CSS** instead of conventional CSS.

[**View live project**](https://pagina-de-receitas-psi.vercel.app/)

</div>

---

## Quick Description

Front-end project of a culinary recipe page, focused on visual layout, content organization and responsiveness. The app presents the **Coffee Cupcake with Whipped Cream** recipe, including ingredients, preparation time, yield, difficulty and step-by-step instructions.

Built with **React** and **Vite**, styled with **Tailwind CSS** and deployed on **Vercel**. The main goal was to practice building modern and semantic interfaces, while reinforcing utility-first styling concepts and front-end project structuring.

---

## Preview

<div align="center">
  <img src="public/assets/main-image.png" alt="Coffee cupcake with whipped cream" width="420" />
</div>

---

## About the Project

This project is part of the **RocketSeat** FullStack track and consists of a culinary recipe page — a **Coffee Cupcake with Whipped Cream**.

Honestly, I found it quite simple since I usually build more dynamic things, but I made it harder for myself by using **Tailwind CSS** instead of conventional CSS to practice the tool before moving on to more advanced projects.

The page features:

- Recipe description with preparation time, yield and difficulty
- Full ingredients list
- Detailed preparation method — batter, filling and assembly
- Responsive design with warm tones
- Decorative background image with color blend

---

## Stack

| Technology         | Usage                             |
| ------------------ | --------------------------------- |
| **React 18**       | UI building                       |
| **Vite 5**         | Build tool and dev server         |
| **Tailwind CSS 4** | Utility-first styling             |
| **Vercel**         | Deploy and hosting                |
| **Google Fonts**   | Typography (_Alice_, _Fira Code_) |

---

## What I did differently

The original project used conventional CSS, but I went further and styled everything with **Tailwind CSS**, practicing utility classes directly in the HTML.

Some technical highlights:

- **Background with blend mode:** `bg-[url('assets/bg-image.jpg')] bg-yellow-200/10 bg-blend-multiply`
- **Custom theme:** `tcpi` palette defined in [`src/index.css`](src/index.css) via the `@theme` block
- **Responsiveness:** adaptive layout with `md:py-12 md:px-60` and `md:p-24`
- **Gzip compression:** configured in the build via [`vite.config.js`](vite.config.js) with `vite-plugin-compression`

Bring on the next, more advanced projects — and bring on the Back-end.

---

## Running locally

**Prerequisites:** Node.js v18+ and npm or yarn.

```bash
# Clone the repository
git clone https://github.com/seu-usuario/pagina-de-receitas.git

# Enter the project folder
cd pagina-de-receitas

# Install dependencies
npm install

# Start the development server
npm run dev
```

The project will be available at `http://localhost:5378`.

### Scripts

| Command           | Description                                  |
| ----------------- | -------------------------------------------- |
| `npm run dev`     | Starts the development server                |
| `npm run build`   | Generates the production build in `/dist`    |
| `npm run preview` | Previews the production build on port `4173` |

---

## Structure

```
├── public/
│   └── assets/              # Images (background, main image, favicon)
├── src/
│   ├── App.jsx              # Main React component
│   ├── main.jsx             # Application entry point
│   └── index.css            # Tailwind import and custom theme
├── index.html               # Main page with recipe and Tailwind classes
├── styles.css               # Tailwind base import
├── vite.config.js           # Vite config, aliases, plugins and build
├── vercel.json              # Vercel deploy config
├── posbuild.js              # Post-build script for asset cleanup
├── package.json             # Dependencies and scripts
└── README.md
```

---

## Color Palette

| Color        | Hex                | Usage              |
| ------------ | ------------------ | ------------------ |
| Dark brown   | `#291B1A`          | Headings           |
| Medium brown | `#573A37`          | Text and borders   |
| Golden beige | `#F6E9B2`          | Card background    |
| Soft yellow  | `bg-yellow-200/10` | Background overlay |
| TCPI blue    | `#557AA1`          | Custom theme color |

---

## Next steps

- [ ] Break the recipe into reusable components
- [ ] Add more recipes with page navigation
- [ ] Implement a backend with a recipes API
- [ ] Add search and filters
- [ ] User recipe submission system

---

## Author

**Pedro Paulo** — developed as part of the RocketSeat FullStack track.

---

## License

This project is free to use for educational purposes.