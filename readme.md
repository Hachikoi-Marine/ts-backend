## Contributions

- `$ git clone https://github.com/Hachikoi-Marine/ts-backend.git`
- Add your local Postgres connectio string `postgresql://<username>:<password>@localhost:5432/csv?schema=public` in a new .env file
- `$ yarn prisma generate`
- sync prisma with DB `yarn prisma migrate dev --name init`

## Prisma instructions

**Install stuff**

- cli:

  - bun a -d prisma
  - yarn add -D prisma

- client
  - bun a @prisma/client
  - yarn add @prisma/client

## Init prisma project

`$ yarn prisma init`
then follow instructions given after the command finishes

## Create DB & add models

`$ yarn prisma migrate dev --name init`
every migration needs a name, so that flag is abligatory

## Built-in GUI

`yarn prisma studio`

## further study

[docs](https://www.prisma.io/docs/getting-started/quickstart)

## Postgres CLI

- List tables: \dt
- List items in table: `select * from "User";` or if it's lowercase `select * from user;` is enough
- `create database my_database` - self explanatory

# Fastify

## Routing

- [separate files](https://www.fastify.io/docs/latest/Guides/Getting-Started/#your-first-plugin)
