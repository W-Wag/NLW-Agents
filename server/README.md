# NLW-Agents

[🇧🇷 Português](#português) | [🇺🇸 English](#english)

---

## 🇧🇷 Português

### Sobre o Projeto

**NLW-Agents** é um projeto desenvolvido durante o evento NLW (Next Level Week) da Rocketseat. O projeto consiste em uma API backend para gerenciamento de agentes de IA, permitindo a criação de salas, envio de perguntas e processamento de áudio.

### 🛠️ Tecnologias Utilizadas

- **Runtime**: Node.js com TypeScript
- **Framework**: Fastify (API REST)
- **Banco de Dados**: PostgreSQL com pgvector
- **ORM**: Drizzle ORM
- **Validação**: Zod
- **IA**: Google Gemini AI
- **Linting/Formatting**: Biome + Ultracite
- **Containerização**: Docker + Docker Compose

### 🏗️ Arquitetura e Padrões

- **Arquitetura**: API REST com Fastify
- **Validação**: Schema validation com Zod
- **Banco de Dados**: Migrations com Drizzle Kit
- **Estrutura**: Organização modular por funcionalidades
- **Type Safety**: TypeScript com type providers

### 🚀 Setup e Configuração

#### Pré-requisitos

- Node.js 18+
- Docker e Docker Compose
- Conta no Google AI Studio (para API key do Gemini)

#### 1. Clone o repositório

```bash
git clone <repository-url>
cd NLW-Agents/server
```

#### 2. Configure as variáveis de ambiente

Crie um arquivo `.env` na raiz do projeto:

```env
PORT=3333
DATABASE_URL=postgresql://docker:docker@localhost:5433/agents
GEMINI_API_KEY=sua_api_key_do_gemini
```

#### 3. Inicie o banco de dados

```bash
docker-compose up -d
```

#### 4. Instale as dependências

```bash
npm install
```

#### 5. Execute as migrations

```bash
npm run db:generate
npm run db:migrate
```

#### 6. Inicie o servidor

```bash
npm run dev
```

### 📋 Scripts Disponíveis

- `npm run dev` - Inicia o servidor em modo desenvolvimento
- `npm run start` - Inicia o servidor em produção
- `npm run db:generate` - Gera migrations do Drizzle
- `npm run db:migrate` - Executa migrations
- `npm run db:seed` - Popula o banco com dados iniciais

### 🔗 Endpoints da API

- `GET /health` - Health check
- `GET /rooms` - Lista todas as salas
- `POST /rooms` - Cria uma nova sala
- `POST /questions` - Cria uma nova pergunta
- `GET /rooms/:id/questions` - Lista perguntas de uma sala
- `POST /upload-audio` - Upload e processamento de áudio

---

## 🇺🇸 English

### About the Project

**NLW-Agents** is a project developed during Rocketseat's NLW (Next Level Week) event. The project consists of a backend API for managing AI agents, allowing room creation, question submission, and audio processing.

### 🛠️ Technologies Used

- **Runtime**: Node.js with TypeScript
- **Framework**: Fastify (REST API)
- **Database**: PostgreSQL with pgvector
- **ORM**: Drizzle ORM
- **Validation**: Zod
- **AI**: Google Gemini AI
- **Linting/Formatting**: Biome + Ultracite
- **Containerization**: Docker + Docker Compose

### 🏗️ Architecture and Patterns

- **Architecture**: REST API with Fastify
- **Validation**: Schema validation with Zod
- **Database**: Migrations with Drizzle Kit
- **Structure**: Modular organization by features
- **Type Safety**: TypeScript with type providers

### 🚀 Setup and Configuration

#### Prerequisites

- Node.js 18+
- Docker and Docker Compose
- Google AI Studio account (for Gemini API key)

#### 1. Clone the repository

```bash
git clone <repository-url>
cd NLW-Agents/server
```

#### 2. Configure environment variables

Create a `.env` file in the project root:

```env
PORT=3333
DATABASE_URL=postgresql://docker:docker@localhost:5433/agents
GEMINI_API_KEY=your_gemini_api_key
```

#### 3. Start the database

```bash
docker-compose up -d
```

#### 4. Install dependencies

```bash
npm install
```

#### 5. Run migrations

```bash
npm run db:generate
npm run db:migrate
```

#### 6. Start the server

```bash
npm run dev
```

### 📋 Available Scripts

- `npm run dev` - Starts the server in development mode
- `npm run start` - Starts the server in production
- `npm run db:generate` - Generates Drizzle migrations
- `npm run db:migrate` - Runs migrations
- `npm run db:seed` - Seeds the database with initial data

### 🔗 API Endpoints

- `GET /health` - Health check
- `GET /rooms` - List all rooms
- `POST /rooms` - Create a new room
- `POST /questions` - Create a new question
- `GET /rooms/:id/questions` - List questions from a room
- `POST /upload-audio` - Upload and process audio

---

## 📄 License

MIT License
