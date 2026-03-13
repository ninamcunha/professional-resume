# 📄 Professional Resume - React/TypeScript

<div align="center">

![React](https://img.shields.io/badge/React-18.3.1-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.1.12-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-6.3.5-646CFF?style=for-the-badge&logo=vite&logoColor=white)

**Bilingual professional resume (PT/EN) with high-fidelity PDF export**

[🌐 Live Demo](#) | [📥 Download PDF](#) | [🐛 Report Bug](../../issues) | [✨ Request Feature](../../issues)

</div>

---

## 📋 Table of Contents

- [About the Project](#-about-the-project)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [How to Use](#-how-to-use)
- [Customization](#-customization)
- [PDF Export](#-pdf-export)
- [Deployment](#-deployment)
- [License](#-license)

---

## 🎯 About the Project

This is an **interactive professional resume** built with React/TypeScript, specifically designed for tech professionals. The project offers a modern and responsive visual experience, with language toggle functionality (Portuguese/English) and PDF export with **100% visual fidelity**.

### 🎨 Design & Layout

- **Two perfectly structured pages** - Optimized layout for content distribution
- **Professional colors** - Dark red/wine titles (`#7f1d1d`), orange highlights (`#ea580c`)
- **Integrated icons** - Lucide React library for consistent visual elements
- **Dashed lines** - Elegant separators between sections
- **Smart spacing** - Language-specific adjustments to optimize visual distribution

### 📱 Responsiveness

- **Mobile-First** - Adapted layout for phones and tablets
- **Desktop Optimized** - 125% zoom applied only on large screens for better readability
- **Perfect Print** - Dedicated CSS to ensure impeccable PDF formatting

---

## ✨ Features

### 🌍 Complete Bilingual System

- **PT/EN Toggle** - Button in the top right corner with language icon
- **Dynamic Content** - All texts, sections, and information change instantly
- **Separate Data** - Independent files (`resumePT.ts` and `resumeEN.ts`)
- **Differentiated File Names** - PDFs exported with language-specific names

### 📥 PDF Export

- **High Fidelity** - 100% visual correspondence between screen and PDF
- **Exactly Two Pages** - Automatic and optimized content distribution
- **Advanced Print CSS** - Specific media queries for printing
- **window.print()** - Native solution without heavy external dependencies
- **Smart Names** - Files saved as `Curriculo_Nina_Menezes_Cunha.pdf` (PT) or `Resume_Nina_Menezes_Cunha.pdf` (EN)

### 📊 Resume Sections

1. **Header** - Name, title, email, LinkedIn, GitHub, portfolio
2. **Professional Summary** - Executive presentation
3. **Experience** - 6 positions with logos, dates, location, and descriptions
4. **Publications & Projects** - 7 featured items with clickable links
5. **Education** - 4 institutions with logos and details
6. **Certifications** - 10 certificates with institutions, dates, and credentials
7. **Skills** - Categories with dynamic icons

### 🎨 Smart Layout

- **Desktop**: 2-column layout (experience/publications on left, summary/education/skills/certifications on right)
- **Mobile**: Single column layout with optimized order
- **Language Adjustments**: Specific spacing (PT: 0.95rem, EN: 0.5rem in experiences)

---

## 🛠 Technologies Used

### Core

| Technology | Version | Description |
|------------|---------|-------------|
| **React** | 18.3.1 | JavaScript library for user interfaces |
| **TypeScript** | 5.x | Typed superset of JavaScript |
| **Vite** | 6.3.5 | Modern and fast build tool |
| **Tailwind CSS** | 4.1.12 | Utility-first CSS framework |

### Main Libraries

| Library | Version | Project Use |
|---------|---------|-------------|
| **lucide-react** | 0.487.0 | SVG icons (Mail, LinkedIn, GitHub, etc.) |
| **@radix-ui/** | Multiple | Accessible UI components (base) |
| **class-variance-authority** | 0.7.1 | CSS class management |
| **tailwind-merge** | 3.2.0 | Smart merging of Tailwind classes |

### Extra Features

- **react-router** (7.13.0) - Routing (if needed for expansion)
- **motion** (12.23.24) - Smooth animations
- **date-fns** (3.6.0) - Date manipulation
- **sonner** (2.0.3) - Toast notifications

---

## 📁 Project Structure

```
📦 professional-resume
├── 📂 src
│   ├── 📂 app
│   │   ├── 📄 App.tsx                    # Main component with language logic and PDF
│   │   ├── 📂 components
│   │   │   ├── 📄 Resume.tsx             # Resume component with mobile/desktop layouts
│   │   │   ├── 📄 ResumePDF.tsx          # [Legacy] Previous PDF component
│   │   │   ├── 📂 figma
│   │   │   │   └── 📄 ImageWithFallback.tsx  # [System] Image component
│   │   │   └── 📂 ui                     # UI components (Radix + Tailwind)
│   │   │       ├── 📄 button.tsx
│   │   │       ├── 📄 card.tsx
│   │   │       └── ... (50+ components)
│   │   └── 📂 data
│   │       ├── 📄 resumePT.ts            # Resume data in Portuguese
│   │       ├── 📄 resumeEN.ts            # Resume data in English
│   │       └── 📄 resume.ts              # [Legacy] Old data
│   └── 📂 styles
│       ├── 📄 index.css                  # Global CSS
│       ├── 📄 tailwind.css               # Tailwind configurations
│       ├── 📄 theme.css                  # Theme tokens
│       └── 📄 fonts.css                  # Font imports
├── 📄 package.json                       # Dependencies and scripts
├── 📄 vite.config.ts                     # Vite configuration
├── 📄 postcss.config.mjs                 # PostCSS configuration
└── 📄 README.md                          # This file
```

### 🗂 Main Files

#### **`/src/app/App.tsx`**
- Application root component
- Manages language state (`pt` | `en`)
- Implements `downloadPDF()` function with `window.print()`
- Applies 125% zoom on desktop (`md:scale-125`)
- Defines PDF filename dynamically

#### **`/src/app/components/Resume.tsx`**
- Main resume component
- Receives data via typed props (`ResumeProps`)
- Contains 2 layouts: mobile (`.md:hidden`) and desktop (`.hidden.md:grid`)
- Dynamic icons based on categories
- Print styles with `print:` utilities

#### **`/src/app/data/resumePT.ts` and `/src/app/data/resumeEN.ts`**
- TypeScript objects with all content
- Structures: `header`, `summary`, `experiences`, `education`, `skillCategories`, `publications`, `certifications`
- Company/institution logos in base64 or URLs

---

## 🚀 Installation

### Prerequisites

- **Node.js** 18+ ([Download](https://nodejs.org/))
- **pnpm** (recommended) or npm/yarn

```bash
# Install pnpm (if you don't have it)
npm install -g pnpm
```

### Installation Steps

1. **Clone the repository**

```bash
git clone https://github.com/your-username/professional-resume.git
cd professional-resume
```

2. **Install dependencies**

```bash
pnpm install
```

3. **Start the development server**

```bash
pnpm dev
```

4. **Open in browser**

```
http://localhost:5173
```

---

## 💻 How to Use

### 1️⃣ Toggle Languages

Click the **PT/EN** button in the top right corner of the resume. The content will change instantly.

### 2️⃣ Export to PDF

**Option 1: Download Button** (if implemented)
- Click the download button
- The browser will open the print dialog
- Select "Save as PDF"

**Option 2: Manual**
```bash
Ctrl+P (Windows/Linux) or Cmd+P (Mac)
```

### 3️⃣ View on Desktop

The resume automatically applies **125% zoom** on large screens (≥768px) for better readability. On mobile, it remains 100%.

### 4️⃣ View on Mobile

The layout adapts to a single column with:
- Each contact link on a separate line
- Sections stacked vertically
- Optimized spacing

---

## 🎨 Customization

### Change Personal Data

Edit the files `/src/app/data/resumePT.ts` and `/src/app/data/resumeEN.ts`:

```typescript
export const resumePT = {
  header: {
    name: "YOUR NAME",
    title: "Your Professional Title",
    email: "your.email@example.com",
    linkedin: "https://linkedin.com/in/your-profile",
    github: "https://github.com/your-username",
    portfolio: "https://your-portfolio.com"
  },
  summary: "Your professional summary here...",
  experiences: [
    {
      role: "Position",
      company: "Company",
      period: "Jan 2023 - Present",
      location: "City, Country",
      description: ["Responsibility 1", "Responsibility 2"],
      logo: "URL_OR_BASE64"
    }
  ],
  // ... continue with other sections
};
```

### Change Colors

Edit `/src/styles/theme.css` or use Tailwind classes directly:

```css
/* Main title color */
.text-red-900 → Change to .text-blue-900

/* Highlight color */
.text-orange-600 → Change to .text-green-600

/* Borders */
.border-red-900 → Change to .border-blue-900
```

### Adjust Spacing

In the file `/src/app/App.tsx`, inside the `<style>` tag:

```css
/* Spacing between experiences (PT) */
[data-language="pt"] #resume-content > div > div > section:nth-child(2) > div > div {
  margin-bottom: 0.95rem; /* Adjust value */
}

/* Spacing between experiences (EN) */
[data-language="en"] #resume-content > div > div > section:nth-child(2) > div > div {
  margin-bottom: 0.5rem; /* Adjust value */
}
```

### Add New Sections

1. Add data to `resumePT.ts` and `resumeEN.ts`
2. Create JSX structure in `Resume.tsx`
3. Add icons from `lucide-react` library
4. Style with Tailwind CSS

---

## 📄 PDF Export

### How It Works

The system uses **`window.print()`** combined with **print CSS** to generate PDFs:

```typescript
const downloadPDF = () => {
  const fileName = language === 'pt' 
    ? 'Curriculo_Nina_Menezes_Cunha.pdf' 
    : 'Resume_Nina_Menezes_Cunha.pdf';

  const style = document.createElement('style');
  style.innerHTML = `@page { size: A4; margin: 0; }`;
  document.head.appendChild(style);

  document.title = fileName.replace('.pdf', '');
  window.print();
  
  document.head.removeChild(style);
};
```

### Print CSS

Tailwind classes with `print:` prefix:

```jsx
<div className="print:shadow-none print:max-w-none print:p-3 print:m-0">
  <button className="print:hidden">Button that doesn't appear in PDF</button>
</div>
```

### Optimizations

- **`@page { size: A4; margin: 0; }`** - Defines exact page size
- **`print:scale-100`** - Removes desktop zoom in PDF
- **Page breaks** - Avoided with adjusted spacing
- **Colors maintained** - `-webkit-print-color-adjust: exact`

### Troubleshooting

**Problem**: PDF appears in more than 2 pages
- **Solution**: Adjust language-specific spacing

**Problem**: Colors don't appear in PDF
- **Solution**: Add `-webkit-print-color-adjust: exact;` to CSS

**Problem**: Broken layout in PDF
- **Solution**: Check `print:` classes and `@media print` media query

---

## 🌐 Deployment

### Deployment Options

#### **Vercel** (Recommended)

```bash
# Install Vercel CLI
pnpm install -g vercel

# Deploy
vercel
```

#### **Netlify**

```bash
# Build
pnpm build

# Drag the 'dist' folder to Netlify Drop
```

#### **GitHub Pages**

1. Add to `vite.config.ts`:

```typescript
export default defineConfig({
  base: '/professional-resume/', // Your repository name
  // ... other configs
});
```

2. Add script to `package.json`:

```json
"scripts": {
  "deploy": "vite build && gh-pages -d dist"
}
```

3. Execute:

```bash
pnpm install -D gh-pages
pnpm deploy
```

---

## 📦 Available Scripts

| Command | Description |
|---------|-------------|
| `pnpm dev` | Starts development server |
| `pnpm build` | Creates production build in `dist/` folder |
| `pnpm preview` | Preview of production build |

---

## 🎓 Technical Details

### TypeScript Interfaces

```typescript
interface ResumeProps {
  experiences: Experience[];
  education: Education[];
  skillCategories: SkillCategory[];
  publications: Publication[];
  certifications: Certification[];
  summary: string;
  header: {
    name: string;
    title: string;
    email: string;
    linkedin: string;
    github: string;
    portfolio: string;
  };
  sections: {
    experience: string;
    summary: string;
    skills: string;
    education: string;
    publications: string;
    certifications: string;
  };
  language: 'pt' | 'en';
  onLanguageToggle: () => void;
}
```

### Responsive Breakpoints

- **Mobile**: `< 768px` - Single column layout
- **Desktop**: `≥ 768px` (`.md:`) - 2-column layout + 125% zoom
- **Print**: Media query `@media print` - PDF-optimized layout

### Dynamic Icons

```typescript
const getSkillIcon = (title: string) => {
  const lowerTitle = title.toLowerCase();
  if (lowerTitle.includes('programm')) return <Database />;
  if (lowerTitle.includes('data')) return <Cpu />;
  if (lowerTitle.includes('machine')) return <Briefcase />;
  // ... more conditions
  return <Code />; // default icon
};
```

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. **Fork** the project
2. Create a **Branch** for your feature (`git checkout -b feature/NewFeature`)
3. **Commit** your changes (`git commit -m 'Add new feature'`)
4. **Push** to the Branch (`git push origin feature/NewFeature`)
5. Open a **Pull Request**

---

## 📝 License

This project is under the MIT license. See the [LICENSE](LICENSE) file for more details.

---

## 👤 Author

**Nina Menezes Cunha**

- LinkedIn: [nina-menezes-cunha](https://linkedin.com/in/nina-menezes-cunha)
- GitHub: [@ninamenezes](https://github.com/ninamenezes)
- Portfolio: [ninamenezes.com](https://ninamenezes.com)

---

## 🙏 Acknowledgments

- [Lucide Icons](https://lucide.dev/) - Icon library
- [Tailwind CSS](https://tailwindcss.com/) - CSS framework
- [Radix UI](https://www.radix-ui.com/) - Primitive components
- [Vite](https://vitejs.dev/) - Build tool

---

<div align="center">

**Made with ❤️ and React**

⭐ If this project helped you, consider giving it a star!

</div>
