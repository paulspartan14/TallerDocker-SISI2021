#### Construir contenedor

docker build -t myapi:v1 .

#### Correr contenedor

docker run -d --name container -p 3000:3000 myapi:v1

#### Ver procesos dentro de un contenedor

docker logs container -f

#### entrar al contenedor

docker exec -it container bash

#### Ver el SO del contenedor una vez dentro

uname -a

-------------------------------

#### mostrar comandos docker compose

#### correr servicios por separado

#### verificar que un contenedor ve a otro

#### al no ser root podemos ejecutar un:

docker exec -u 0 -it [container_id] bash

### si no deja hacer ping actualizas paquetes e instalas

apt-get update
apt-get install iputils-ping
