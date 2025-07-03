# 🍕 Food Campus

> MVP para 3° unidade da disciplina de Processos de Software

[![Frontend](https://img.shields.io/badge/Frontend-Production-brightgreen)](https://foodcampusfrontend-production.up.railway.app/)
[![Backend](https://img.shields.io/badge/Backend-API-blue)](https://github.com/vmedei/foodcampus_backend)
[![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-orange)](https://github.com/vmedei/foodcampus_frontend)

## 📋 Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Funcionalidades](#funcionalidades)
- [Tecnologias](#tecnologias)
- [Arquitetura](#arquitetura)
- [Instalação e Uso](#instalação-e-uso)
- [Equipe](#equipe)
- [Documentação](#documentação)
- [Links Úteis](#links-úteis)

## 🎯 Sobre o Projeto

O **Food Campus** é um sistema inovador destinado ao setor de comércio e venda de alimentos no entorno da UFRN. O projeto visa facilitar tanto a busca do estudante por alimentos quanto proporcionar aos ambulantes um ambiente centralizado e seguro para divulgar seus produtos.

### 🎯 Objetivos

- **Para Estudantes**: Facilitar a busca e descoberta de opções alimentares próximas ao campus
- **Para Ambulantes**: Oferecer uma plataforma centralizada para divulgação de produtos
- **Para a Comunidade**: Criar um ecossistema digital que conecte oferta e demanda

## ✨ Funcionalidades

### 🧑‍🎓 Para Estudantes
- Busca por alimentos por localização
- Visualização de cardápios e preços
- Sistema de avaliações e comentários
- Filtros por tipo de comida, preço e distância

### 🛒 Para Ambulantes
- Cadastro e gerenciamento de produtos
- Upload de fotos e descrições
- Controle de disponibilidade
- Dashboard de vendas

## 🛠️ Tecnologias

### Frontend
- **React.js** - Biblioteca para construção de interfaces SPA
- **Next.js** - Framework web baseado em React
- **TypeScript** - Superset do JavaScript com tipagem estática
- **Tailwind CSS** - Framework utilitário para estilização
- **Shadcn UI** - Biblioteca de componentes UI
- **Redux** - Gerenciamento de estado global

### Backend
- **Node.js** - Runtime para executar JavaScript no servidor
- **Express.js** - Framework para criação de APIs REST
- **TypeScript** - Superset do JavaScript com tipagem estática
- **Prisma ORM** - ORM para integração com banco de dados
- **MySQL** - Banco de dados relacional

## 🏗️ Arquitetura

O sistema segue uma arquitetura cliente-servidor tradicional:

```
┌─────────────────┐    HTTP/REST    ┌─────────────────┐
│   Frontend      │ ◄──────────────► │    Backend      │
│   (Next.js)     │                 │   (Express.js)  │
└─────────────────┘                 └─────────────────┘
                                              │
                                              ▼
                                     ┌─────────────────┐
                                     │   MySQL DB      │
                                     └─────────────────┘
```

## 🚀 Instalação e Uso

### Pré-requisitos
- Node.js (versão 18 ou superior)
- npm ou yarn
- MySQL

### Frontend
```bash
# Clone o repositório frontend
git clone https://github.com/vmedei/foodcampus_frontend.git
cd foodcampus_frontend

# Instale as dependências
npm install

# Execute em modo de desenvolvimento
npm run dev
```

### Backend
```bash
# Clone o repositório backend
git clone https://github.com/vmedei/foodcampus_backend.git
cd foodcampus_backend

# Instale as dependências
npm install

# Configure as variáveis de ambiente
cp .env.example .env

# Execute as migrações do banco
npx prisma migrate dev

# Execute em modo de desenvolvimento
npm run dev
```

## 👥 Equipe

### Líder Técnico
- **Vinicius Alves Medeiros** - Fullstack Developer

### Desenvolvedores Frontend
- **Matheus Albert da Silva Araújo**
- **Paulo Daniel Carvalho de Souza**

### Desenvolvedores Backend
- **Chrystian Ruan Inacio de Sousa**
- **Robert Matheus Costa Targino**

## 📚 Documentação

- [📋 Acordo de Trabalho](./docs/Acordo_trabalho.md)
- [🏗️ Arquitetura do Sistema](./docs/Arquitetura.md)
- [👥 Papéis da Equipe](./docs/Papeis.md)
- [📅 Sprint Planning](./docs/Sprint_Planning.md)
- [📊 Fluxos de Usuários](./docs/fluxos-usuarios.pdf)

## 🔗 Links Úteis

### Repositórios
- **Frontend**: [foodcampus_frontend](https://github.com/vmedei/foodcampus_frontend)
- **Backend**: [foodcampus_backend](https://github.com/vmedei/foodcampus_backend)

### Aplicações
- **Frontend (Produção)**: [https://foodcampusfrontend-production.up.railway.app/](https://foodcampusfrontend-production.up.railway.app/)

### Comunicação
- **Canal Oficial**: WhatsApp
- **Reuniões**: Google Meet
- **Horário de Trabalho**: Horário da aula (35N34)

---

## 📄 Licença

Este projeto foi desenvolvido para fins acadêmicos na disciplina de Processos de Software da UFRN.

---

<div align="center">
  <p>Feito com ❤️ pela equipe Food Campus</p>
  <p>UFRN - 2024</p>
</div>