
---

# CodeFlix 🎬

CodeFlix é uma plataforma de streaming de vídeos inspirada na Netflix, desenvolvida com foco em arquitetura moderna, escalabilidade e boas práticas de engenharia de software.

## 🔧 Tecnologias Utilizadas

* **Backend:**

  * Java 17 + Spring Boot
  * Golang
  * GraphQL
  * DDD (Domain-Driven Design)
  * TDD (Test-Driven Development)
  * Clean Architecture
  * Kafka
  * ElasticSearch
  * Keycloak (OAuth 2.0)
  * Docker([GitHub][1], [GitHub][2])

* **Frontend:**

  * React + Redux (Admin)
  * Next.js + TailwindCSS (Usuário)([GitHub][1])

* **Encoding de Vídeos:**

  * Golang
  * Bento4 (MP4 para MPEG-DASH)([GitHub][2])

## 🧩 Arquitetura de Microsserviços

O projeto é composto por diversos microsserviços, cada um com responsabilidades bem definidas:

* **Admin do Catálogo:**

  * Backend em Java 17 com Spring Boot
  * Frontend em React + Redux + Material UI
  * Implementa DDD, TDD e Clean Architecture([GitHub][1])

* **Catálogo de Vídeos:**

  * API em Java 17 com Spring Boot e GraphQL
  * Responsável por fornecer dados para o frontend do usuário([Gist][3], [GitHub][4])

* **Encoder de Vídeos:**

  * Desenvolvido em Golang
  * Realiza a conversão de vídeos de MP4 para MPEG-DASH utilizando Bento4

* **Frontend do Usuário:**

  * Desenvolvido com Next.js e TailwindCSS
  * Interface amigável para os usuários consumirem o conteúdo

## 🔐 Autenticação e Segurança

* Implementação de autenticação e autorização utilizando Keycloak com suporte a OAuth 2.0.
* Gerenciamento de usuários, permissões e tokens de acesso.

## 📦 Deploy e DevOps

* Containerização de todos os serviços utilizando Docker.
* Orquestração com Kubernetes (em planejamento).
* Pipelines de CI/CD configuradas com GitHub Actions.
* Monitoramento e logging com ElasticSearch.([GitHub][5], [GitHub][1])

## 🚀 Como Executar o Projeto

### Pré-requisitos

* Docker e Docker Compose instalados
* JDK 17
* Node.js e Yarn
* Go instalado([GitHub][2])

### Passos

1. Clone o repositório:([GitHub][4])

   ```bash
   git clone https://github.com/Nesrux/CodeFlix.git

   ```
2. Navegue até o diretório do projeto:

   ```bash
   cd CodeFlix

   ```
3. Inicie os containers com Docker Compose:

   ```bash
   docker-compose up --build

   ```
4. Acesse o frontend do usuário em:

   ```
   http://localhost:3000

   ```
5. Acesse o painel de administração em:

   ```
   http://localhost:3001

   ```

## 📁 Estrutura do Repositório

```
CodeFlix/
├── admin-do-catalogo/         # Backend do administrador
├── api-catalogo-de-videos/    # API do catálogo de vídeos
├── api-enconder/              # Serviço de encoding de vídeos
├── Front-Codeflix/            # Frontend do usuário
├── docker-compose.yml         # Orquestração dos serviços
└── README.md                  # Documentação do projeto
```



## 🛠️ Funcionalidades em Desenvolvimento

* Implementação do microsserviço de assinatura do serviço.
* Integração completa com Kubernetes para deploy em produção.
* Melhorias na interface do usuário e experiência geral.([GitHub][6])

## 🤝 Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e pull requests.

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---
