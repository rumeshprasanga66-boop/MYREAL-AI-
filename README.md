# AI Starter Kit – Next.js AI Website Templates and SaaS Starter Kit

A modern, feature-rich Next.js template for building AI-powered websites and SaaS applications. Built with TypeScript, Tailwind CSS, and designed for rapid development.

#### 📺 Preview
- [Live Demo](https://themewagon.github.io/aistarterkit/)

#### 📥 Original Source
- [Download from ThemeWagon](https://themewagon.com/themes/aistarterkit/)

## 📋 Table of Contents
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Configuration](#configuration)
- [Usage](#usage)
- [Customization](#customization)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features
- ⚡ Built with **Next.js 13+** for optimal performance
- 🎨 **Tailwind CSS** for modern, responsive design
- 🔐 **TypeScript** support for type-safe development
- 📱 **Fully Responsive** - Mobile, tablet, and desktop optimized
- 🚀 **SEO Optimized** with Next.js built-in SEO features
- 🎯 **Pre-built Components** for rapid development
- 🌙 **Dark Mode Support** (optional)
- 📦 **Production Ready** - Optimized for deployment

## 📦 Prerequisites
- **Node.js** 18.x or higher
- **npm** 9.x+ or **yarn** 1.22.x+
- A code editor (VS Code recommended)
- Git for version control

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/rumeshprasanga66-boop/MYREAL-AI-.git
cd MYREAL-AI-
```

### 2. Install Dependencies
```bash
npm install
# or
yarn install
# or
pnpm install
# or
bun install
```

### 3. Run the Development Server
```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser to see the result.

### 4. Build for Production
```bash
npm run build
npm run start
```

## 📁 Project Structure
```
MYREAL-AI-/
├── app/                    # Next.js app directory
│   ├── page.tsx           # Home page
│   ├── layout.tsx         # Root layout
│   └── ...
├── components/             # Reusable React components
│   ├── Header.tsx
│   ├── Footer.tsx
│   └── ...
├── public/                 # Static assets
│   ├── images/
│   ├── icons/
│   └── ...
├── styles/                 # Global styles
│   └── globals.css
├── lib/                    # Utility functions
│   └── utils.ts
├── package.json            # Dependencies and scripts
├── tsconfig.json          # TypeScript configuration
├── tailwind.config.js     # Tailwind CSS configuration
└── README.md              # This file
```

## ⚙️ Configuration

### Environment Variables
Create a `.env.local` file in the root directory:
```bash
# Example environment variables
NEXT_PUBLIC_API_URL=http://localhost:3000
NEXT_PUBLIC_APP_NAME=MyReal AI
```

### Tailwind CSS Configuration
Customize the theme in `tailwind.config.js`:
```javascript
// Add custom colors, fonts, spacing, etc.
module.exports = {
  theme: {
    extend: {
      colors: {
        primary: '#your-color',
      },
    },
  },
}
```

### TypeScript Configuration
Update `tsconfig.json` for strict type checking and path aliases:
```json
{
  "compilerOptions": {
    "baseUrl": ".",
    "paths": {
      "@/*": ["./*"]
    }
  }
}
```

## 🎯 Usage

### Creating a New Page
Create a new file in the `app` directory:
```bash
# app/about/page.tsx
export default function About() {
  return (
    <div>
      <h1>About Us</h1>
      <p>Your content here...</p>
    </div>
  )
}
```

### Using Components
Import and use components throughout your app:
```typescript
import Header from '@/components/Header'

export default function Home() {
  return (
    <>
      <Header />
      <main>Your content</main>
    </>
  )
}
```

### Adding Styles
Use Tailwind CSS classes directly in your JSX:
```typescript
<div className="flex items-center justify-between bg-gradient-to-r from-blue-500 to-purple-600 p-4 rounded-lg">
  <h1 className="text-2xl font-bold text-white">Welcome</h1>
</div>
```

## 🎨 Customization

### Change Brand Colors
Edit `tailwind.config.js`:
```javascript
theme: {
  colors: {
    primary: '#your-brand-color',
    secondary: '#your-secondary-color',
  },
}
```

### Modify Typography
Update fonts in `layout.tsx`:
```typescript
import { Inter, Poppins } from 'next/font/google'

const poppins = Poppins({
  subsets: ['latin'],
  weight: ['400', '600', '700'],
})
```

### Customize Components
All components are located in the `components/` directory and can be easily modified to match your brand and requirements.

## 🐛 Troubleshooting

### Port Already in Use
If port 3000 is already in use:
```bash
npm run dev -- -p 3001
```

### Module Not Found Errors
Clear cache and reinstall dependencies:
```bash
rm -rf node_modules package-lock.json
npm install
```

### Build Failures
Check for TypeScript errors:
```bash
npm run build
```

Ensure all imports are correct and all types are properly defined.

### Styling Issues
1. Clear `.next` folder: `rm -rf .next`
2. Restart development server
3. Ensure Tailwind CSS is properly configured in `tailwind.config.js`

### Common Issues
- **Hydration mismatch**: Ensure client/server code is consistent
- **Image optimization**: Use `next/image` for better performance
- **API routes**: Place them in `app/api/` directory

## 🤝 Contributing

Contributions are welcome! Here's how to get started:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/amazing-feature`
3. Commit changes: `git commit -m 'Add amazing feature'`
4. Push to branch: `git push origin feature/amazing-feature`
5. Open a Pull Request

## 📝 License

- **Design and Code**: Copyright © [nextjstemplates](https://nextjstemplates.com/)
- **Licensed under**: [MIT License](LICENSE)
- **Distributed by**: [ThemeWagon](https://themewagon.com)

## 📧 Support

For questions or issues, please:
- Open an issue on GitHub
- Check the [Troubleshooting](#troubleshooting) section
- Review the [original project documentation](https://themewagon.com/themes/aistarterkit/)

---

**Happy coding!** 🚀 Start building your AI-powered application today.
