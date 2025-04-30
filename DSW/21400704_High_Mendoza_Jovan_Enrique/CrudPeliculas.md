**POST**

Descripcion: Post de la creacion de una pelicula
Metodo HTTP: POST
URI: /movie
JSON enviado:
{
    "id": 1,
    "nombre": "Volver al futuro",
    "director": "Robert Zemeckis",
    "año": 1985,
    "duración": 116,
    "genero": "Infantil/Ciencia ficción"
}

**JSON Recibido: 
{
    status: 200
}

**GET**
**Descripcion: Get de una pelicula por 1
**Metodo HTTP: GET
**URI: /movie/1
**JSON enviado:
{
    "id": 1
}

**JSON Recibido: 
{
    "id": 1,
    "nombre": "Volver al futuro",
    "director": "Robert Zemeckis",
    "año": 1985,
    "duración": 116,
    "genero": "Infantil/Ciencia ficción"
}

**PUT**
**Descripcion: Actualizar el año, director y duracion de una pelicula por id
**Metodo HTTP: PUT
**URI: /movie/1
**JSON enviado:
{
    "id": 1,
    "nombre": "Volver al futuro",
    "director": "Robert Z.",
    "año": 1995,
    "duración": 100,
    "genero": "Infantil/Ciencia ficción"
}

**JSON Recibido: 
{
    status: 200
}
**DELETE**
**Descripcion: Borrar una pelicula por id
**Metodo HTTP: DELETE
**URI: /movie/1
**JSON enviado:
{
   
}

**JSON Recibido: 
{
    status: 200
}