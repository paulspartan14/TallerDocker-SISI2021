# instalar docker ubuntu

`curl -fsSL https://get.docker.com -o get-docker.sh`
`sudo sh get-docker.sh`

# usar docker como usuario no root (opcional)
`sudo usermod -aG docker your-user`

```
sudo curl -L https://github.com/docker/compose/releases/download/1.21.2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
```

`sudo chmod +x /usr/local/bin/docker-compose`

# que es docker

#### que problema resuelve docker

#### como construir una imagen con docker (crear imagen)

#### como crear contenedor a partir de una imagen

#### despues de crear el contenedor comandos basicos para ver el contenedor, eliminar contenedor e imagenes

#### para eliminar contenedor usas 
 - docker rm -fv [container]
 
#### forcevolume fuerza a detener el contenedor y elimina el volumen que creo

#### que es docker compose

#### que facilita docker compose

#### crear base de datos y web docker

#### monitorear contenedores 

`docker stats`

# limpiar espacio

`docker system prune`

#### ver informacion del contenedor

`docker inspect 'name | id container'`

#### diferencia host y contenedor, (host somos nosotros)

prometheus

https://grafana.com/grafana/dashboards/893