# 🐾 Plataforma MeuPet

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Quarkus](https://img.shields.io/badge/Quarkus-3.14-blueviolet?style=for-the-badge)
![Java](https://img.shields.io/badge/Java-21-blue?style=for-the-badge)
![JWT](https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=json-web-tokens)
![NGINX](https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=nginx&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Heroku](https://img.shields.io/badge/Heroku-430098?style=for-the-badge&logo=heroku&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

## Olá, seja bem-vindo(a) à organização da **Plataforma MeuPet**! 👋

Somos um projeto focado em facilitar o gerenciamento de pets e seu histórico de saúde, oferecendo uma solução moderna e distribuída construída com base em microsserviços. Nossa plataforma visa proporcionar uma experiência fluida para tutores de animais, desde o cadastro de informações básicas até o acompanhamento de vacinas e dados de saúde.

---

## 🎥 Demonstração da Plataforma

Para demonstrar o funcionamento e a estabilidade da nossa plataforma, preparamos um vídeo que exibe um **teste de ponta a ponta (end-to-end)** rodando com **Selenium**. A automação simula o fluxo de um usuário real, desde o cadastro até o gerenciamento de pets, validando a integração entre o frontend e todos os microsserviços do backend. Assista para ver a plataforma em ação!



https://github.com/user-attachments/assets/80b3bbe3-5aa3-426f-92e1-ddae4cac2f1d


---

## 🚀 Sobre a Plataforma MeuPet

A Plataforma MeuPet é construída com uma arquitetura de microsserviços, garantindo escalabilidade, resiliência e manutenibilidade. Cada parte da aplicação tem uma responsabilidade bem definida e se comunica de forma eficiente.

### **Componentes e Arquitetura:**

Nossa plataforma é composta pelos seguintes microsserviços e componentes de infraestrutura:

* **Frontend (`meupet-frontend`):**
    * Desenvolvido com **Next.js**, **React**, **TypeScript** e **Tailwind CSS**.
    * É a interface de usuário principal, onde tutores podem cadastrar, visualizar e gerenciar seus pets e dados.
    * Hospedado na **Vercel**.
    * Comunica-se com o backend através do **API Gateway (NGINX)**.

* **API Gateway (`meupet-api-gateway-prod`):**
    * Implementado com **NGINX**.
    * Atua como o **ponto de entrada único** para todas as requisições do frontend, gerenciando roteamento (ex: `/usuarios` para o serviço de usuários, `/animais` para o serviço de animais) e aplicando políticas de **CORS**.
    * Hospedado no **Heroku**.

* **Microsserviço de Usuários (`meupet-users-api`):**
    * Backend em **Java (Quarkus)**.
    * Responsável pelo gerenciamento de usuários, incluindo **cadastro**, **login** e **autenticação** via **JWT**.
    * Hospedado no **Heroku**.

* **Microsserviço de Animais (`meupet-animals-api`):**
    * Backend em **Java (Quarkus)**.
    * Responsável pelo gerenciamento de **animais** (cachorros, gatos, aves) e seus **históricos de vacinação**.
    * Comunica-se com o microsserviço de usuários para validações e operações em cascata (ex: exclusão de animais ao deletar um tutor).
    * Hospedado no **Heroku**.

* **Banco de Dados:**
    * Utilizamos **PostgreSQL** como nosso banco de dados principal.
    * É um serviço de banco de dados gerenciado, garantindo persistência e alta disponibilidade.

### **Tecnologias Principais Utilizadas:**

* **Frontend:** Next.js, React, TypeScript, Tailwind CSS, Shadcn UI
* **Backend:** Java 21, Quarkus, Hibernate ORM com Panache, Maven, SmallRye JWT
* **Infraestrutura:** Docker, NGINX, PostgreSQL
* **Cloud Hosting:** Heroku (para backends e gateway), Vercel (para frontend)

---

## 🌐 Aplicação Publicada

A Plataforma MeuPet está implantada e acessível online.

* **Frontend (Aplicação Principal):**[ https://community.render.com/t/connecting-frontend-from-vercel/2078](https://meupet-frontend-web.vercel.app/)
* **API Gateway (Ponto de Entrada das APIs):** 
* **Microsserviço de Usuários (Swagger UI):** 
* **Microsserviço de Animais (Swagger UI):** 

---

## 📖 Recursos Úteis

Explore nossos repositórios individuais para mais detalhes sobre cada componente:

* **Repositório do Frontend:** [[Link para o repositório do frontend]](https://github.com/MeuPet-Platform/meupet-webapp)
* **Repositório da Infraestrutura:** [[Link para o repositório da infraestrutura]](https://github.com/MeuPet-Platform/meupet-infra)
* **Repositório da API de Usuários:** [[Link para o repositório da API de usuários]](https://github.com/MeuPet-Platform/meupet-users-api)
* **Repositório da API de Animais:** [[Link para o repositório da API de animais]](https://github.com/MeuPet-Platform/meupet-animals-api)
