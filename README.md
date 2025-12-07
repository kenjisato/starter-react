# React + Vite Starter Template

A modern, lightweight starter template for building React applications with Vite. This template provides a minimal setup to get React working with Vite, including Hot Module Replacement (HMR) and ESLint rules.

## Features

- ⚡️ **Vite** - Lightning-fast build tool and dev server
- ⚛️ **React 19** - Latest version of React
- 🎨 **CSS Support** - Write plain CSS with full support
- 🔥 **Hot Module Replacement** - Instant feedback during development
- 📦 **ESLint** - Code quality and consistency with preconfigured rules
- 🚀 **Fast Refresh** - Preserve component state during edits

## Getting Started

### Prerequisites

- Node.js (version 18 or higher recommended)
- npm or yarn or pnpm

### Installation

1. Clone this repository:
```bash
git clone https://github.com/kenjisato/starter-react.git
cd starter-react
```

2. Install dependencies:
```bash
npm install
```

### Development

Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5173` (or another port if 5173 is already in use).

### Building for Production

Build the application for production:
```bash
npm run build
```

The build output will be in the `docs` directory.

### Preview Production Build

Preview the production build locally:
```bash
npm run preview
```

### Deploying to GitHub Pages

This project is configured to deploy to GitHub Pages from the `docs` directory:

1. Build the project:
```bash
npm run build
```

2. Commit and push the `docs` directory to your repository:
```bash
git add docs
git commit -m "Build for GitHub Pages"
git push
```

3. Enable GitHub Pages in your repository settings:
   - Go to Settings → Pages
   - Under "Source", select "Deploy from a branch"
   - Select the `main` branch and `/docs` folder
   - Click Save

Your site will be available at `https://kenjisato.github.io/starter-react/`

### Linting

Run ESLint to check code quality:
```bash
npm run lint
```

## Project Structure

```
starter-react/
├── public/          # Static assets
├── src/
│   ├── assets/      # Images, fonts, and other assets
│   ├── App.css      # App component styles
│   ├── App.jsx      # Main App component
│   ├── index.css    # Global styles
│   └── main.jsx     # Application entry point
├── .gitignore       # Git ignore rules
├── eslint.config.js # ESLint configuration
├── index.html       # HTML entry point
├── package.json     # Project dependencies and scripts
└── vite.config.js   # Vite configuration
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## Technologies Used

- **React** - UI library
- **Vite** - Build tool and dev server
- **ESLint** - Code linting
- **@vitejs/plugin-react** - Official Vite plugin for React

## Customization

### Changing the Port

Edit `vite.config.js` to specify a custom port:

```javascript
export default defineConfig({
  plugins: [react()],
  server: {
    port: 3000
  }
})
```

### Adding Environment Variables

Create a `.env` file in the root directory and prefix variables with `VITE_`:

```
VITE_API_URL=https://api.example.com
```

Access them in your code:
```javascript
const apiUrl = import.meta.env.VITE_API_URL
```

## License

This template is available as open source under the terms of your chosen license.

## Contributing

Contributions are welcome! Feel free to submit issues and pull requests.