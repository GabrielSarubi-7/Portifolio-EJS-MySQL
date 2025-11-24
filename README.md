# Portfólio Acadêmico — Gabriel Sarubi Motta Ferreira

Projeto em **Node.js + Express + EJS** com **CRUD** (GET/POST/PUT/DELETE) e integração com **MySQL**

## Como rodar

```bash
npm install
npm install mysql2 dotenv
npm start
# abra http://localhost:3000
````

> Lembre-se de configurar o arquivo `.env` com as credenciais do banco de dados MySQL antes de iniciar o servidor.

## Rotas principais

* `/` — Apresentação
* `/formacao` — Formação e cursos
* `/projetos` — Lista + CRUD de projetos (com endpoints REST persistidos no MySQL)
* `/competencias` — Competências técnicas e interpessoais
* `/contato` — Links

### CRUD de Projetos (também via API)
* `GET /api/projetos` — lista JSON de projetos cadastrados no banco
* `POST /projetos` — cria projeto (formulário na página)
* `PUT /projetos/:id` — edita projeto (usa `?_method=PUT`)
* `DELETE /projetos/:id` — exclui projeto (usa `?_method=DELETE`)

> Os dados dos projetos agora são salvos em um **banco MySQL**, conforme script em `banco.sql`.
