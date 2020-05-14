# How to use

## Starting apache for postgres

```bash
docker-compose up apache-postgres
```

## Util CLIs

### Composer

```bash
docker run --rm -it -v ${PWD}:/app composer --version
```

### Laravel

```bash
# Building Docker image with Laravel
docker build -t laravel ./docker/laravel
# Executing Laravel CLI (checking version)
docker run --rm -it -v ${PWD}:/app laravel --version
```
