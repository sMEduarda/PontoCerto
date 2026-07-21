# 📍 PontoCerto

Sistema de Registro de Ponto com Geolocalização desenvolvido como projeto acadêmico.

O projeto é composto por uma API REST em C# (.NET) responsável pelas regras de negócio e persistência dos dados, além de uma aplicação Web em React para interação com os usuários.

# 🚀 Tecnologias Utilizadas

### Back-end

* C#
* ASP.NET Core Web API
* Entity Framework Core
* SQL Server
* JWT Authentication
* Swagger

### Front-end

* React
* React Router DOM
* Axios
* HTML5
* CSS3
* JavaScript
  
# 📌 Funcionalidades

* Login de usuários
* Autenticação utilizando JWT
* Registro de ponto
* Registro de geolocalização
* Histórico de registros
* Integração entre Front-end e API
* Banco de dados SQL Server
* Documentação da API com Swagger

# 🏗️ Arquitetura

React
   │
   ▼
ASP.NET Core Web API
   │
   ▼
Entity Framework Core
   │
   ▼
SQL Server

# 📂 Estrutura do Projeto

PontoCerto/

├── API_PontoCerto/
│   ├── Controllers/
│   ├── Models/
│   ├── DTOs/
│   ├── Services/
│   ├── Repositories/
│   ├── Data/
│   └── Program.cs
│
├── pontocerto-front/
│   ├── src/
│   ├── components/
│   ├── pages/
│   ├── services/
│   └── App.jsx
│
└── README.md

# ⚙️ Como Executar o Projeto

## 1. Clone o repositório

bash
git clone https://github.com/sMEduarda/PontoCerto.git

Entre na pasta do projeto.

## 2. Configure o Banco de Dados

* Instale o SQL Server.
* Abra o SQL Server Management Studio (SSMS).
* Crie o banco de dados.
* Atualize a Connection String no arquivo: appsettings.json

## 3. Execute a API

Entre na pasta da API:

bash
cd API_PontoCerto

Restaure os pacotes:

bash
dotnet restore

Execute as migrations:

bash
dotnet ef database update

Inicie a API:

bash
dotnet run

A documentação ficará disponível em:

text
https://localhost:xxxx/swagger

## 4. Execute o Front-end

Abra outro terminal.

Entre na pasta:

bash
cd pontocerto-front


Instale as dependências:

bash
npm install


Inicie o projeto:

bash
npm run dev


# Fluxo da Aplicação

1. O usuário realiza o login.
2. A API valida as credenciais.
3. Um token JWT é gerado.
4. O React armazena o token.
5. O usuário registra o ponto.
6. A localização é enviada para a API.
7. A API salva os dados no SQL Server.
8. O histórico de registros pode ser consultado pelo usuário.

# Conceitos Aplicados

* API REST
* Arquitetura Cliente-Servidor
* Autenticação JWT
* Entity Framework Core
* SQL Server
* React
* Consumo de API com Axios
* Geolocalização
* CRUD
* Arquitetura em Camadas

Projeto desenvolvido para a disciplina de Desenvolvimento de Sistemas.
