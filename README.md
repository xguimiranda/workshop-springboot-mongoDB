# API SocialApp – Spring Boot + MongoDB

Projeto desenvolvido como parte do **curso de Java do Prof. Nélio Alves (Udemy)** para praticar conceitos de desenvolvimento backend com Spring Boot, arquitetura em camadas e persistência em banco NoSQL (MongoDB).

---

## 🎯 Objetivo

Fornecer uma API REST simples para uma rede social minimalista, contemplando:
- Cadastro e gestão de usuários
- Publicação e consulta de posts
- Curtidas e comentários

---

## 🧱 Principais Conceitos Praticados

- Spring Boot (auto configuração, starters)
- Injeção de dependência e organização em camadas (Controller / Service / Repository / DTO / Model)
- Persistência com **Spring Data MongoDB**
- Modelagem de documentos e referências/embutidos
- Boas práticas de design de API REST
- Tratamento básico de exceções (ExceptionHandler)
- Padronização de responses com DTOs

---

## 🚀 Funcionalidades (Resumo)

| Recurso | Descrição |
|---------|-----------|
| Usuários | Criar, listar, buscar por id |
| Posts | Criar, listar, buscar por id, (editar/excluir se implementado) |
| Comentarios | Comentarios em publicações aparecem ao chamar o usuario |

---

## 🛠 Tecnologias e Dependências

- Java 17+ (ou versão utilizada no curso)
- Spring Boot
- Spring Data MongoDB
- MongoDB Community / Atlas
- Maven (ou Gradle)
- (Opcional) Spring Web, Validation, Spring Security, Lombok

---


## 📖 Exemplos de Endpoints (ilustrativos)

| Método | Endpoint | Descrição |
|--------|----------|-----------|
| GET | /users | Lista usuários |
| GET | /users/{id} | Busca usuário por id |
| POST | /users | Cria novo usuário |
| PUT | /users/{id} | Atualiza usuário (se implementado) |
| DELETE | /users/{id} | Remove usuário (se implementado) |
| GET | /posts | Lista posts |
| POST | /posts | Cria post |
| GET | /posts/{id} | Detalha post |
| DELETE | /posts/{id} | Remove post (se implementado) |
| POST | /users/{id}/follow | Seguir usuário (se implementado) |
| POST | /users/{id}/unfollow | Deixar de seguir (se implementado) |
| GET | /feed | Feed de posts (se implementado) |

---

## ❗ Tratamento de Erros (Sugestão)

Retornar JSON padronizado, exemplo:
```json
{
  "timestamp": "2025-01-01T12:00:00Z",
  "status": 404,
  "error": "Not Found",
  "message": "Usuário não encontrado",
  "path": "/users/123"
}
```

---

## 👤 Autor

**Guilherme Miranda**  
- GitHub: [@xguimiranda](https://github.com/xguimiranda)  
- LinkedIn: https://www.linkedin.com/in/SEU-PERFIL-AQUI  

---

## 🙏 Créditos

- Curso Java Completo (Prof. Nélio Alves – Udemy)
- Comunidade Spring
- Documentação oficial do MongoDB

---
