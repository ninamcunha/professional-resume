
[🇺🇸 English](./README.md) | 🇧🇷 Português

# Template de Currículo Profissional

![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.1-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-6.x-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Deploy](https://img.shields.io/badge/Deploy-GitHub_Pages-black?style=for-the-badge&logo=github)

Template de currículo profissional **bilíngue (PT/EN)** criado com React, TypeScript e Vite.

---

# Demo

https://ninamcunha.github.io/professional-resume/

---

# Download dos PDFs

Inglês  
https://ninamcunha.github.io/professional-resume/pdfs/Nina_Menezes_Cunha_Resume_EN.pdf

Português  
https://ninamcunha.github.io/professional-resume/pdfs/Nina_Menezes_Cunha_Resume_PT.pdf

---

# Preview

Você pode visualizar o currículo diretamente através do PDF:

Inglês  
https://ninamcunha.github.io/professional-resume/pdfs/Nina_Menezes_Cunha_Resume_EN.pdf

Português  
https://ninamcunha.github.io/professional-resume/pdfs/Nina_Menezes_Cunha_Resume_PT.pdf

---

# Funcionalidades

• suporte bilíngue (PT / EN)  
• layout responsivo  
• design pronto para impressão  
• download de PDFs  
• dados do currículo separados da interface  
• deploy com GitHub Pages  
• fácil customização

---

# Stack

React  
TypeScript  
Vite  
TailwindCSS  
GitHub Pages

---

# Estrutura do Projeto

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

# Rodar Localmente

git clone https://github.com/seu-usuario/professional-resume.git

cd professional-resume

npm install

npm run dev

Abrir

http://localhost:5173

---

# Build

npm run build

Preview

npm run preview

---

# Deploy

npm run deploy

Depois ativar GitHub Pages

Settings → Pages

Branch: gh-pages

---

# Como Replicar

1. Clonar o repositório

2. Instalar dependências

npm install

3. Editar conteúdo

src/app/data/resumeEN.ts  
src/app/data/resumePT.ts

4. Trocar logos

src/assets

5. Trocar PDFs

public/pdfs

6. Ajustar base

vite.config.ts

7. Deploy

npm run deploy

---

# Scripts

npm run dev  
npm run build  
npm run preview  
npm run deploy

---

# Licença

MIT

---

# Autor

Nina Menezes Cunha
