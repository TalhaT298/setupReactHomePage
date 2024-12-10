# React Router Tailwind DaisyUI Boilerplate

This repository provides a fully functional boilerplate for creating React projects with integrated React Router, TailwindCSS, DaisyUI, and essential configurations. It streamlines the process of starting a new project, allowing you to focus on building your application.

## Features

- **React Router DOM**: Set up for easy routing in your React applications.
- **TailwindCSS**: Pre-configured utility-first CSS framework.
- **DaisyUI**: Customizable component library built on TailwindCSS.
- **Vite**: Fast development server and build tool.
- **Linting**: Configured with ESLint for consistent code quality.
- **Dark and Light Themes**: Includes multiple DaisyUI themes like `dark`, `light`, `night`, and more.

## Installation

Clone this repository and get started with the following steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/react-router-tailwind-boilerplate.git
   cd react-router-tailwind-boilerplate
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start the development server:**
   ```bash
   npm run dev
   ```

## Usage

This boilerplate is ready for you to build your application. Below are key components:

- **`Home` Component:** A simple homepage template with a banner.
- **`Navbar` Component:** Responsive navigation bar with dropdown support for mobile screens.
- **`Footer` Component:** Customizable footer with social media links.

Feel free to extend or replace these components based on your project needs.

### File Structure
```
src/
├── components/
│   ├── Banner/
│   │   └── Banner.jsx
│   ├── Footer/
│   │   └── Footer.jsx
│   └── Navbar/
│       └── Navbar.jsx
├── Routes/
│   └── Routes.jsx
├── App.jsx
├── index.jsx
└── index.css
```

### TailwindCSS Configuration
TailwindCSS is configured in `tailwind.config.js` to scan all necessary files and includes DaisyUI with multiple themes.

```js
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
    themes: ["dark", "light", "black", "forest", "autumn", "valentine", "night", "dracula"],
  },
};
```

## Scripts

- **`npm run dev`**: Starts the development server.
- **`npm run build`**: Builds the project for production.
- **`npm run preview`**: Previews the production build.
- **`npm run lint`**: Runs ESLint for code quality checks.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---
