
🇺🇸 English | [🇧🇷 Português](./README_PT.md)

# Professional Resume Template

![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.1-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-6.x-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Deploy](https://img.shields.io/badge/Deploy-GitHub_Pages-black?style=for-the-badge&logo=github)

A bilingual **professional resume template built with React, TypeScript and Vite**, designed to be easily customized and deployed using GitHub Pages.

---

# Live Demo

https://ninamcunha.github.io/professional-resume/

---

# Download Resume

English  
https://ninamcunha.github.io/professional-resume/pdfs/Nina_Menezes_Cunha_Resume_EN.pdf

Português  
https://ninamcunha.github.io/professional-resume/pdfs/Nina_Menezes_Cunha_Resume_PT.pdf

---

# Features

• bilingual resume support (EN / PT)  
• responsive layout  
• printable design  
• downloadable PDF files  
• structured resume data separated from UI  
• GitHub Pages deployment  
• easy customization

---

# Tech Stack

React  
TypeScript  
Vite  
TailwindCSS  
GitHub Pages

---

# Project Structure

```
professional-resume
├── public
│   └── pdfs
│       ├── Nina_Menezes_Cunha_Resume_EN.pdf
│       └── Nina_Menezes_Cunha_Resume_PT.pdf
├── src
│   ├── app
│   │   ├── components
│   │   ├── data
│   │   │   ├── resumeEN.ts
│   │   │   └── resumePT.ts
│   │   └── App.tsx
│   ├── assets
│   ├── styles
│   └── main.tsx
├── package.json
├── vite.config.ts
└── README.md
```

---

# Run Locally

Clone the repository

git clone https://github.com/your-username/professional-resume.git

cd professional-resume

Install dependencies

npm install

Start development server

npm run dev

Open

http://localhost:5173

---

# Build

npm run build

Preview production

npm run preview

---

# Deploy to GitHub Pages

npm run deploy

Then enable GitHub Pages:

Repository → Settings → Pages

Branch: gh-pages

---

# Replicating This Resume

1. Clone the repository

git clone https://github.com/your-username/professional-resume.git

2. Install dependencies

npm install

3. Edit resume content

src/app/data/resumeEN.ts  
src/app/data/resumePT.ts

4. Replace logos

src/assets

5. Replace PDFs

public/pdfs

6. Adjust base path

vite.config.ts

base: '/your-repository-name/'

7. Deploy

npm run deploy

---

# Scripts

npm run dev  
npm run build  
npm run preview  
npm run deploy

---

# License

MIT

---

# Author

Nina Menezes Cunha
