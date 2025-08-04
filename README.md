# React Tailwind Boilerplate

A modern, high-performance React boilerplate with the latest versions of React, TypeScript, Vite, React Router, and Tailwind CSS v4.0.

## ✨ Features

- ⚡ **Vite 7.0** - Lightning-fast development server with HMR
- ⚛️ **React 19** - Latest React with TypeScript support
- 🎨 **Tailwind CSS v4.0** - CSS-first configuration with `@theme` directive
- 🌐 **React Router v7** - Client-side routing
- 🔒 **TypeScript** - Full type safety
- 📱 **Responsive Design** - Mobile-first approach
- 🚀 **Optimized Build** - Production-ready builds

## 🆕 What's New in Tailwind CSS v4.0

Tailwind CSS v4.0 brings significant improvements:

- **CSS-First Configuration**: Configure your design system directly in CSS using `@theme`
- **Vite Plugin Integration**: Native Vite plugin for better performance
- **Auto Content Detection**: No manual content configuration needed
- **Performance Boost**: 5x faster builds, 100x faster incremental builds
- **Simplified Installation**: Fewer dependencies, zero configuration

## 🚀 Quick Start

### Prerequisites

- Node.js 18+ 
- npm or yarn

### Installation

1. **Clone this repository**
   ```bash
   git clone https://github.com/your-username/react-tailwind-boilerplate.git
   cd react-tailwind-boilerplate
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   ```
   http://localhost:5173
   ```

## 📦 Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint |

## 🏗️ Project Structure

```
src/
├── components/          # Reusable UI components
│   ├── Layout.tsx      # Main layout wrapper
│   └── Navigation.tsx  # Navigation component
├── pages/              # Page components
│   ├── Home.tsx        # Home page
│   └── About.tsx       # About page
├── App.tsx             # Main App component with routing
├── main.tsx            # Application entry point
├── index.css           # Global styles with Tailwind imports
└── vite-env.d.ts       # Vite type definitions
```

## 🎨 Tailwind CSS v4.0 Configuration

This boilerplate uses the new CSS-first configuration approach:

### CSS Configuration (`src/index.css`)
```css
@import "tailwindcss";

@theme {
  --font-display: "system-ui", "sans-serif";
  --color-primary: #3b82f6;
  --color-secondary: #6366f1;
}
```

### Vite Integration (`vite.config.ts`)
```typescript
import { defineConfig } from 'vite'
import react from '@vitejs/plugin-react'
import tailwindcss from '@tailwindcss/vite'

export default defineConfig({
  plugins: [
    react(),
    tailwindcss(),
  ],
})
```

## 🔧 Customization

### Adding Custom Colors
```css
@theme {
  --color-brand: #ff6b6b;
  --color-accent: #4ecdc4;
}
```

### Custom Fonts
```css
@theme {
  --font-heading: "Inter", "system-ui", "sans-serif";
  --font-body: "Open Sans", "system-ui", "sans-serif";
}
```

### Breakpoints
```css
@theme {
  --breakpoint-tablet: 640px;
  --breakpoint-laptop: 1024px;
  --breakpoint-desktop: 1280px;
}
```

## 🌐 Routing

This boilerplate includes React Router v7 setup:

```typescript
// Add new routes in src/App.tsx
<Routes>
  <Route path="/" element={<Home />} />
  <Route path="/about" element={<About />} />
  <Route path="/contact" element={<Contact />} />
</Routes>
```

## 📱 Components

### Layout Component
- Responsive navigation
- Main content wrapper
- Consistent spacing

### Navigation Component
- Mobile-friendly design
- Active link highlighting
- Smooth transitions

## 🏷️ Tech Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| React | ^19.1.0 | UI Library |
| TypeScript | ~5.8.3 | Type Safety |
| Vite | ^7.0.4 | Build Tool |
| Tailwind CSS | ^4.1.11 | Styling |
| React Router | ^7.7.1 | Routing |

## 🎯 Best Practices

- **Component Organization**: Separate components and pages
- **TypeScript**: Strict typing for better development experience
- **CSS-in-CSS**: Use Tailwind's new `@theme` directive for customization
- **Responsive Design**: Mobile-first approach with Tailwind utilities
- **Performance**: Optimized builds with Vite

## 🚀 Deployment

### Build for Production
```bash
npm run build
```

### Deploy to Vercel
```bash
npx vercel --prod
```

### Deploy to Netlify
```bash
npm run build
# Upload dist/ folder to Netlify
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Vite](https://vitejs.dev/) - Next generation frontend tooling
- [React](https://reactjs.org/) - A JavaScript library for building user interfaces
- [Tailwind CSS](https://tailwindcss.com/) - A utility-first CSS framework
- [React Router](https://reactrouter.com/) - Declarative routing for React

---

**Happy coding! 🎉**

For questions or support, please open an issue on GitHub.