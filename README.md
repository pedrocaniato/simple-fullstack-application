# 🧩 Simple Fullstack Application

Este é um projeto **Fullstack** simples desenvolvido com **Next.js (frontend)**, **NestJS (backend)** e **PostgreSQL (banco de dados)**.  
O objetivo é demonstrar uma arquitetura completa e organizada para o **cadastro e listagem de produtos**.

---

## 🚀 Tecnologias Utilizadas

### Frontend
- [Next.js](https://nextjs.org/) — Framework React para renderização SSR e SSG  
- [TypeScript](https://www.typescriptlang.org/) — Tipagem estática para maior segurança no código  
- [CSS Modules / Tailwind] — Estilização da interface  

### Backend
- [NestJS](https://nestjs.com/) — Framework Node.js modular e escalável  
- [TypeORM](https://typeorm.io/) — ORM para integração com banco de dados  
- [PostgreSQL](https://www.postgresql.org/) — Banco de dados relacional  

---

## ⚙️ Funcionalidades

- ✅ Cadastrar novos produtos  
- ✅ Listar produtos cadastrados  
- ✅ Integração completa entre frontend e backend  
- ✅ Conexão com banco de dados PostgreSQL  
- ✅ Estrutura pronta para expansão (atualizar e deletar produtos)

---

## 🗂️ Estrutura do Projeto

simple-fullstack-application/
│
├── backend/ # API construída com NestJS
│ ├── src/
│ │ ├── main.ts # Ponto de entrada da aplicação
│ │ ├── app.module.ts # Módulo raiz
│ │ ├── product/ # Módulo responsável pelos produtos
│ │ └── ...
│ ├── ormconfig.json # Configuração de conexão com o banco
│ └── package.json
│
├── frontend/ # Aplicação Next.js (interface)
│ ├── pages/
│ │ ├── index.tsx # Página inicial (listagem)
│ │ ├── create.tsx # Página de cadastro de produto
│ │ └── ...
│ ├── components/ # Componentes reutilizáveis
│ └── package.json
│
└── README.md


---

## 🧠 Conceito do Projeto

A ideia é fornecer uma **base sólida** para desenvolvimento **fullstack**, conectando as principais partes de um sistema web moderno:

1. **Frontend (Next.js)** envia requisições HTTP ao backend.  
2. **Backend (NestJS)** recebe e processa os dados, aplicando regras de negócio.  
3. **Banco de dados (PostgreSQL)** armazena as informações de forma persistente.  

---

## 🔧 Como Rodar o Projeto Localmente

### Pré-requisitos
- Node.js 18+  
- PostgreSQL instalado e rodando  
- npm ou yarn  

### Passo a passo

#### 1️⃣ Clonar o repositório

git clone https://github.com/pedrocaniato/simple-fullstack-application.git
cd simple-fullstack-application


#### 2️⃣ Configurar o Banco de Dados

Crie um banco no PostgreSQL (exemplo):

```bash
CREATE DATABASE products_db;
```

Atualize as credenciais no arquivo:

backend/ormconfig.json

#### 3️⃣ Rodar o Backend
```bash
cd backend
npm install
npm run start:dev
```

Servidor rodando em:

```bash
http://localhost:3334
```
#### 4️⃣ Rodar o Frontend
```bash
cd ../frontend
npm install
npm run dev
```

Aplicação acessível em:
```bash
http://localhost:3000
```


🧪 Teste Rápido

Acesse o frontend e:

Adicione um novo produto pelo formulário.

Verifique se ele aparece na listagem.

Você também pode testar a API diretamente com ferramentas como Postman ou Insomnia.

🧭 Próximos Passos (Sugestões)

🔐 Adicionar autenticação (JWT ou OAuth)

🛠️ Implementar atualização e exclusão de produtos

📊 Adicionar paginação e busca

🧰 Criar testes unitários e de integração

🚀 Dockerizar os serviços para execução simplificada

👨‍💻 Autor

Pedro Caniato
📧 pedrolucascaniato@gmail.com

🔗 github.com/pedrocaniato


