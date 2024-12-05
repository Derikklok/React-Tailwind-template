# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

``` bash
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Derikklok/React-Tailwind-template.git
git push -u origin main


git remote add origin https://github.com/Derikklok/React-Tailwind-template.git
git branch -M main
git push -u origin main

```

# Empty tailwind project initialize  

```bash

Create npm project with shadcn  - updated


1. Create the project as normal

npm create vite@latest

__________________________________________________________________


2. Install tailwind css

npm install -D tailwindcss postcss autoprefixer

npx tailwindcss init -p


__________________________________________________________________


3.Create jsconfig.json as ususal

{
  "compilerOptions": {
    // ...
    "baseUrl": ".",
    "paths": {
      "@/*": [
        "./src/*"
      ]
    }
    // ...
  }
}


__________________________________________________________________



4.Update vite.config.js

import path from "path"
import react from "@vitejs/plugin-react"
import { defineConfig } from "vite"

export default defineConfig({
  plugins: [react()],
  resolve: {
    alias: {
      "@": path.resolve(__dirname, "./src"),
    },
  },
})


__________________________________________________________________



5.Update tailwind.config.js

  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
	'./pages/**/*.{html,js}',
    './components/**/*.{html,js}',
  ],

_________________________________________________________________


6. Update index.css file

remove everything then ->  Add

@tailwind base;
@tailwind components;
@tailwind utilities;


_________________________________________________________________


7. Run the command

npx shadcn@latest init

Which style would you like to use? › New York
Which color would you like to use as base color? › Zinc
Do you want to use CSS variables for colors? › no / yes






```