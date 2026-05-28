<div align="center">

# Felipe Shimizu

**Desenvolvedor Backend Java · Spring Boot · Kafka · Microsserviços · REST APIs**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/felipesshimizu)
[![Portfólio](https://img.shields.io/badge/Portfólio-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://www.devfelipeshimizu.me)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Felipe-SMZ)

</div>

---

## Sobre mim

Desenvolvedor backend com foco em **Java e Spring Boot**, estudante de Desenvolvimento de Software Multiplataforma na **FATEC Cotia** (4º semestre).

Antes da programação, acumulei 15+ anos de experiência profissional — gestão operacional em empresa familiar, departamento de licitações em gestão hospitalar e **4 anos na indústria automotiva japonesa**. Essa bagagem me trouxe precisão, disciplina e orientação a qualidade que aplico diretamente no código que escrevo.

- 📍 São Paulo — SP, Brasil
- 🎯 Foco: Backend Java · Spring Boot · Kafka · Microsserviços · REST APIs
- 🚀 Buscando oportunidade de estágio ou Jr em desenvolvimento backend
- 🌱 Estudando: AWS · Testes integrados · Boas práticas de arquitetura

---

## Stack

<div align="center">

**Backend**

![Java](https://img.shields.io/badge/Java-007396?style=for-the-badge&logo=java&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=for-the-badge&logo=springsecurity&logoColor=white)
![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=for-the-badge&logo=apachekafka&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)

**Banco de dados**

![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)

**Infraestrutura & Ferramentas**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apache-maven&logoColor=white)

</div>

---

## Projetos em destaque

### 🛵 Sistema de Delivery — Microsserviços com Kafka
> Arquitetura orientada a eventos com 4 microsserviços independentes

Sistema de delivery onde a criação de um pedido dispara um fluxo assíncrono entre serviços via Apache Kafka. Cada serviço tem seu próprio banco de dados — sem compartilhamento de tabelas, sem acoplamento.

**Destaques técnicos:**
- 4 microsserviços independentes: order, restaurant, delivery e notification
- Comunicação assíncrona via Apache Kafka com consumer groups
- Idempotência implementada na API REST e nos consumers Kafka
- Database per service — isolamento total entre os bancos
- Docker Compose com Kafka, Zookeeper e MySQL
- Fluxo completo: pedido → restaurante → entregador → notificação

`Java` `Spring Boot 4` `Apache Kafka` `MySQL` `Docker` `Spring Data JPA`

| Repositório | Descrição |
|-------------|-----------|
| [order-service](https://github.com/Felipe-SMZ/delivery-order-service) | Producer Kafka — recebe e persiste pedidos |
| [restaurant-service](https://github.com/Felipe-SMZ/delivery-restaurant-service) | Consumer/Producer — processa e aceita pedidos |
| [delivery-service](https://github.com/Felipe-SMZ/delivery-delivery-service) | Consumer/Producer — gerencia entregadores |
| [notification-service](https://github.com/Felipe-SMZ/delivery-notification-service) | Consumer — notifica clientes em cada etapa |
| [delivery-infra](https://github.com/Felipe-SMZ/delivery-infra) | Docker Compose com toda a infraestrutura |

---

### 🎮 Game Critic — Plataforma de Reviews de Jogos
> Fullstack em produção — backend Railway · frontend Vercel

Plataforma completa onde usuários podem se cadastrar, buscar jogos por filtros dinâmicos e publicar reviews. Deploy real com CI/CD automatizado.

**Destaques técnicos:**
- Autenticação JWT com Spring Security e sistema de roles (ADMIN/USER)
- Filtros dinâmicos com Specification do Spring Data JPA
- Documentação interativa com Swagger/OpenAPI
- Headers de segurança: CSP, HSTS e X-Frame-Options
- CI/CD com GitHub Actions — deploy automático no Railway e Vercel
- Testes unitários e de integração com MockMvc e H2

`Java` `Spring Boot` `Spring Security` `JWT` `MySQL` `React` `TailwindCSS` `Docker` `GitHub Actions`

[![Backend](https://img.shields.io/badge/Backend-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Felipe-SMZ/jogos-review-api)
[![Frontend](https://img.shields.io/badge/Frontend-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Felipe-SMZ/jogos-review-frontend)
[![Demo](https://img.shields.io/badge/Demo_ao_vivo-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://jogos-review-frontend.vercel.app)

---

### 🚗 FatecRide — Plataforma de Caronas Universitárias
> Projeto Integrador FATEC — arquitetura com múltiplos backends

Sistema de caronas colaborativas para a comunidade acadêmica. Arquitetura com 3 backends independentes (Spring Boot + 2x Node.js), chat em tempo real via WebSocket e visualização de rotas com Leaflet Maps.

**Destaques técnicos:**
- Arquitetura de microsserviços com Spring Boot e Node.js
- Autenticação JWT com Spring Security
- Chat em tempo real via WebSocket
- Agendamento recorrente de caronas
- Visualização de rotas com Leaflet Maps

`Java` `Spring Boot` `Node.js` `React` `MySQL` `MongoDB` `WebSocket` `JWT`

[![Backend](https://img.shields.io/badge/Backend-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Felipe-SMZ/FatecRideBackend2.0)
[![Frontend](https://img.shields.io/badge/Frontend-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Felipe-SMZ/FatecRideFrontend2.0)

---

### 📝 ThreadFlow — API REST de Blog
> Backend com foco em segurança e testes

API REST robusta para gerenciamento de blog com autenticação JWT, controle de permissões por roles e documentação interativa.

**Destaques técnicos:**
- Autenticação JWT com sistema de roles (USER, ADMIN, MODERATOR)
- Testes com JUnit 5 e Mockito
- Documentação com Swagger UI
- Busca e paginação avançadas
- Containerização com Docker

`Java` `Spring Boot` `JWT` `PostgreSQL` `JUnit 5` `Mockito` `Docker` `Swagger`

[![Repositório](https://img.shields.io/badge/Repositório-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Felipe-SMZ/Blog)


---

<div align="center">

**Disponível para estágio e oportunidades Jr em backend**

[![LinkedIn](https://img.shields.io/badge/Vamos_conversar-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/felipesshimizu)

</div>
