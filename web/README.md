# NLW-Agents

---

## 🇧🇷 Português

### Sobre o Projeto

Projeto desenvolvido durante o evento NLW (Next Level Week) da Rocketseat, focado em criar uma aplicação web para gerenciamento de salas e perguntas com funcionalidades de áudio.

### 🚀 Tecnologias

#### Core

- **React 19** - Biblioteca principal para interface
- **TypeScript** - Tipagem estática
- **Vite** - Build tool e dev server

#### UI/UX

- **Tailwind CSS 4** - Framework CSS utilitário
- **Radix UI** - Componentes acessíveis
- **Lucide React** - Ícones
- **Class Variance Authority** - Gerenciamento de variantes de componentes

#### Estado e Formulários

- **React Query (TanStack Query)** - Gerenciamento de estado do servidor
- **React Hook Form** - Formulários performáticos
- **Zod** - Validação de schemas

#### Roteamento

- **React Router DOM** - Navegação SPA

#### Utilitários

- **Day.js** - Manipulação de datas
- **CLSX** - Composição de classes CSS
- **Tailwind Merge** - Merge inteligente de classes

#### Desenvolvimento

- **Biome** - Linter e formatter
- **Ultracite** - Configuração de linting

### 📁 Estrutura do Projeto

```
src/
├── components/          # Componentes reutilizáveis
│   ├── ui/            # Componentes base (Radix UI)
│   └── *.tsx          # Componentes específicos
├── http/              # Camada de comunicação HTTP
│   ├── types/         # Tipos TypeScript para API
│   └── use-*.ts       # Hooks customizados para API
├── lib/               # Utilitários e helpers
├── pages/             # Páginas da aplicação
└── app.tsx            # Componente raiz
```

### 🛠️ Setup e Instalação

#### Pré-requisitos

- Node.js 18+
- npm ou yarn

#### Instalação

```bash
# Clone o repositório
git clone <repository-url>
cd NLW-Agents/web

# Instale as dependências
npm install

# Execute o projeto em modo desenvolvimento
npm run dev

# Build para produção
npm run build

# Preview do build
npm run preview
```

### 🔧 Configuração

#### Variáveis de Ambiente

Crie um arquivo `.env` na raiz do projeto:

```env
# API Configuration
VITE_API_URL=your-api-url
```

#### Scripts Disponíveis

- `npm run dev` - Inicia o servidor de desenvolvimento
- `npm run build` - Gera build de produção
- `npm run preview` - Preview do build local

### 🎯 Funcionalidades

- ✅ Criação de salas
- ✅ Gerenciamento de perguntas
- ✅ Gravação de áudio
- ✅ Interface responsiva
- ✅ Validação de formulários
- ✅ Gerenciamento de estado otimizado

### 📝 Padrões de Projeto

- **Componentes Funcionais** - Uso de hooks React
- **Custom Hooks** - Lógica reutilizável em hooks
- **TypeScript** - Tipagem estática completa
- **Atomic Design** - Estrutura de componentes
- **React Query** - Cache e sincronização de dados
- **Formulários Controlados** - React Hook Form + Zod

---

## 🇺🇸 English

### About the Project

Project developed during Rocketseat's NLW (Next Level Week) event, focused on creating a web application for room and question management with audio features.

### 🚀 Technologies

#### Core

- **React 19** - Main interface library
- **TypeScript** - Static typing
- **Vite** - Build tool and dev server

#### UI/UX

- **Tailwind CSS 4** - Utility CSS framework
- **Radix UI** - Accessible components
- **Lucide React** - Icons
- **Class Variance Authority** - Component variant management

#### State & Forms

- **React Query (TanStack Query)** - Server state management
- **React Hook Form** - Performant forms
- **Zod** - Schema validation

#### Routing

- **React Router DOM** - SPA navigation

#### Utilities

- **Day.js** - Date manipulation
- **CLSX** - CSS class composition
- **Tailwind Merge** - Smart class merging

#### Development

- **Biome** - Linter and formatter
- **Ultracite** - Linting configuration

### 📁 Project Structure

```
src/
├── components/          # Reusable components
│   ├── ui/            # Base components (Radix UI)
│   └── *.tsx          # Specific components
├── http/              # HTTP communication layer
│   ├── types/         # TypeScript types for API
│   └── use-*.ts       # Custom API hooks
├── lib/               # Utilities and helpers
├── pages/             # Application pages
└── app.tsx            # Root component
```

### 🛠️ Setup and Installation

#### Prerequisites

- Node.js 18+
- npm or yarn

#### Installation

```bash
# Clone the repository
git clone <repository-url>
cd NLW-Agents/web

# Install dependencies
npm install

# Run the project in development mode
npm run dev

# Build for production
npm run build

# Preview the build
npm run preview
```

### 🔧 Configuration

#### Environment Variables

Create a `.env` file in the project root:

```env
# API Configuration
VITE_API_URL=your-api-url
```

#### Available Scripts

- `npm run dev` - Starts development server
- `npm run build` - Generates production build
- `npm run preview` - Local build preview

### 🎯 Features

- ✅ Room creation
- ✅ Question management
- ✅ Audio recording
- ✅ Responsive interface
- ✅ Form validation
- ✅ Optimized state management

### 📝 Project Patterns

- **Functional Components** - React hooks usage
- **Custom Hooks** - Reusable logic in hooks
- **TypeScript** - Complete static typing
- **Atomic Design** - Component structure
- **React Query** - Cache and data synchronization
- **Controlled Forms** - React Hook Form + Zod
