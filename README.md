<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo_text.svg" width="320" alt="Nest Logo" /></a>
</p>

<p align="center">Probando NestJS.</p>

## Descripción

Tienda de libros

## Instalación

```bash
$ npm install
```

## Ejecutar

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

## Notas

> Este proyecto es construido con fines didacticos, por lo que los archivos
> .env y orm.config.json no deben ser subidos a los repositorios

## Instalar dependencias de configuaración

```shell script
npm i -D dotenv @types/dotenv
```

## Crear un modulo
```shell script
nest g module config
```

## Contenedor postgres

https://hub.docker.com/_/postgres

```shell script
docker run -d -p 5444:5432 --name postgres -e POSTGRES_PASSWORD=secret postgres
```

## Instalar el ORM para postgress
```shell script
npm i @nestjs/typeorm typeorm pg
```

## Crear modulo de base de datos
```shell script
nest g module database
```

## Crear modulo de usuarios
```shell script
nest g module modules/user
```

## Instalar ts-node para migraciones
```shell script
npm i -g ts-node
```

## Generar migraciones
```shell script
npm run migration:generate first_migration
npm run migration:run
npm run migration:revert
```