### correr un nginx

docker run -d --name mynginx -p 8084:80 nginx

#### Construir contenedor

docker build -t myapi:v1.0 .

#### Correr contenedor

docker run -d --name container -p 3000:3000 myapi:v1

#### Ver procesos dentro de un contenedor

docker logs container -f

#### entrar al contenedor

docker exec -it container bash

#### Ver el SO del contenedor una vez dentro

uname -a

#### construir la imagen y subirla a docker hub

```
docker build -t myapi:v1.0 .

### iniciar sesion
docker login

### asignar un tag
docker tag myapi:v1.0 paulspartan/myapi:v1.0

### subir contenedor a dockerhub
docker push paulspartan/myapi:v1.0

### correr nuestro contenedor desde nuestra imagen creada
docker run -d -p 3000:3000 --name api-hub paulspartan/myapi:v1.0

```
