# Desafio 2

### Desafio Nest.js

Neste desafio, você deve criar uma aplicação Nest.js com Docker que rode na porta 3000. Esta aplicação precisa expor 2 rotas de API Rest:

- Listar assets - POST /api/assets
- Criar assets - GET /api/assets
- Criar orders - POST /api/orders
- Listar orders - GET /api/orders

Um asset tem os seguintes dados:

- id (é informado pelo usuário
- symbol (símbolo do ativo

Uma order tem os seguintes dados:

- id automático do banco
- asset_id (relacionado com Asset)
- price
- status (open, pending, closed) (não pode deixar mandar o status no POST)

O ORM a ser usado é o Prisma ORM e o banco de dados precisa ser o Mongo, image: bitnami/mongodb:5.0.17

**Obs:** Neste caso, em vez de usar a imagem solicitada, por problemas de compatibilidade com o SO, foi usada outra solução compatível.

### Executando o projeto

Para executar o projeto, execute:

- `docker compose up`

Em outro terminal

- `nvm use`
- `npm install`
- `npm run start:dev`

# General Guidelines

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://kamilmysliwiec.com)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](LICENSE).
