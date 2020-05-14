# How to use

## Starting apache for postgres

```bash
docker-compose up apache-postgres
```

## Using Composer CLI

```bash
docker run --rm -it -v ${PWD}:/app composer --version
```

## Using Laravel CLI

```bash
# Building Docker image with Laravel
docker build -t laravel ./docker/laravel
# Executing Laravel CLI (checking version)
docker run --rm -it -v ${PWD}:/app laravel --version
```
