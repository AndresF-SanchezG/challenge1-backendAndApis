# Timestamp Microservice

Build a full stack JavaScript app that is functionally similar to this: https://timestamp-microservice.freecodecamp.rocks.

Este código es para una aplicación de Node.js que configura una API básica utilizando el marco de trabajo Express.js. La aplicación proporciona puntos finales para manejar solicitudes relacionadas con fechas y devolver marcas de tiempo Unix y cadenas UTC correspondientes. Aquí tienes una explicación del código:

Importación de Módulos:

Los módulos requeridos, express y cors, se importan para crear el servidor y habilitar el intercambio de recursos entre diferentes orígenes (CORS, por sus siglas en inglés).
Inicialización de la Aplicación Express:

Se crea una instancia de la aplicación Express utilizando express().
Configuración de CORS:

CORS se habilita mediante el middleware cors para permitir pruebas remotas de la API.
A los navegadores antiguos que podrían tener problemas con una respuesta 204 se les envía un estado 200.
Servicio de Archivos Estáticos:

La aplicación sirve archivos estáticos ubicados en el directorio "public". Esto es útil para servir archivos del lado del cliente, como CSS, imágenes y JavaScript.
Enrutamiento Básico:

Cuando se realiza una solicitud a la ruta raíz ("/"), el servidor envía el archivo "index.html" ubicado en el directorio "views".
Función de Validación de Fechas:

Se define la función isInvalidDate(date) para verificar si una fecha dada es válida comparando su representación de cadena UTC con "Invalid Date".
Punto Final de la API para Conversión de Fechas:

Se crea un punto final de API (/api/:date) para manejar solicitudes con un parámetro de fecha proporcionado.
El parámetro se utiliza para crear un objeto JavaScript Date.
Si la fecha no es válida, se verifica si el parámetro es un valor numérico (marca de tiempo Unix).
Si la fecha sigue siendo inválida, se envía una respuesta de error.
Si la fecha es válida, el servidor responde con un objeto que contiene la marca de tiempo Unix y la representación de cadena UTC de la fecha.
Punto Final de API por Defecto:

Se define otro punto final de API (/api) para los casos en que no se proporcione un parámetro de fecha.
Responde con la marca de tiempo Unix actual y la representación de cadena UTC.
Escucha del Servidor:

El servidor comienza a escuchar en el puerto especificado en la variable process.env.PORT.
Se registra un mensaje para indicar que el servidor está en ejecución y escuchando en el puerto especificado.
En resumen, este código crea una aplicación sencilla de Express.js que sirve archivos estáticos, maneja solicitudes de API relacionadas con la conversión de fechas y responde con marcas de tiempo Unix y cadenas UTC. Es un ejemplo básico de cómo construir una API RESTful utilizando Node.js y Express.js.
  
# Solution Challenge
In this challenge I tried to get as close as possible to your solution:
- Live Site URL: [Replit](https://replit.com/@AndresF-Sanchez/boilerplate-project-timestamp-3)

# Author

- Author - [@AndresF-SanchezG](https://github.com/AndresF-SanchezG)
- School - [Freecodecamp](https://www.freecodecamp.org/)
- Curse - [Timestamp Microservice](https://www.freecodecamp.org/learn/back-end-development-and-apis/back-end-development-and-apis-projects/timestamp-microservice)







