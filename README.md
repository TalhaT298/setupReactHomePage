## Modern React Boilerplate with Vite, TailwindCSS & DaisyUI

This project is designed as a modern React home boilerplate, leveraging the power of Vite for fast and efficient development. By integrating essential tools like React Router DOM, TailwindCSS, and DaisyUI, this setup provides a robust foundation for building responsive and dynamic web applications. </br>

To get started, the project begins with the creation of a new React application using Vite, a build tool that significantly speeds up development with its optimized performance. Installing React Router DOM is crucial for enabling seamless navigation between different pages of the application, enhancing the user experience by providing client-side routing capabilities.</br>

TailwindCSS, a utility-first CSS framework, is then integrated to facilitate rapid UI development with minimal custom CSS. This ensures that the application remains responsive and visually appealing across different devices. Complementing TailwindCSS, DaisyUI is introduced to provide pre-built components with customizable themes, further accelerating the development process while maintaining design consistency.</br>

ESLint is incorporated into the project to maintain code quality and ensure consistency across the codebase. This tool is vital for catching potential issues early in the development process, leading to a more reliable and maintainable application.</br>


# Project Setup

This guide will help you set up a new React project using Vite, React Router DOM, and TailwindCSS.

## 1. Create a New Project with Vite

To start, create a new project using Vite:

```bash
npm create vite@latest name-of-your-project -- --template react
```
Replace name-of-your-project with your desired project name.

Navigate into your project directory:

```bash
cd name-of-your-project
```
Install the initial dependencies:

```bash
npm install
```
## 2. Set Up React Router DOM
Next, install React Router DOM and its dependencies:

```bash
npm install react-router-dom
npm install localforage match-sorter sort-by
```
These libraries are essential for client-side routing and data management in your React app.

## 3. Set Up TailwindCSS
To set up TailwindCSS, you need to install TailwindCSS and its dependencies:

```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```
Next, configure Tailwind to remove unused styles in production by adding the paths to all of your template files in the content array in tailwind.config.js:

```bash
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```
Then, include Tailwind in your CSS by adding the following lines to your src/index.css file:

```bash
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## 4. Install DaisyUI
DaisyUI is a plugin for TailwindCSS that provides pre-built UI components. Install it with:

```bash
npm i -D daisyui@latest
```
Then, add DaisyUI to your tailwind.config.js plugins:

```bash
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [require("daisyui")],
  daisyui: {
    themes: ["dark","light","black","forest","autumn","valentine","night","dracula"],
  },
}
```

By following the installation steps and configuring each tool correctly, developers can quickly set up a powerful and scalable React application. This boilerplate not only simplifies the initial setup but also provides a strong foundation for building complex, production-ready web applications.</br>
