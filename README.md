# Vite React Tailwind Template

Vite React Tailwind CSS starter project (with Vite, Typescript, ESLint, Sass)

## Quick Start using degit

> _NOTE: need to install degit first with `npm i -g degit`_

```bash
degit emanuelefavero/vite-react-tailwind my-app
cd my-app
npm install
npm run dev
```

## Usage

- clone this repo
- run `npm install`
- run `npm run dev` to start the vite dev server
- run `npm run host` to start the vite dev server with host
- run `npm run build` to just build the project
- run `npm run preview` to preview the build

## Features

- Vite
- React
- Tailwind
- Typescript
- ESLint
- Prettier (I've added a .prettierrc file with my personal settings but I've not added prettier as a dependency since I just use the prettier extension in VSCode)
- Sass

## Recreate this template from scratch

- run `npm create vite@latest my-vite-app --template react-ts`
- cd into the project
- run `npm install`
- run `eslint --init` and choose your preferred options
- add these rules in .eslintrc.json (suppress errors for missing 'import React' in files)

```json
    "react/react-in-jsx-scope": "off",
    "react/jsx-filename-extension": [
      1,
      { "extensions": [".js", ".jsx", ".ts", ".tsx"] }
    ]
```

- run `npm install -D sass`
- change `App.css` to `App.scss`

### Install Tailwind

- run `npm install -D tailwindcss postcss autoprefixer`
- initialize tailwind with `npx tailwindcss init -p`
- add template files paths in `tailwind.config.js`

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ['./index.html', './src/**/*.{js,ts,jsx,tsx}'],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

- add tailwind directives in `index.css`

```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

- start the build process with `npm run dev`

- start using tailwind classes in your components!

### Cheat sheets

- [Tailwind cheat sheet](https://nerdcave.com/tailwind-cheat-sheet)
- [Typescript cheat sheet](https://github.com/emanuelefavero/typescript)
- [Sass cheat sheet](https://devhints.io/sass)

## Resources

- [Vite](https://vitejs.dev/)
- [React](https://reactjs.org/)
- [Tailwind](https://tailwindcss.com/)
- [Typescript](https://www.typescriptlang.org/)
- [Sass](https://sass-lang.com/)
- [ESLint](https://eslint.org/)
- [Prettier](https://prettier.io/)
