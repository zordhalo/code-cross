# code-cross

✞ Jesus Christ is Risen ~ Repository for project code-cross ✠

A modern React application built with Vite, TailwindCSS, Redux Toolkit, and React Router.

## 🚀 Features

- ⚡️ React 18.3 with Vite for fast development and building
- 🎨 TailwindCSS for utility-first styling
- 🔄 Redux Toolkit for state management
- 🛣️ React Router v6 for navigation
- 📦 Path aliases for clean imports
- 🔍 ESLint for code quality
- 💅 Prettier for code formatting

## 📋 Prerequisites

- Node.js (version 16 or higher)
- npm or yarn

## 🛠️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/zordhalo/code-cross.git
cd code-cross
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up environment variables

Copy the example environment file and configure it:

```bash
cp .env.example .env
```

Edit `.env` and update the variables as needed.

### 4. Start the development server

```bash
npm run dev
```

The application will be available at `http://localhost:5173`

## 📜 Available Scripts

- `npm run dev` - Start the development server
- `npm run build` - Build for production
- `npm run preview` - Preview the production build
- `npm run lint` - Run ESLint to check code quality
- `npm run format` - Format code with Prettier

## 📁 Project Structure

```
src/
├── components/     # Reusable UI components
├── pages/          # Page components (route-level)
├── features/       # Redux slices and feature-based modules
├── hooks/          # Custom React hooks
├── utils/          # Utility functions and helpers
├── assets/         # Static assets (images, fonts, etc.)
└── styles/         # Global styles and CSS modules
```

### Folder Purpose

- **components/**: Shared, reusable UI components (buttons, forms, cards, etc.)
- **pages/**: Top-level components that represent entire pages/routes
- **features/**: Redux slices, actions, and feature-specific logic
- **hooks/**: Custom React hooks for shared logic
- **utils/**: Helper functions, constants, and utilities
- **assets/**: Images, fonts, and other static files
- **styles/**: Global CSS, TailwindCSS customizations

## 🔧 Path Aliases

The project uses path aliases for cleaner imports:

```javascript
// Instead of: import Button from '../../../components/Button'
import Button from '@components/Button';

// Available aliases:
// @           -> src/
// @components -> src/components
// @pages      -> src/pages
// @features   -> src/features
// @hooks      -> src/hooks
// @utils      -> src/utils
// @assets     -> src/assets
// @styles     -> src/styles
```

## 🎨 Styling with TailwindCSS

This project uses TailwindCSS for styling. You can use Tailwind utility classes directly in your JSX:

```jsx
<div className="flex items-center justify-center p-4 bg-blue-500">
  <h1 className="text-2xl font-bold text-white">Hello World</h1>
</div>
```

## 🏗️ Building for Production

```bash
npm run build
```

The optimized files will be in the `dist/` directory.

## 📝 Contributing

We welcome contributions! Please follow these guidelines:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Contribution Guidelines

- Follow the existing code style
- Run `npm run lint` and `npm run format` before committing
- Write meaningful commit messages
- Update documentation for significant changes
- Add tests when applicable

## 📄 License

This project is licensed under the terms specified in the LICENSE file.

## 🙏 Acknowledgments

Built with modern web technologies and best practices.

---

✞ For the glory of God ✠
