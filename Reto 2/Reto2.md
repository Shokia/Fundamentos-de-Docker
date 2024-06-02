# Quiz 2

## Paso 1: Crear la red Docker
Comando Utilizado: docker network create teemii-network


## Paso 2: Crear volumen Docker y ejecutar el Contenedor del Back-end
Crear el volumen: docker volume create teemii-backend-data

![Alt Text](volumen.png)

Comando Utilizado: docker run -d --name teemii-backend --network teemii-network -v teemii-backend-data:/data -p 3000:3000 dokkaner/teemii-backend:develop

![Alt Text](backend.png)

## Paso 3: Ejecutar el Contenedor del Front-end
Comando Utilizado: docker run -d --name teemii-frontend --network teemii-network -p 8080:80 dokkaner/teemii-frontend:develop

![Alt Text](Frontend.png)

## Paso 4: Verificar los contenedores
Comando utilizado: docker ps

![Alt Text](verificar.png)

## Paso 5: Acceder a la página
http://localhost:8080

![Alt Text](pagina.png)

## Paso 6: Añadir Manga

![Alt Text](manga.png)

## Paso 7: Eliminar el contenedor back-end y volver a crear el contenedor backend
Comando Utilizado: docker rm -f teemii-backend
Comando Utilizado: docker run -d --name teemii-backend --network teemii-network -v teemii-backend-data:/data -p 3000:3000 dokkaner/teemii-backend:develop
