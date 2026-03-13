# 📄 Currículo Profissional - React/TypeScript

<div align="center">

![React](https://img.shields.io/badge/React-18.3.1-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.1.12-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-6.3.5-646CFF?style=for-the-badge&logo=vite&logoColor=white)

**Currículo profissional bilíngue (PT/EN) com exportação para PDF de alta fidelidade**

[🌐 Demo ao Vivo](#) | [📥 Baixar PDF](#) | [🐛 Reportar Bug](../../issues) | [✨ Solicitar Feature](../../issues)

</div>

---

## 📋 Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades](#-funcionalidades)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Estrutura do Projeto](#-estrutura-do-projeto)
- [Instalação](#-instalação)
- [Como Usar](#-como-usar)
- [Customização](#-customização)
- [Exportação para PDF](#-exportação-para-pdf)
- [Deploy](#-deploy)
- [Licença](#-licença)

---

## 🎯 Sobre o Projeto

Este é um **currículo profissional interativo** desenvolvido em React/TypeScript, projetado especificamente para profissionais de tecnologia. O projeto oferece uma experiência visual moderna e responsiva, com funcionalidade de alternância de idiomas (Português/Inglês) e exportação para PDF com **100% de fidelidade visual**.

### 🎨 Design & Layout

- **Duas páginas perfeitamente estruturadas** - Layout otimizado para distribuição de conteúdo
- **Cores profissionais** - Títulos em vermelho escuro/vinho (`#7f1d1d`), destaques em laranja (`#ea580c`)
- **Ícones integrados** - Biblioteca Lucide React para elementos visuais consistentes
- **Linhas tracejadas** - Separadores elegantes entre seções
- **Espaçamento inteligente** - Ajustes específicos por idioma para otimizar a distribuição visual

### 📱 Responsividade

- **Mobile-First** - Layout adaptado para celulares e tablets
- **Desktop Otimizado** - Zoom de 125% aplicado apenas em telas grandes para melhor legibilidade
- **Impressão Perfeita** - CSS dedicado para garantir formatação impecável em PDFs

---

## ✨ Funcionalidades

### 🌍 Sistema Bilíngue Completo

- **Alternância PT/EN** - Botão no canto superior direito com ícone de idiomas
- **Conteúdo Dinâmico** - Todos os textos, seções e informações mudam instantaneamente
- **Dados Separados** - Arquivos independentes (`resumePT.ts` e `resumeEN.ts`)
- **Nomes de Arquivo Diferenciados** - PDFs exportados com nomes específicos por idioma

### 📥 Exportação para PDF

- **Alta Fidelidade** - 100% de correspondência visual entre tela e PDF
- **Duas Páginas Exatas** - Distribuição automática e otimizada do conteúdo
- **Print CSS Avançado** - Media queries específicas para impressão
- **window.print()** - Solução nativa sem dependências externas pesadas
- **Nomes Inteligentes** - Arquivos salvos como `Curriculo_Nina_Menezes_Cunha.pdf` (PT) ou `Resume_Nina_Menezes_Cunha.pdf` (EN)

### 📊 Seções do Currículo

1. **Header** - Nome, título, email, LinkedIn, GitHub, portfolio
2. **Resumo Profissional** - Apresentação executiva
3. **Experiência** - 6 posições com logos, datas, localização e descrições
4. **Publicações & Projetos** - 7 itens destacados com links clicáveis
5. **Educação** - 4 instituições com logos e detalhes
6. **Certificações** - 10 certificados com instituições, datas e credenciais
7. **Habilidades** - Categorias com ícones dinâmicos

### 🎨 Layout Inteligente

- **Desktop**: Layout de 2 colunas (experiência/publicações à esquerda, resumo/educação/skills/certificações à direita)
- **Mobile**: Layout em coluna única com ordem otimizada
- **Ajustes por Idioma**: Espaçamentos específicos (PT: 0.95rem, EN: 0.5rem nas experiências)

---

## 🛠 Tecnologias Utilizadas

### Core

| Tecnologia | Versão | Descrição |
|------------|--------|-----------|
| **React** | 18.3.1 | Biblioteca JavaScript para interfaces |
| **TypeScript** | 5.x | Superset tipado do JavaScript |
| **Vite** | 6.3.5 | Build tool moderna e rápida |
| **Tailwind CSS** | 4.1.12 | Framework CSS utility-first |

### Bibliotecas Principais

| Biblioteca | Versão | Uso no Projeto |
|------------|--------|----------------|
| **lucide-react** | 0.487.0 | Ícones SVG (Mail, LinkedIn, GitHub, etc.) |
| **@radix-ui/** | Várias | Componentes UI acessíveis (base) |
| **class-variance-authority** | 0.7.1 | Gerenciamento de classes CSS |
| **tailwind-merge** | 3.2.0 | Mesclagem inteligente de classes Tailwind |

### Funcionalidades Extras

- **react-router** (7.13.0) - Roteamento (caso necessário para expansão)
- **motion** (12.23.24) - Animações suaves
- **date-fns** (3.6.0) - Manipulação de datas
- **sonner** (2.0.3) - Notificações toast

---

## 📁 Estrutura do Projeto

```
📦 professional-resume
├── 📂 src
│   ├── 📂 app
│   │   ├── 📄 App.tsx                    # Componente principal com lógica de idiomas e PDF
│   │   ├── 📂 components
│   │   │   ├── 📄 Resume.tsx             # Componente do currículo com layouts mobile/desktop
│   │   │   ├── 📄 ResumePDF.tsx          # [Legado] Componente anterior de PDF
│   │   │   ├── 📂 figma
│   │   │   │   └── 📄 ImageWithFallback.tsx  # [Sistema] Componente de imagens
│   │   │   └── 📂 ui                     # Componentes UI (Radix + Tailwind)
│   │   │       ├── 📄 button.tsx
│   │   │       ├── 📄 card.tsx
│   │   │       └── ... (50+ componentes)
│   │   └── 📂 data
│   │       ├── 📄 resumePT.ts            # Dados do currículo em português
│   │       ├── 📄 resumeEN.ts            # Dados do currículo em inglês
│   │       └── 📄 resume.ts              # [Legado] Dados antigos
│   └── 📂 styles
│       ├── 📄 index.css                  # CSS global
│       ├── 📄 tailwind.css               # Configurações Tailwind
│       ├── 📄 theme.css                  # Tokens de tema
│       └── 📄 fonts.css                  # Importações de fontes
├── 📄 package.json                       # Dependências e scripts
├── 📄 vite.config.ts                     # Configuração do Vite
├── 📄 postcss.config.mjs                 # Configuração do PostCSS
└── 📄 README.md                          # Este arquivo
```

### 🗂 Arquivos Principais

#### **`/src/app/App.tsx`**
- Componente raiz da aplicação
- Gerencia estado de idioma (`pt` | `en`)
- Implementa função `downloadPDF()` com `window.print()`
- Aplica zoom de 125% no desktop (`md:scale-125`)
- Define nome do arquivo PDF dinamicamente

#### **`/src/app/components/Resume.tsx`**
- Componente principal do currículo
- Recebe dados via props tipadas (`ResumeProps`)
- Contém 2 layouts: mobile (`.md:hidden`) e desktop (`.hidden.md:grid`)
- Ícones dinâmicos baseados em categorias
- Estilos de impressão com `print:` utilities

#### **`/src/app/data/resumePT.ts` e `/src/app/data/resumeEN.ts`**
- Objetos TypeScript com todo o conteúdo
- Estruturas: `header`, `summary`, `experiences`, `education`, `skillCategories`, `publications`, `certifications`
- Logos das empresas/instituições em base64 ou URLs

---

## 🚀 Instalação

### Pré-requisitos

- **Node.js** 18+ ([Download](https://nodejs.org/))
- **pnpm** (recomendado) ou npm/yarn

```bash
# Instalar pnpm (se não tiver)
npm install -g pnpm
```

### Passos de Instalação

1. **Clone o repositório**

```bash
git clone https://github.com/seu-usuario/professional-resume.git
cd professional-resume
```

2. **Instale as dependências**

```bash
pnpm install
```

3. **Inicie o servidor de desenvolvimento**

```bash
pnpm dev
```

4. **Abra no navegador**

```
http://localhost:5173
```

---

## 💻 Como Usar

### 1️⃣ Alternar Idiomas

Clique no botão **PT/EN** no canto superior direito do currículo. O conteúdo mudará instantaneamente.

### 2️⃣ Exportar para PDF

**Opção 1: Botão de Download** (se implementado)
- Clique no botão de download
- O navegador abrirá a caixa de diálogo de impressão
- Selecione "Salvar como PDF"

**Opção 2: Manual**
```bash
Ctrl+P (Windows/Linux) ou Cmd+P (Mac)
```

### 3️⃣ Visualizar no Desktop

O currículo automaticamente aplica **zoom de 125%** em telas grandes (≥768px) para melhor legibilidade. No mobile, permanece 100%.

### 4️⃣ Visualizar no Mobile

O layout se adapta para uma coluna única com:
- Cada link de contato em linha separada
- Seções empilhadas verticalmente
- Espaçamentos otimizados

---

## 🎨 Customização

### Alterar Dados Pessoais

Edite os arquivos `/src/app/data/resumePT.ts` e `/src/app/data/resumeEN.ts`:

```typescript
export const resumePT = {
  header: {
    name: "SEU NOME",
    title: "Seu Título Profissional",
    email: "seu.email@example.com",
    linkedin: "https://linkedin.com/in/seu-perfil",
    github: "https://github.com/seu-usuario",
    portfolio: "https://seu-portfolio.com"
  },
  summary: "Seu resumo profissional aqui...",
  experiences: [
    {
      role: "Cargo",
      company: "Empresa",
      period: "Jan 2023 - Atual",
      location: "Cidade, País",
      description: ["Responsabilidade 1", "Responsabilidade 2"],
      logo: "URL_OU_BASE64"
    }
  ],
  // ... continuar com outras seções
};
```

### Mudar Cores

Edite `/src/styles/theme.css` ou use classes Tailwind diretamente:

```css
/* Cor principal dos títulos */
.text-red-900 → Alterar para .text-blue-900

/* Cor de destaque */
.text-orange-600 → Alterar para .text-green-600

/* Bordas */
.border-red-900 → Alterar para .border-blue-900
```

### Ajustar Espaçamentos

No arquivo `/src/app/App.tsx`, dentro da tag `<style>`:

```css
/* Espaçamento entre experiências (PT) */
[data-language="pt"] #resume-content > div > div > section:nth-child(2) > div > div {
  margin-bottom: 0.95rem; /* Ajustar valor */
}

/* Espaçamento entre experiências (EN) */
[data-language="en"] #resume-content > div > div > section:nth-child(2) > div > div {
  margin-bottom: 0.5rem; /* Ajustar valor */
}
```

### Adicionar Novas Seções

1. Adicione os dados em `resumePT.ts` e `resumeEN.ts`
2. Crie a estrutura JSX em `Resume.tsx`
3. Adicione ícones da biblioteca `lucide-react`
4. Estilize com Tailwind CSS

---

## 📄 Exportação para PDF

### Como Funciona

O sistema usa **`window.print()`** combinado com **CSS de impressão** para gerar PDFs:

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

### CSS de Impressão

Classes Tailwind com prefixo `print:`:

```jsx
<div className="print:shadow-none print:max-w-none print:p-3 print:m-0">
  <button className="print:hidden">Botão que não aparece no PDF</button>
</div>
```

### Otimizações

- **`@page { size: A4; margin: 0; }`** - Define tamanho exato da página
- **`print:scale-100`** - Remove zoom do desktop no PDF
- **Quebras de página** - Evitadas com espaçamentos ajustados
- **Cores mantidas** - `-webkit-print-color-adjust: exact`

### Solução de Problemas

**Problema**: PDF aparece em mais de 2 páginas
- **Solução**: Ajustar espaçamentos específicos por idioma

**Problema**: Cores não aparecem no PDF
- **Solução**: Adicionar `-webkit-print-color-adjust: exact;` no CSS

**Problema**: Layout quebrado no PDF
- **Solução**: Verificar classes `print:` e media query `@media print`

---

## 🌐 Deploy

### Opções de Deploy

#### **Vercel** (Recomendado)

```bash
# Instalar CLI da Vercel
pnpm install -g vercel

# Deploy
vercel
```

#### **Netlify**

```bash
# Build
pnpm build

# Arraste a pasta 'dist' no Netlify Drop
```

#### **GitHub Pages**

1. Adicione ao `vite.config.ts`:

```typescript
export default defineConfig({
  base: '/professional-resume/', // Nome do seu repositório
  // ... outras configs
});
```

2. Adicione script ao `package.json`:

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

## 📦 Scripts Disponíveis

| Comando | Descrição |
|---------|-----------|
| `pnpm dev` | Inicia servidor de desenvolvimento |
| `pnpm build` | Cria build de produção na pasta `dist/` |
| `pnpm preview` | Preview do build de produção |

---

## 🎓 Detalhes Técnicos

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

### Responsividade Breakpoints

- **Mobile**: `< 768px` - Layout em coluna única
- **Desktop**: `≥ 768px` (`.md:`) - Layout 2 colunas + zoom 125%
- **Print**: Media query `@media print` - Layout otimizado para PDF

### Ícones Dinâmicos

```typescript
const getSkillIcon = (title: string) => {
  const lowerTitle = title.toLowerCase();
  if (lowerTitle.includes('programm')) return <Database />;
  if (lowerTitle.includes('data')) return <Cpu />;
  if (lowerTitle.includes('machine')) return <Briefcase />;
  // ... mais condições
  return <Code />; // ícone padrão
};
```

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para:

1. Fazer um **Fork** do projeto
2. Criar uma **Branch** para sua feature (`git checkout -b feature/NovaFuncionalidade`)
3. **Commit** suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4. **Push** para a Branch (`git push origin feature/NovaFuncionalidade`)
5. Abrir um **Pull Request**

---

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 👤 Autor

**Nina Menezes Cunha**

- LinkedIn: [nina-menezes-cunha](https://linkedin.com/in/nina-menezes-cunha)
- GitHub: [@ninamenezes](https://github.com/ninamenezes)
- Portfolio: [ninamenezes.com](https://ninamenezes.com)

---

## 🙏 Agradecimentos

- [Lucide Icons](https://lucide.dev/) - Biblioteca de ícones
- [Tailwind CSS](https://tailwindcss.com/) - Framework CSS
- [Radix UI](https://www.radix-ui.com/) - Componentes primitivos
- [Vite](https://vitejs.dev/) - Build tool

---

<div align="center">

**Feito com ❤️ e React**

⭐ Se este projeto te ajudou, considere dar uma estrela!

</div>
