## Primeiro Projeto - Publicando imagem Laravel

Para rodar essa aplicação siga os passos abaixo:

Clone o aplicativo
```
git clone https://github.com/milsonei/code-education-projeto-01.git milsonei-laravel
```
Mude para o diretório milsonei-laravel
```
cd milsonei-laravel
```

Execute o comando docker-compose
```
docker-compose up -d
```

Acesse o contêiner da aplicação app
```
docker exec -it app bash 
```

Instale o composer
```
bash-5.0# composer install 
```

Gere a chave da aplicação
```
bash-5.0# php artisan key:generate
```

Execute o comando migrate
```
bash-5.0# php artisan migrate
```

Acesse a aplicação pelo browser de sua preferência
```
http://localhost:8000/
```

### Dockerhub
Caminho das imagens que estão indicadas no arquivo docker-compose.yaml

- **App**: https://hub.docker.com/repository/docker/milsonei/code-education-laravel-app
- **Nginx**: https://hub.docker.com/repository/docker/milsonei/code-education-laravel-nginx
- **MySQL**: https://hub.docker.com/repository/docker/milsonei/code-education-laravel-mysql
- **Redis**: https://hub.docker.com/repository/docker/milsonei/code-education-laravel-redis
