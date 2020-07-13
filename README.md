# Money Jar Docker Setting

## Prequisites

- Docker. Visit [installation guide](https://www.docker.com/community-edition)
- Docker Compose. Visit [installation guide](https://docs.docker.com/compose/install/)


## Preparation

- Make sure cloning 2 repositories into the same directory

```
... trachanhgao/
... trachanhgao-dev/
```


## Builder Docker Images Steps:

### 1. Create .env file by copying .env.example

```
$ cp .env.example .env
```

### 2.  Build docker containers

```
$ docker-compose build
```

### 3. Run docker containers

```
$ docker-compose up -d
```

> -d: detach mode

### 4. Access to web container as "gao" user

```
$ docker-compose exec --user=gao web bash
```

### 5. Access to browser "http://trachanhgao.local"
