# NodePop-API
 run the app:
     $ DEBUG=nodepop:* npm start
     # Introduction
- Proyecto backend del API de la app Nodepop, creada como practica parte del curso de Desarrollo Backend con Node.js del Bootcamp Web (Mujeres en el sector tech) de Keepcoding.
- El servicio mantiene anuncios de compra o venta de artículos y permite consultar,  y buscar filtros por varios criterios.
- Además puedes visitar un site con los anuncios en la base de datos de nodepop después de iniciar la app ingresando al url [http://localhost:3000/](http://localhost:3000/).

## Overview

- **Tecnologías:** Este proyecto usa EXPRESS, MongoDB, mongoose y Node.js. Se puede conocer las dependencias en `package.json`.

- El Api de nodepop esta basada en principios REST y usa los métodos HTTP(GET y POST) para acceder a los recursos.

- El formato de transferencia soportado por el API para enviar y recibir respuestas es en JSON.

### MongoDB
Para este proyecto es necesario tener instalado MongoDB. Primero vamos a arrancar un servidor MongoDB local escribiendo la siguiente lìnea en un terminal:

```shell
> ./bin/mongod --dbpath ./data/db --directoryperdb
```

### Instalación de dependencias
Un paso importante antes de arrancar el servidor es instalar todas las dependencias del proyecto. Para hacerlo, en un terminal ejecutamos lo siguiente:

```shell
> npm install
```
### Inicializar Base de Datos
En este proceso se crearà y cargará una colección de documentos de la base de datos necesaria para el funcionamiento de la aplicación 'nodepop', para esto ejecutamos el script `installDB` dentro del package.json:
```shell
> npm run installDB
```

### Iniciar App
Hay varias formas de iniciar o arrancar nodepop:
- En modo DEBUG para el desarrollo, ejecutamos en un terminal:
```shell
> npm run dev
```
- En modo Produción, ejecutamos:
```shell
> npm run prod
```
