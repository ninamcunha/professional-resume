🇺🇸 English | [🇧🇷 Português](./README_PT.md)

# Professional Resume Template

A bilingual professional resume template built with **React, TypeScript, and Vite**, designed to be easily customized and deployed with **GitHub Pages**.

**Live Demo**  
https://ninamcunha.github.io/professional-resume/

**PDF Downloads**

- English:  
  https://ninamcunha.github.io/professional-resume/pdfs/Nina_Menezes_Cunha_Resume_EN.pdf
- Portuguese:  
  https://ninamcunha.github.io/professional-resume/pdfs/Nina_Menezes_Cunha_Resume_PT.pdf

---

## Preview

Add a screenshot to the root of the repository, for example:

```md
![Professional Resume Preview](./preview.png)
```

---

## About

This project started as a resume created in Figma Make and was later reorganized into a cleaner public GitHub repository so it can be reused as a template.

It includes:

- bilingual resume support
- printable layout
- downloadable PDF versions
- GitHub Pages deployment
- structured resume data separated from UI

This repository can be used as:

- your own online resume
- a professional CV template
- a starting point for a public personal profile

---

## Tech Stack

- React
- TypeScript
- Vite
- Tailwind CSS
- GitHub Pages

---

## Project Structure

```text
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
├── README.md
├── README_PT.md
├── package.json
└── vite.config.ts
```

---

## Run Locally

### 1. Clone the repository

```bash
git clone https://github.com/your-username/professional-resume.git
cd professional-resume
```

### 2. Install dependencies

```bash
npm install
```

### 3. Start the development server

```bash
npm run dev
```

### 4. Open in your browser

```text
http://localhost:5173
```

If the browser does not open automatically, copy and paste the local URL shown in the terminal.

---

## Build Locally

To generate a production build:

```bash
npm run build
```

To preview the production build locally:

```bash
npm run preview
```

---

## Deploy to GitHub Pages

Run:

```bash
npm run deploy
```

Then go to:

**Repository → Settings → Pages**

Configure:

- **Source:** Deploy from a branch
- **Branch:** `gh-pages`
- **Folder:** `/(root)`

Your final URL will look like this:

```text
https://your-username.github.io/your-repository-name/
```

---

## How to Replicate This Resume

This section is for anyone who wants to reuse the project for their own resume.

### Step 1 — Clone or fork the repository

You can either:

- fork the repository on GitHub, or
- clone it directly and create your own repository from it

```bash
git clone https://github.com/your-username/professional-resume.git
cd professional-resume
```

### Step 2 — Install dependencies

```bash
npm install
```

### Step 3 — Update the project name

Open `package.json` and change the name, for example:

```json
"name": "my-professional-resume"
```

Then run:

```bash
npm install
```

### Step 4 — Replace the resume content

Edit these files:

```text
src/app/data/resumeEN.ts
src/app/data/resumePT.ts
```

These files contain the structured content for each language, including:

- header
- summary
- experience
- education
- certifications
- skills
- projects/publications

### Step 5 — Replace logos and visual assets

Update the files inside:

```text
src/assets
```

You can replace:

- company logos
- education logos
- certification logos

Keep filenames readable and update imports in `resumeEN.ts` and `resumePT.ts` when needed.

### Step 6 — Replace exported PDFs

Put your final PDFs here:

```text
public/pdfs
```

Example:

```text
public/pdfs/My_Resume_EN.pdf
public/pdfs/My_Resume_PT.pdf
```

Files inside `public/` are served directly by Vite and GitHub Pages.

### Step 7 — Adjust the GitHub Pages base path

Open:

```text
vite.config.ts
```

Make sure this line matches your repository name:

```ts
base: '/professional-resume/',
```

If your repository is called `my-professional-resume`, then change it to:

```ts
base: '/my-professional-resume/',
```

### Step 8 — Install the deploy dependency

If it is not already installed:

```bash
npm install -D gh-pages
```

### Step 9 — Build and deploy

```bash
npm run build
npm run deploy
```

### Step 10 — Enable GitHub Pages

On GitHub, open your repository and go to:

**Settings → Pages**

Then configure:

- **Source:** Deploy from a branch
- **Branch:** `gh-pages`
- **Folder:** `/(root)`

### Step 11 — Open your published resume

Your final URL will look like this:

```text
https://your-username.github.io/your-repository-name/
```

---

## Available Scripts

```bash
npm run dev
npm run build
npm run preview
npm run deploy
```

---

## Notes

- The `public/` folder is exposed at the site root.
- The `gh-pages` branch is created when you run `npm run deploy`.
- If the page opens blank after deployment, the most common cause is an incorrect `base` value in `vite.config.ts`.

---

## Recommended Customization Flow

1. Update `resumeEN.ts`
2. Update `resumePT.ts`
3. Replace logos in `src/assets`
4. Replace PDFs in `public/pdfs`
5. Check `vite.config.ts`
6. Run `npm run build`
7. Run `npm run deploy`

---

## License

MIT is a good default option if you want to keep this project public and reusable.

---

## Author

Originally adapted and organized by **Nina Menezes Cunha**.
