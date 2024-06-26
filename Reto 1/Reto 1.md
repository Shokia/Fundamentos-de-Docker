# Tema 1: Descargando mi primer imagen

### Para este reto, necesitarán descargar una imagen específica de Docker Registry y ponerla en ejecución.
### 1. Descarguen la imagen `nginx:latest` de Docker Registry.
### 2. Inicien un contenedor a partir de esta imagen. Exponerlo al puerto 8080 de su computadora.
### 3. Asegúrense de que el contenedor esté en ejecución y de que puedan acceder al servidor Nginx a través de un navegador web. Esto lo pueden verificar usando la direccion [`http://localhost:8080`](http://localhost:8080/) en el navegador
### 4. Tomen una captura de pantalla del navegador web mostrando la página de bienvenida de Nginx y envíenla como evidencia al profesor de que completaron el reto.

Recuerden, el objetivo de este reto es validar lo que ya aprendieron. ¡Buena suerte!

## Paso 1: Descarga la imagen
docker pull nginx:latest

![Alt Text](Descargar.png)

## Paso 2: Iniciar contenedor
docker run --name my-nginx -p 8080:80 -d nginx:latest

![Alt Text](Iniciar.png)

## Paso 3: Verificar contenedor
docker ps

![Alt Text](Check.png)

## Paso 4: Acceder al servidor Nginx a través de un navegador web

## Paso 5: Captura

![Alt Text](captura.png)





