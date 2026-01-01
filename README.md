# Vite React File Routing Template

A Vite + React + TypeScript starter template with file-based routing.

## Features

- ⚡️ **Vite + Rolldown** - Lightning-fast development and build
- ⚛️ **React 19** with React Compiler for automatic optimizations
- 🗂️ **File-based routing** with vite-plugin-pages - No manual route configuration needed
- 🎨 **Tailwind CSS v4** - Latest styling framework
- 📝 **TypeScript** - Type safety out of the box
- 🔍 **ESLint** - Pre-configured for React 19

## File-Based Routing

This template uses [vite-plugin-pages](https://github.com/hannoeru/vite-plugin-pages) for automatic route generation. Simply create files in the `src/pages` directory, and routes are automatically created:

```
src/pages/
  ├── index.tsx        →  /
  ├── about.tsx        →  /about
  ├── users/
  │   ├── index.tsx    →  /users
  │   └── [id].tsx     →  /users/:id (dynamic route)
  └── blog/
      └── [slug].tsx   →  /blog/:slug
```

No need to manually configure React Router - just create files and start building!

## Folder Structure

```
vite-react-file-routing-starter
├── public
│   └── vite.svg
├── src
│   ├── assets
│   ├── pages
│   │   ├── index.tsx
│   │   ├── page-a
│   │   │   ├── index.tsx
│   │   │   └── components
│   │   │       └── HeroSection.tsx
│   │   └── page-b.tsx
│   ├── App.css
│   ├── index.css
│   └── main.tsx
├── index.html
├── package.json
├── tsconfig.json
├── vite.config.ts
└── README.md
```

## Getting Started

To get a local copy up and running, follow these steps:

**1. Clone the repository**

```bash
git clone https://github.com/your-username/vite-react-file-routing-starter.git
cd vite-react-file-routing-starter
```

**2. Install dependencies**

```bash
pnpm install
```

**3. Start the development server**

```bash
pnpm dev
```

Then open [http://localhost:5173](http://localhost:5173) to view it in your browser.

## Available Scripts

| Script       | Description                                         |
| ------------ | --------------------------------------------------- |
| `pnpm dev`   | Starts the development server                       |
| `pnpm build` | Builds the app for production to the `dist` folder  |
| `pnpm preview` | Serves the production build locally               |
| `pnpm lint`  | Runs ESLint to check code quality                   |

## License

This project is licensed under the MIT License.
