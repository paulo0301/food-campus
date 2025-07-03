# 🏗️ Arquitetura do Sistema Food Campus

> Documentação técnica detalhada da arquitetura e tecnologias utilizadas no projeto

## 📚 Índice

1. [Visão Geral](#visão-geral)
2. [Tecnologias](#tecnologias)
3. [Componentes](#componentes)
4. [Diagrama da Arquitetura](#diagrama-da-arquitetura)
5. [Fluxo de Dados](#fluxo-de-dados)
6. [Padrões Utilizados](#padrões-utilizados)
7. [Segurança](#segurança)
8. [Deploy e Infraestrutura](#deploy-e-infraestrutura)

## 🎯 Visão Geral

O Food Campus segue uma arquitetura **cliente-servidor** moderna, com separação clara entre frontend e backend. O sistema foi projetado para ser escalável, manutenível e seguir as melhores práticas de desenvolvimento web.

### 🏛️ Princípios Arquiteturais

- **Separação de Responsabilidades**: Frontend e backend independentes
- **API-First**: Backend expõe APIs REST bem documentadas
- **Componentização**: Frontend modular com componentes reutilizáveis
- **Escalabilidade**: Arquitetura preparada para crescimento
- **Manutenibilidade**: Código limpo e bem documentado

## 🛠️ Tecnologias

### 🖥️ Frontend

| Tecnologia | Versão | Propósito |
|------------|--------|-----------|
| **React.js** | 18.x | Biblioteca para construção de interfaces SPA |
| **Next.js** | 14.x | Framework web baseado em React com SSR |
| **TypeScript** | 5.x | Superset do JavaScript com tipagem estática |
| **Tailwind CSS** | 3.x | Framework utilitário para estilização |
| **Shadcn UI** | Latest | Biblioteca de componentes UI modernos |
| **Redux Toolkit** | 2.x | Gerenciamento de estado global |
| **React Query** | 5.x | Gerenciamento de estado do servidor |

### 🔧 Backend

| Tecnologia | Versão | Propósito |
|------------|--------|-----------|
| **Node.js** | 18.x | Runtime para executar JavaScript no servidor |
| **Express.js** | 4.x | Framework para criação de APIs REST |
| **TypeScript** | 5.x | Superset do JavaScript com tipagem estática |
| **Prisma ORM** | 5.x | ORM para integração com banco de dados |
| **MySQL** | 8.x | Banco de dados relacional |
| **JWT** | Latest | Autenticação e autorização |
| **bcrypt** | 5.x | Criptografia de senhas |

### 🗄️ Banco de Dados

| Tecnologia | Versão | Propósito |
|------------|--------|-----------|
| **MySQL** | 8.x | Banco de dados principal |
| **Prisma** | 5.x | ORM e migrations |
| **Redis** | 7.x | Cache e sessões (futuro) |

## 🧩 Componentes

### 📱 Frontend (Next.js)

```
src/
├── components/          # Componentes reutilizáveis
│   ├── ui/             # Componentes base (Shadcn)
│   ├── forms/          # Formulários
│   └── layout/         # Componentes de layout
├── pages/              # Páginas da aplicação
│   ├── api/            # API routes (Next.js)
│   ├── auth/           # Páginas de autenticação
│   ├── products/       # Páginas de produtos
│   └── profile/        # Páginas de perfil
├── hooks/              # Custom hooks
├── services/           # Serviços de API
├── store/              # Estado global (Redux)
├── types/              # Definições TypeScript
└── utils/              # Utilitários
```

### ⚙️ Backend (Express.js)

```
src/
├── controllers/        # Controladores das rotas
├── services/          # Lógica de negócio
├── models/            # Modelos de dados
├── routes/            # Definição de rotas
├── middleware/        # Middlewares customizados
├── utils/             # Utilitários
├── config/            # Configurações
└── types/             # Definições TypeScript
```

## 🏗️ Diagrama da Arquitetura

```mermaid
graph TB
    subgraph "Cliente"
        A[Browser] --> B[Next.js App]
        B --> C[React Components]
        B --> D[Redux Store]
    end
    
    subgraph "Frontend (Railway)"
        E[Next.js Server]
        F[Static Assets]
    end
    
    subgraph "Backend (Railway)"
        G[Express.js API]
        H[Controllers]
        I[Services]
        J[Middleware]
    end
    
    subgraph "Banco de Dados"
        K[MySQL Database]
        L[Prisma ORM]
    end
    
    subgraph "Serviços Externos"
        M[File Storage]
        N[Email Service]
        O[Payment Gateway]
    end
    
    A --> E
    E --> G
    G --> L
    L --> K
    G --> M
    G --> N
    G --> O
    
    style A fill:#e1f5fe
    style E fill:#f3e5f5
    style G fill:#e8f5e8
    style K fill:#fff3e0
```

## 🔄 Fluxo de Dados

### 1. **Autenticação**
```
Cliente → Frontend → Backend → Database
   ↑         ↓         ↓         ↓
   ←─────────←─────────←─────────←
```

### 2. **Busca de Produtos**
```
Cliente → Frontend → Backend → Database
   ↑         ↓         ↓         ↓
   ←─────────←─────────←─────────←
```

### 3. **Criação de Pedido**
```
Cliente → Frontend → Backend → Database
   ↑         ↓         ↓         ↓
   ←─────────←─────────←─────────←
```

## 🎨 Padrões Utilizados

### 🏗️ Padrões de Arquitetura

- **MVC (Model-View-Controller)**: Separação de responsabilidades
- **Repository Pattern**: Abstração do acesso a dados
- **Service Layer**: Lógica de negócio centralizada
- **Middleware Pattern**: Processamento de requisições

### 📝 Padrões de Código

- **Clean Code**: Código limpo e legível
- **DRY (Don't Repeat Yourself)**: Evitar duplicação
- **SOLID Principles**: Princípios de design orientado a objetos
- **TypeScript**: Tipagem estática para maior segurança

## 🔒 Segurança

### 🛡️ Medidas Implementadas

- **JWT Authentication**: Tokens seguros para autenticação
- **Password Hashing**: Senhas criptografadas com bcrypt
- **CORS**: Configuração adequada para requisições cross-origin
- **Input Validation**: Validação de dados de entrada
- **SQL Injection Protection**: Uso de ORM com prepared statements

### 🔐 Práticas de Segurança

- **HTTPS**: Comunicação criptografada
- **Environment Variables**: Configurações sensíveis em variáveis de ambiente
- **Rate Limiting**: Proteção contra ataques de força bruta
- **Input Sanitization**: Limpeza de dados de entrada

## 🚀 Deploy e Infraestrutura

### ☁️ Plataformas de Deploy

| Serviço | Propósito | URL |
|---------|-----------|-----|
| **Railway** | Frontend (Produção) | https://foodcampusfrontend-production.up.railway.app/ |
| **Railway** | Backend (Produção) | Em desenvolvimento |
| **GitHub** | Versionamento | https://github.com/vmedei/foodcampus_* |

### 🔧 Configuração de Ambiente

#### Frontend
```bash
# Variáveis de ambiente
NEXT_PUBLIC_API_URL=https://api.foodcampus.com
NEXT_PUBLIC_APP_URL=https://foodcampus.com
```

#### Backend
```bash
# Variáveis de ambiente
DATABASE_URL=mysql://user:pass@host:port/db
JWT_SECRET=your-secret-key
PORT=3001
NODE_ENV=production
```

### 📊 Monitoramento

- **Logs**: Railway logs para debugging
- **Performance**: Monitoramento de performance via Railway
- **Uptime**: Verificação de disponibilidade
- **Errors**: Captura e análise de erros

---

## 📈 Roadmap Técnico

### 🎯 Próximas Implementações

- [ ] **Cache Layer**: Implementação de Redis para cache
- [ ] **CDN**: Distribuição de conteúdo estático
- [ ] **Microservices**: Separação em serviços menores
- [ ] **Docker**: Containerização da aplicação
- [ ] **CI/CD**: Pipeline automatizado de deploy

### 🔮 Melhorias Futuras

- [ ] **WebSockets**: Comunicação em tempo real
- [ ] **PWA**: Progressive Web App
- [ ] **Mobile App**: Aplicativo nativo
- [ ] **Analytics**: Métricas de uso
- [ ] **A/B Testing**: Testes de usabilidade

---

> **Última atualização**: Dezembro 2024  
> **Responsável**: Equipe de Desenvolvimento Food Campus
