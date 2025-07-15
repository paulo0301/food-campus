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
- **Next.js 15.3.4** - Framework web baseado em React com App Router
- **React 19** - Biblioteca para construção de interfaces SPA
- **TypeScript 5** - Superset do JavaScript com tipagem estática
- **Tailwind CSS 4.1.11** - Framework utilitário para estilização
- **DaisyUI 5.0.46** - Biblioteca de componentes UI baseada em Tailwind
- **Leaflet 1.9.4** - Biblioteca para mapas interativos
- **React Leaflet 5.0.0** - Componentes React para Leaflet
- **Lucide React 0.525.0** - Biblioteca de ícones
- **NextAuth.js 5.0.0-beta.29** - Autenticação para Next.js

### Backend
- **Java 17** - Linguagem de programação
- **Spring Boot 3.5.3** - Framework para desenvolvimento de aplicações Java
- **Spring Security** - Framework de segurança
- **Spring Data JPA** - Persistência de dados
- **MySQL** - Banco de dados relacional
- **MapStruct 1.6.3** - Mapeamento de objetos
- **Lombok** - Redução de código boilerplate
- **JWT (Auth0)** - Autenticação baseada em tokens
- **SpringDoc OpenAPI 2.5.0** - Documentação da API

## 🏗️ Arquitetura

O sistema segue uma arquitetura cliente-servidor tradicional:

```
┌─────────────────┐    HTTP/REST    ┌─────────────────┐
│   Frontend      │ ◄──────────────► │    Backend      │
│   (Next.js)     │                 │  (Spring Boot)  │
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
- Java 17 ou superior
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

# Execute com Gradle
./gradlew bootRun

# Ou compile e execute
./gradlew build
java -jar build/libs/foodcampus-0.0.1-SNAPSHOT.jar
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