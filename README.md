# 🛒 API de Gerenciamento de Produtos

API REST desenvolvida com **ASP.NET Core (.NET 9)** para gerenciamento de produtos, aplicando boas práticas de desenvolvimento backend, arquitetura em camadas e autenticação com **JWT**.

---

## 🚀 Sobre o projeto

Esta API permite o gerenciamento completo de produtos por meio de operações CRUD, com persistência em banco de dados e controle de acesso baseado em autenticação.

O projeto foi desenvolvido com foco em simular um ambiente real de backend, aplicando conceitos amplamente utilizados no mercado como:

- Arquitetura em camadas  
- Injeção de dependência  
- Entity Framework Core  
- Autenticação e autorização com JWT  

---

## ⚙️ Funcionalidades

- 📌 Listar todos os produtos  
- 🔍 Buscar produto por ID  
- ➕ Cadastrar novo produto  
- ✏️ Atualizar produto existente  
- ❌ Remover produto  
- 🔐 Autenticação de usuários (login)  
- 🛡️ Autorização baseada em perfil  
- 📄 Documentação interativa com Swagger  

---

## 🔐 Segurança (JWT)

A API utiliza autenticação baseada em **JWT (JSON Web Token)**.

- O usuário realiza login e recebe um token  
- Esse token é enviado nas requisições protegidas  
- A API valida o token antes de permitir o acesso  

💡 Isso garante que apenas usuários autenticados possam acessar determinados recursos.

---

## 🛠️ Tecnologias utilizadas

- **.NET 9.0.312**
- **ASP.NET Core (Web API)**
- **Entity Framework Core**
- **PostgreSQL**
- **JWT (Autenticação e Autorização)**
- **Swagger (Swashbuckle)**

---

## 🧱 Arquitetura do projeto

O projeto segue o padrão de separação em camadas:

- **Controllers** → Recebem as requisições HTTP  
- **Services** → Contêm as regras de negócio  
- **Models** → Representam as entidades  
- **Data (DbContext)** → Acesso ao banco de dados  

💡 Essa abordagem facilita manutenção, testes e escalabilidade.

---

## 📡 Endpoints principais

### 🔓 Públicos
| Método | Endpoint | Descrição |
|--------|----------|----------|
| POST   | /login   | Autenticação do usuário |

### 🔒 Protegidos (requer JWT)
| Método | Endpoint         | Descrição                     |
|--------|-----------------|-------------------------------|
| GET    | /produtos       | Lista todos os produtos       |
| GET    | /produtos/{id}  | Busca produto por ID          |
| POST   | /produtos       | Cadastra um novo produto      |
| PUT    | /produtos/{id}  | Atualiza um produto existente |
| DELETE | /produtos/{id}  | Remove um produto             |

---

## 👤 Autor

**Rafael Artur F. Quaresma**

📌 Projeto com fins de aprendizagem e educacionais.
