[🇺🇸 English](./README.md) | 🇧🇷 Português

# Template de Currículo Profissional

Template de currículo profissional bilíngue feito com **React, TypeScript e Vite**, pronto para customização e deploy com **GitHub Pages**.

**Demo ao vivo**  
https://ninamcunha.github.io/professional-resume/

**Downloads dos PDFs**

- Inglês:  
  https://ninamcunha.github.io/professional-resume/pdfs/Nina_Menezes_Cunha_Resume_EN.pdf
- Português:  
  https://ninamcunha.github.io/professional-resume/pdfs/Nina_Menezes_Cunha_Resume_PT.pdf

---

## Preview

Adicione uma captura de tela na raiz do repositório, por exemplo:

```md
![Preview do Currículo](./preview.png)
```

---

## Sobre o projeto

Este projeto começou como um currículo criado no Figma Make e depois foi reorganizado em um repositório público mais limpo, para poder ser reutilizado como template.

Ele inclui:

- suporte bilíngue
- layout pronto para impressão
- versões em PDF para download
- deploy com GitHub Pages
- conteúdo estruturado separado da interface

Este repositório pode ser usado como:

- seu currículo online
- um template de CV profissional
- base para um perfil público pessoal

---

## Stack utilizada

- React
- TypeScript
- Vite
- Tailwind CSS
- GitHub Pages

---

## Estrutura do projeto

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

## Como rodar localmente

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/professional-resume.git
cd professional-resume
```

### 2. Instale as dependências

```bash
npm install
```

### 3. Inicie o servidor local

```bash
npm run dev
```

### 4. Abra no navegador

```text
http://localhost:5173
```

Se o navegador não abrir sozinho, copie e cole manualmente a URL exibida no terminal.

---

## Como gerar o build localmente

```bash
npm run build
```

Para pré-visualizar o build de produção:

```bash
npm run preview
```

---

## Como fazer o deploy no GitHub Pages

Rode:

```bash
npm run deploy
```

Depois vá em:

**Repositório → Settings → Pages**

Configure:

- **Source:** Deploy from a branch
- **Branch:** `gh-pages`
- **Folder:** `/(root)`

A URL final ficará assim:

```text
https://seu-usuario.github.io/nome-do-repositorio/
```

---

## Como replicar este currículo

Esta seção é para quem quiser reutilizar o projeto com o próprio conteúdo.

### Passo 1 — Fazer fork ou clonar o repositório

Você pode:

- fazer um fork no GitHub, ou
- clonar o repositório e criar um novo repo a partir dele

```bash
git clone https://github.com/seu-usuario/professional-resume.git
cd professional-resume
```

### Passo 2 — Instalar as dependências

```bash
npm install
```

### Passo 3 — Atualizar o nome do projeto

Abra `package.json` e troque o nome do projeto, por exemplo:

```json
"name": "meu-curriculo-profissional"
```

Depois rode:

```bash
npm install
```

### Passo 4 — Substituir o conteúdo do currículo

Edite estes arquivos:

```text
src/app/data/resumeEN.ts
src/app/data/resumePT.ts
```

Esses arquivos concentram o conteúdo estruturado de cada idioma, incluindo:

- header
- summary
- experience
- education
- certifications
- skills
- projects/publications

### Passo 5 — Trocar logos e assets visuais

Atualize os arquivos dentro de:

```text
src/assets
```

Você pode trocar:

- logos de empresas
- logos de instituições de ensino
- logos de certificações

Mantenha nomes de arquivo legíveis e atualize os imports em `resumeEN.ts` e `resumePT.ts` quando necessário.

### Passo 6 — Substituir os PDFs exportados

Coloque seus PDFs finais em:

```text
public/pdfs
```

Exemplo:

```text
public/pdfs/Meu_Curriculo_EN.pdf
public/pdfs/Meu_Curriculo_PT.pdf
```

Tudo que está dentro de `public/` é servido diretamente pelo Vite e pelo GitHub Pages.

### Passo 7 — Ajustar o base path do GitHub Pages

Abra:

```text
vite.config.ts
```

E confira esta linha:

```ts
base: '/professional-resume/',
```

Se o seu repositório tiver outro nome, por exemplo `meu-curriculo-profissional`, altere para:

```ts
base: '/meu-curriculo-profissional/',
```

### Passo 8 — Instalar a dependência de deploy

Se necessário:

```bash
npm install -D gh-pages
```

### Passo 9 — Gerar build e fazer deploy

```bash
npm run build
npm run deploy
```

### Passo 10 — Ativar o GitHub Pages

No GitHub, entre no repositório e vá em:

**Settings → Pages**

Depois configure:

- **Source:** Deploy from a branch
- **Branch:** `gh-pages`
- **Folder:** `/(root)`

### Passo 11 — Abrir o currículo publicado

A URL final ficará assim:

```text
https://seu-usuario.github.io/nome-do-repositorio/
```

---

## Scripts disponíveis

```bash
npm run dev
npm run build
npm run preview
npm run deploy
```

---

## Observações

- A pasta `public/` é exposta na raiz do site.
- A branch `gh-pages` é criada quando você roda `npm run deploy`.
- Se a página abrir em branco depois do deploy, a causa mais comum é um `base` incorreto no `vite.config.ts`.

---

## Fluxo recomendado de customização

1. Atualizar `resumeEN.ts`
2. Atualizar `resumePT.ts`
3. Trocar logos em `src/assets`
4. Substituir PDFs em `public/pdfs`
5. Revisar `vite.config.ts`
6. Rodar `npm run build`
7. Rodar `npm run deploy`

---

## Licença

MIT costuma ser uma boa opção se a ideia for manter o projeto público e reutilizável.

---

## Autor

Originalmente adaptado e organizado por **Nina Menezes Cunha**.
