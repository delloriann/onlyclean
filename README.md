# Only Clean - Professional Carpet Cleaning Website

A modern, SEO-optimized Astro website for Only Clean, a London-based carpet cleaning business.

## 🚀 Quick Start

### Prerequisites
- Node.js 18+ 
- npm or yarn

### Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

The site will be available at `http://localhost:4321`

### Production Build

```bash
# Build for production
npm run build

# Preview production build
npm run preview
```

## 📁 Project Structure

```
/
├── public/
│   ├── admin/              # Pages CMS configuration
│   │   ├── config.yml      # CMS field definitions
│   │   └── index.html      # CMS admin panel
│   ├── images/             # Static images
│   └── favicon.svg
├── src/
│   ├── components/
│   │   ├── Hero.astro      # Homepage hero section
│   │   ├── SEO.astro       # Meta tags & JSON-LD schema
│   │   └── StickyFooter.astro  # Mobile CTA bar
│   ├── content/
│   │   ├── homepage/       # CMS-editable homepage content
│   │   └── settings/       # Global site settings
│   ├── layouts/
│   │   └── Layout.astro    # Base layout with fonts
│   ├── pages/
│   │   └── index.astro     # Homepage
│   └── styles/
│       └── global.css      # Tailwind + custom theme
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## 🎨 Design System

### Brand Colors
| Color | Hex | Usage |
|-------|-----|-------|
| Primary Cyan | `#2CD5E5` | Hero backgrounds, accents |
| Primary Dark | `#2B5E75` | Text, CTA buttons |
| Brand White | `#FFFFFF` | Logo text, button text |

### Typography
- **Headings:** Fraunces (Google Fonts) - Soft, retro-serif
- **Body:** Inter (Google Fonts) - Clean, modern sans-serif

### Mobile-First Features
- Sticky "Book Now" footer bar (fixed at bottom on mobile)
- Large touch targets (min 48px)
- Safe area support for iPhone X+

## 🔍 SEO Features

### Local SEO (London Focus)
- Geo-targeted H1: "London's Freshest Carpets, Guaranteed"
- Borough-specific subheadings
- LocalBusiness + CleaningService JSON-LD schema
- Area served: London, Greater London, Central/North/South/East/West London

### Technical SEO
- `fetchpriority="high"` on hero image (LCP optimization)
- Responsive `srcset` for images
- Semantic HTML structure
- Open Graph & Twitter Card meta tags

## 📝 Pages CMS

### Accessing the Admin Panel

1. Start the dev server: `npm run dev`
2. Navigate to: `http://localhost:4321/admin/`
3. Connect your GitHub repository
4. Edit content directly in the browser

### Editable Fields

**Homepage Hero:**
- SEO Title & Description
- Headline & Subheadline  
- CTA Button text & link
- Hero image
- Trust badge text

**Site Settings:**
- Business name, phone, email
- Address & opening hours
- Social media links

## 🛠 Customization

### Adding Real Images

Replace the placeholder SVGs in `/public/images/` with:
- `cleaner-hero.png` - Transparent PNG of cleaner (recommended: 600x700px)
- `logo.png` - Company logo (recommended: 400x100px)
- `og-default.jpg` - Social sharing image (1200x630px)

### Updating Contact Info

Edit `src/content/settings/general.json` or use Pages CMS.

### Modifying Schema

Update the JSON-LD in `src/components/SEO.astro`:
- Replace phone number
- Update address details
- Modify area served boroughs

## 📦 Dependencies

- **Astro 5.x** - Static site generator
- **Tailwind CSS 4.x** - Utility-first CSS
- **Google Fonts** - Fraunces & Inter

## 🚀 Deployment

Recommended platforms:
- **Vercel** (recommended for Astro)
- **Netlify**
- **Cloudflare Pages**

```bash
# Build command
npm run build

# Output directory
dist/
```

## 📄 License

Private - Only Clean © 2024
