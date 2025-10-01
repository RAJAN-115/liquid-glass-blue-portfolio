# 🌊 Liquid Glass Blue Portfolio (v2.0)

> **Version 2.0** - Enhanced with Blue Liquid Glassmorphism Design  
> Built upon the proven foundation of [ai-portfolio-tidio-integration](https://github.com/RAJAN-115/ai-portfolio-tidio-integration)

A stunning, production-ready portfolio website featuring blue liquid glassmorphism design aesthetics. This is the second iteration of the AI-powered portfolio, now with a modern glass morphism theme, enhanced visual effects, and all the powerful features from v1.0.

[![Vercel](https://img.shields.io/badge/vercel-%23000000.svg?style=for-the-badge&logo=vercel&logoColor=white)](https://rajansportfolio.vercel.app/) [![Next.js](https://img.shields.io/badge/Next.js-14-black?style=for-the-badge&logo=next.js)](https://nextjs.org/) [![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/) [![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)

## 🎯 What's New in Version 2.0

This version builds upon the successful **ai-portfolio-tidio-integration** repository and adds:

- 🎨 **Blue Liquid Glassmorphism Design** - Modern, sleek glass morphism effects with stunning blue theme
- 💎 **Enhanced Visual Aesthetics** - Semi-transparent frosted glass effects with depth and layering
- 🌊 **Fluid Animations** - Flowing, liquid-like transitions and interactive elements
- 🎭 **Advanced CSS Effects** - Backdrop blur, gradients, and sophisticated visual hierarchy
- ⚡ **All V1 Features Retained** - Tidio AI chat, voice navigation, performance optimization, and more

## ✨ Complete Feature Set

### 🎨 Design & Aesthetics (NEW in v2.0)
- Blue liquid glassmorphism effects throughout
- Semi-transparent frosted glass UI components
- Flowing animations with smooth transitions
- Blue color palette with dynamic gradients
- Depth layering for visual hierarchy
- Subtle backdrop blur effects

### 🤖 AI & Intelligence (From v1.0)
- Tidio AI chat integration with Lyro AI Agent
- Voice navigation and speech recognition
- Intelligent chatbot trained on portfolio knowledge
- Real-time user engagement

### 💻 Technical Excellence
- **Framework:** Next.js 14 with App Router
- **Language:** TypeScript 5.3 for type safety
- **Styling:** Tailwind CSS 3.4 with custom glassmorphism utilities
- **UI Components:** Radix UI primitives
- **Animations:** Framer Motion for fluid interactions
- **Icons:** Lucide React
- **Testing:** Jest & React Testing Library
- **Deployment:** Vercel with Edge Functions

### 🚀 Performance & UX
- Lighthouse 90+ scores across all metrics
- Optimized image loading and lazy loading
- Mobile-first responsive design
- PWA-ready with offline support
- Smooth scroll navigation
- Dark/Light theme toggle with persistence
- SEO optimized with meta tags and structured data

### 📱 Interactive Features
- Animated typewriter effect on homepage
- Real-time IST clock
- Profile avatar with resume download
- Interactive project gallery with live demos
- Skills dashboard with progress bars
- Contact form with validation
- Social media integration

## 📋 Prerequisites

Before you begin, ensure you have:

- **Node.js** 18.17 or later
- **pnpm** (recommended), npm, or yarn
- **Git** for version control

## 🚀 Getting Started

### Method 1: Use This Repository (Fresh Start)

```bash
# Clone this repository
git clone https://github.com/RAJAN-115/liquid-glass-blue-portfolio.git
cd liquid-glass-blue-portfolio

# Install dependencies
pnpm install
# or
npm install

# Run development server
pnpm dev
# or
npm run dev
```

### Method 2: Start from ai-portfolio-tidio-integration

```bash
# Clone the v1.0 repository
git clone https://github.com/RAJAN-115/ai-portfolio-tidio-integration.git liquid-glass-blue-portfolio
cd liquid-glass-blue-portfolio

# Change remote to this repository
git remote set-url origin https://github.com/RAJAN-115/liquid-glass-blue-portfolio.git

# Install dependencies
pnpm install

# Run development server
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) to see your portfolio.

## 🎨 Implementing Glassmorphism Design

### Step 1: Update Tailwind Configuration

Add glassmorphism utilities to `tailwind.config.ts`:

```typescript
// Add to theme.extend
backdropBlur: {
  xs: '2px',
},
colors: {
  glass: {
    light: 'rgba(255, 255, 255, 0.1)',
    dark: 'rgba(0, 0, 0, 0.1)',
    blue: 'rgba(59, 130, 246, 0.1)',
  }
}
```

### Step 2: Create Glass Components

Example glass card component:

```tsx
// components/ui/glass-card.tsx
export const GlassCard = ({ children, className }) => (
  <div className={`
    backdrop-blur-md bg-white/10 dark:bg-black/10
    border border-white/20 rounded-2xl
    shadow-xl hover:shadow-2xl transition-all
    ${className}
  `}>
    {children}
  </div>
);
```

### Step 3: Apply Blue Theme

Update your CSS with blue glassmorphism:

```css
.glass-morphism {
  background: linear-gradient(135deg, rgba(59, 130, 246, 0.1) 0%, rgba(147, 197, 253, 0.05) 100%);
  backdrop-filter: blur(10px);
  -webkit-backdrop-filter: blur(10px);
  border: 1px solid rgba(59, 130, 246, 0.18);
  box-shadow: 0 8px 32px 0 rgba(59, 130, 246, 0.15);
}
```

## 📁 Project Structure

```
liquid-glass-blue-portfolio/
├── app/                    # Next.js 14 App Router
│   ├── layout.tsx         # Root layout with theme provider
│   ├── page.tsx           # Homepage with glassmorphism
│   └── globals.css        # Global styles + glass effects
├── components/            # React components
│   ├── ui/               # Reusable UI with glass effects
│   ├── sections/         # Page sections (Hero, About, Projects, etc.)
│   ├── navbar.tsx        # Navigation with glass background
│   ├── footer.tsx        # Footer component
│   └── theme-provider.tsx # Dark/Light theme management
├── hooks/                # Custom React hooks
├── lib/                  # Utility functions
├── public/               # Static assets (images, resume, etc.)
├── styles/               # Additional styles
└── types/                # TypeScript type definitions
```

## 🎯 Development Roadmap

### Phase 1: Design Migration ✅
- [x] Set up repository structure
- [x] Create comprehensive README
- [ ] Copy codebase from ai-portfolio-tidio-integration
- [ ] Implement glassmorphism CSS utilities
- [ ] Update color scheme to blue theme

### Phase 2: Component Enhancement
- [ ] Transform UI components with glass effects
- [ ] Add liquid animation effects
- [ ] Implement gradient backgrounds
- [ ] Enhance hover and focus states

### Phase 3: Testing & Optimization
- [ ] Cross-browser testing
- [ ] Mobile responsiveness verification
- [ ] Performance optimization
- [ ] Accessibility audit

### Phase 4: Deployment
- [ ] Deploy to Vercel
- [ ] Configure custom domain (if applicable)
- [ ] Set up analytics
- [ ] Monitor performance metrics

## 🔧 Configuration

### Environment Variables

Create a `.env.local` file:

```env
# Tidio Chat (from v1.0)
NEXT_PUBLIC_TIDIO_KEY=your_tidio_public_key

# Analytics (optional)
NEXT_PUBLIC_GA_ID=your_google_analytics_id
```

### Tidio AI Setup

1. Sign up at [Tidio.com](https://www.tidio.com/)
2. Get your public key from the dashboard
3. Add it to `.env.local`
4. Customize chatbot responses in Tidio panel

## 🌐 Deployment

### Deploy to Vercel (Recommended)

```bash
# Install Vercel CLI
npm install -g vercel

# Deploy
vercel

# Production deployment
vercel --prod
```

Or use the [Vercel Dashboard](https://vercel.com/new) to deploy directly from GitHub.

## 📝 Development Guidelines

- ✅ Use TypeScript for all new components
- ✅ Follow Next.js 14 best practices
- ✅ Implement mobile-first responsive design
- ✅ Maintain glassmorphism aesthetic consistency
- ✅ Optimize images and assets
- ✅ Write clean, maintainable code
- ✅ Comment complex logic
- ✅ Test across different devices and browsers

## 🔗 Related Repositories

- **Version 1.0:** [ai-portfolio-tidio-integration](https://github.com/RAJAN-115/ai-portfolio-tidio-integration) - The original AI-powered portfolio
- **Live Demo:** [rajansportfolio.vercel.app](https://rajansportfolio.vercel.app/) (Currently v1.0)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Rajan Prajapati**  
Full-Stack Developer | MERN Stack Specialist | AI Enthusiast

- 📧 Email: rajanrp115@gmail.com
- 💼 LinkedIn: [linkedin.com/in/rajanrp115](https://linkedin.com/in/rajanrp115)
- 🐙 GitHub: [@RAJAN-115](https://github.com/RAJAN-115)
- 📱 WhatsApp: [+91 9545993850](https://wa.me/919545993850)
- 📍 Location: Mumbai, Maharashtra, India

## 🙏 Acknowledgments

- [Next.js](https://nextjs.org/) - The React Framework
- [Vercel](https://vercel.com/) - Deployment Platform
- [Tailwind CSS](https://tailwindcss.com/) - Styling Framework
- [Tidio](https://www.tidio.com/) - AI Chat Integration
- [Radix UI](https://www.radix-ui.com/) - UI Primitives
- [Framer Motion](https://www.framer.com/motion/) - Animation Library
- Community and Open Source Contributors

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!  
Feel free to check the [issues page](https://github.com/RAJAN-115/liquid-glass-blue-portfolio/issues).

## ⭐ Show Your Support

Give a ⭐️ if you like this project!

---

**Made with ❤️ and ☕ by Rajan Prajapati**  
*Version 2.0 - Blue Liquid Glassmorphism Edition*  
Last Updated: October 2025

> 💡 **Note:** This repository is currently being set up. The complete codebase from ai-portfolio-tidio-integration will be imported and enhanced with glassmorphism design. Stay tuned for updates!
