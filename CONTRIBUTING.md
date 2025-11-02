# Contributing to Code-Cross

✞ Thank you for considering contributing to Code-Cross! ✠

## Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/YOUR_USERNAME/code-cross.git
   cd code-cross
   ```
3. **Install dependencies**:
   ```bash
   npm install
   ```
4. **Create a branch** for your feature or bugfix:
   ```bash
   git checkout -b feature/your-feature-name
   ```

## Development Workflow

### Before You Start

- Check if there's already an issue for what you want to work on
- If not, create an issue to discuss your proposed changes
- Wait for approval before starting significant work

### While Developing

1. **Follow the code style**:
   - Use ESLint and Prettier configurations provided
   - Run `npm run lint` to check for issues
   - Run `npm run format` to format your code

2. **Write meaningful commits**:
   - Use clear, descriptive commit messages
   - Follow the pattern: `type: brief description`
   - Examples:
     - `feat: add user authentication`
     - `fix: resolve navigation bug`
     - `docs: update README setup instructions`
     - `style: format code with prettier`
     - `refactor: simplify API service logic`

3. **Test your changes**:
   - Make sure the app runs without errors
   - Test all affected functionality
   - Ensure the build succeeds: `npm run build`

4. **Keep your branch updated**:
   ```bash
   git fetch origin
   git rebase origin/main
   ```

## Code Style Guidelines

### JavaScript/React

- Use functional components with hooks
- Use arrow functions for component definitions
- Keep components small and focused
- Extract reusable logic into custom hooks
- Use path aliases for imports (e.g., `@components`, `@utils`)

### Component Structure

```jsx
import React from 'react';
import { useState } from 'react';
import PropTypes from 'prop-types'; // if using prop-types

const MyComponent = ({ title, onAction }) => {
  const [state, setState] = useState(initialValue);

  const handleAction = () => {
    // Handle logic
    onAction?.();
  };

  return (
    <div className="container">
      <h1>{title}</h1>
      {/* Component JSX */}
    </div>
  );
};

export default MyComponent;
```

### Naming Conventions

- **Components**: PascalCase (e.g., `UserProfile.jsx`)
- **Utilities/Hooks**: camelCase (e.g., `formatDate.js`, `useAuth.js`)
- **Constants**: UPPER_SNAKE_CASE (e.g., `API_BASE_URL`)
- **CSS Classes**: Follow Tailwind conventions

## Submitting Changes

1. **Push your branch** to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create a Pull Request**:
   - Go to the original repository on GitHub
   - Click "New Pull Request"
   - Select your branch
   - Fill out the PR template with:
     - Clear description of changes
     - Related issue number (if applicable)
     - Screenshots (for UI changes)
     - Testing notes

3. **Address review feedback**:
   - Be responsive to comments
   - Make requested changes
   - Push updates to the same branch

## Pull Request Guidelines

- **Title**: Clear and descriptive
- **Description**: Explain what, why, and how
- **Small PRs**: Keep changes focused and atomic
- **No merge conflicts**: Rebase on main before submitting
- **Tests pass**: Ensure linting and builds succeed

## Code Review Process

1. At least one maintainer will review your PR
2. Address any requested changes
3. Once approved, a maintainer will merge your PR
4. Your contribution will be acknowledged!

## Questions?

If you have questions or need help:
- Open an issue with the `question` label
- Reach out to maintainers

## Code of Conduct

- Be respectful and considerate
- Welcome newcomers and help them learn
- Focus on constructive feedback
- Assume good intentions

---

Thank you for contributing to Code-Cross! 

✞ May God bless your work ✠
