# porchegg-api
[![Build Status](https://travis-ci.com/nppi3enz/porchegg-api.svg?token=x1gvofY5ULJm5fexMUJE&branch=master)](https://travis-ci.com/nppi3enz/porchegg-api)
[![codecov](https://codecov.io/gh/nppi3enz/porchegg-api/branch/master/graph/badge.svg?token=9R8TzUdJgk)](https://codecov.io/gh/nppi3enz/porchegg-api)

> Porchegg-api

Base on Laravel Lumen is a stunningly fast PHP micro-framework for building web applications with expressive, elegant syntax. We believe development must be an enjoyable, creative experience to be truly fulfilling. Lumen attempts to take the pain out of development by easing common tasks used in the majority of web projects, such as routing, database abstraction, queueing, and caching.

#### Build Setup


Run the docker for development:
---------------------
First you need to copy `.env.local` to `.env` for setup environment of appplication

``` bash
cp .env.example .env
```

You can now build, create, start, and attach to containers to the environment for your application. To build the containers use following command inside the project root:

```bash
docker-compose build
```

To start the application and run the containers in the background, use following command inside project root:

```bash
docker-compose up -d
```
```bash
docker-compose down
```

Installing Dependencies via Composer
------------------------------------
Run the composer installer:

```bash
docker exec -it porchegg-api composer install
```
or
```bash
docker exec -it porchegg-api composer update
```

Database Setup
------------------------------------
Run the migration artisan command:
```bash
docker exec -it porchegg-api php artisan migrate
docker exec -it porchegg-api php artisan db:seed
```
