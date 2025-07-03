# 📅 Sprint Planning - Food Campus

> Planejamento detalhado das sprints e acompanhamento do progresso do projeto

## 🎯 Visão Geral do Projeto

**Objetivo Geral**: Desenvolver um sistema completo para conectar estudantes e ambulantes no entorno da UFRN, facilitando a busca por alimentos e a divulgação de produtos.

**Duração Total**: 4 Sprints  
**Metodologia**: Scrum  
**Equipe**: 5 desenvolvedores

---

## 📊 Sprint 1: Fundação e Planejamento

### 🎯 **Objetivo**
Entregar documentação completa e infraestrutura técnica para o desenvolvimento

### ✅ **Metas de Entrega**
- [x] **Organização da equipe**
  - Definição de papéis e responsabilidades
  - Estabelecimento de acordos de trabalho
  - Configuração de canais de comunicação

- [x] **Infraestrutura técnica**
  - Configuração dos repositórios (Frontend/Backend)
  - Setup do ambiente de desenvolvimento
  - Configuração de ferramentas de CI/CD

- [x] **Backlog e planejamento das sprints**
  - Criação do Product Backlog
  - Priorização de histórias de usuário
  - Estimativa de story points

- [x] **Sprint planning**
  - Definição de critérios de aceitação
  - Distribuição de tarefas
  - Estabelecimento de Definition of Done


## 🚀 Sprint 2: Cadastros e Autenticação

### 🎯 **Objetivo**
Permitir cadastro completo de usuários e produtos, estabelecendo a base do sistema

### 📋 **Metas de Entrega**

#### 👤 **Cadastro de Usuário Comum (Comprador)**
- [ ] **Funcionalidades**:
  - Formulário de cadastro com validação
  - Sistema de autenticação JWT
  - Perfil do usuário com informações básicas
  - Recuperação de senha

- [ ] **Critérios de Aceitação**:
  - Usuário consegue se cadastrar com email e senha
  - Validação de dados obrigatórios
  - Confirmação de email
  - Login/logout funcionando

#### 🛒 **Cadastro de Vendedor**
- [ ] **Funcionalidades**:
  - Formulário específico para vendedores
  - Validação de documentos
  - Aprovação manual (futuro)
  - Dashboard básico do vendedor

- [ ] **Critérios de Aceitação**:
  - Vendedor consegue se cadastrar
  - Campos específicos para vendedores
  - Status de aprovação
  - Acesso ao dashboard

#### 📦 **Cadastro de Produtos**
- [ ] **Funcionalidades**:
  - Formulário de cadastro de produtos
  - Upload de imagens
  - Categorização de produtos
  - Controle de disponibilidade

- [ ] **Critérios de Aceitação**:
  - Vendedor consegue cadastrar produtos
  - Imagens são salvas corretamente
  - Produtos aparecem no sistema
  - Controle de estoque básico


## 🎨 Sprint 3: Funcionalidades Principais

### 🎯 **Objetivo**
Entregar o fluxo principal de uso do sistema, permitindo busca e pedidos

### 📋 **Metas de Entrega**

#### 🏠 **Vitrine de Produtos (Tela Home)**
- [ ] **Funcionalidades**:
  - Listagem de produtos com filtros
  - Busca por nome e categoria
  - Ordenação por preço, distância, avaliação
  - Paginação de resultados

- [ ] **Critérios de Aceitação**:
  - Produtos são exibidos corretamente
  - Filtros funcionam adequadamente
  - Interface responsiva
  - Performance otimizada

#### 🛍️ **Sistema de Reserva/Pedido**
- [ ] **Funcionalidades**:
  - Carrinho de compras
  - Processo de checkout
  - Confirmação de pedido
  - Histórico de pedidos

- [ ] **Critérios de Aceitação**:
  - Usuário consegue adicionar produtos ao carrinho
  - Checkout completo funcionando
  - Confirmação enviada por email
  - Histórico disponível

#### 📍 **Localização do Vendedor**
- [ ] **Funcionalidades**:
  - Integração com mapas
  - Exibição da localização
  - Cálculo de distância
  - Rota para o vendedor

- [ ] **Critérios de Aceitação**:
  - Localização exibida no mapa
  - Distância calculada corretamente
  - Rota disponível
  - Funciona em dispositivos móveis

## 🎯 Sprint 4: Diferenciais e Deploy

### 🎯 **Objetivo**
Entregar funcionalidades diferenciais e colocar o sistema no ar

### 📋 **Metas de Entrega**

#### 🌐 **Ambiente de Demonstração**
- [ ] **Funcionalidades**:
  - Deploy em produção
  - Configuração de domínio
  - SSL/HTTPS configurado
  - Monitoramento básico

- [ ] **Critérios de Aceitação**:
  - Sistema acessível publicamente
  - Performance adequada
  - Segurança implementada
  - Logs funcionando

#### 💬 **Chat entre Vendedor/Comprador**
- [ ] **Funcionalidades**:
  - Sistema de mensagens em tempo real
  - Notificações push
  - Histórico de conversas
  - Status online/offline

- [ ] **Critérios de Aceitação**:
  - Mensagens são enviadas/recebidas
  - Notificações funcionam
  - Histórico preservado
  - Interface intuitiva

#### ⭐ **Sistema de Avaliações**
- [ ] **Funcionalidades**:
  - Avaliação de produtos
  - Avaliação de vendedores
  - Comentários e reviews
  - Sistema de reputação

- [ ] **Critérios de Aceitação**:
  - Usuários podem avaliar
  - Média de avaliações calculada
  - Comentários moderados
  - Reputação visível

## 📈 Métricas de Acompanhamento

### 🎯 **Métricas por Sprint**

| Sprint | Story Points | Entregues | Velocidade | Bugs | Status |
|--------|-------------|-----------|------------|------|--------|
| Sprint 1 | 13 | 13 | 100% | 0 | ✅ Concluída |
| Sprint 2 | 21 | 0 | 0% | 0 | 🔄 Em Andamento |
| Sprint 3 | 34 | 0 | 0% | 0 | ⏳ Planejada |
| Sprint 4 | 29 | 0 | 0% | 0 | ⏳ Planejada |


## 📅 Próximas Reuniões

### 🗓️ **Agenda de Cerimônias**

| Cerimônia | Data | Horário | Objetivo |
|-----------|------|---------|----------|
| Sprint Review 1 | 10/12/2024 | 35N34 | Apresentar resultados da Sprint 1 |
| Sprint Planning 2 | 17/12/2024 | 35N34 | Planejar Sprint 2 |
| Daily Standup | Diário | 35N34 | Sincronização da equipe |
| Retrospectiva 1 | 10/12/2024 | 35N34 | Melhorias do processo |

---

> **Última atualização**: Dezembro 2024  
> **Próxima revisão**: Ao final de cada sprint
