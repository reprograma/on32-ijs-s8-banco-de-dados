# Links Úteis

- [PostGreSQL Editor](https://onecompiler.com/postgresql)
- [DBeaver](https://dbeaver.io/download/)

## Tutoriais

- [Instalação PostGreSQL MacOS](https://www.postgresqltutorial.com/postgresql-getting-started/install-postgresql-macos/)
- [Instalação PostGreSQL Linux](https://www.postgresqltutorial.com/postgresql-getting-started/install-postgresql-linux/)
- [Instalação PostGreSQL Windows](https://www.postgresqltutorial.com/postgresql-getting-started/install-postgresql/)

## TypeORM

- [Getting Started](https://typeorm.io/)

## Docker

### Instalação da imagem do postgres

```sh
docker pull postgres:latest
```

### Cria um banco de dados usando docker

```sh
docker run --name postgres-db-hands -e POSTGRES_PASSWORD=Users123 -e POSTGRES_USER=lais -e POSTGRES_DB=users -p 5432:5432 -d postgres
```

### Encerra um container docker

```sh
docker container stop postgres-db-hands
```

### Excluir um container docker

```sh
docker rm postgres-db-hands
```

## Instalação do TypeORM em projeto Nestjs

```sh
npm install @nestjs/typeorm typeorm pg
```
