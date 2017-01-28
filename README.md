# Double-Docker

## Services
- Mysql
- Php
- Maildev
- Nginx



## Procedure
- docker-compose build
- docker-compose up -d
- Add double-gestion.project in hosts


## Aliases

### Composer
- alias composer='sudo docker run -ti --rm -v $(pwd):/app composer/composer:alpine'

### Php
- alias php='sudo docker exec -ti php php'