# Crea el Flujo e interacción Cliente-Servidor para un CRUD básico de una tienda de películas:
- Crear una película.
- Consulta una película por su id.
- Actualiza el año, director y duración de una película por su id
- Borra una película por su id.

# Estructura para cada pelicula
{
    "id" : Number,
    "nombre" : String,
    "director" : String,
    "año" : Number,
    "duración" : Number,
    "genero" : String
}

## Actividad ##

1. Crear una pelicula
- Descripción: Creacion de una pelicula

- Método HTTP: POST

- URI: /movies

# JSON enviado:
{
    "id" : 4,
    "nombre" : "El Resplandor",
    "director" : "Stanley Kubric",
    "año" : 2003,
    "duración" : 180,
    "genero" : "Terror,Drama,Suspenso"
}

# JSON recibido:
{
    "code" : 200,
    "message" : "Pelicula Creada"
}

2. Consultar pelicula por id
- Descripción: Consultar una pelicula por su ID

- Método HTTP: GET

- URI: /movies/4

# JSON enviado:
{
    
}

# JSON recibido:
{
    "id" : 4,
    "nombre" : "El Resplandor",
    "director" : "Stanley Kubric",
    "año" : 2003,
    "duración" : 180,
    "genero" : "Terror,Drama,Suspenso"  
}

3. Actualizar pelicula
- Descripción: Actualizar el director, año y duracion de una pelicula

- Método HTTP: PUT 

- URI: /movies/4

# JSON enviado:
{
    "director" : "Mel Gibson",
    "año" : 1999,
    "duración" : 126
}

# JSON recibido:
{
    "code" : 201,
    "message" : "Pelicula Actualizada"
}

4. Borrar pelicula
- Descripción: Eliminar una pelicula por su ID

- Método HTTP: DELETE

- URI: /movies/4

# JSON enviado:
{

}

# JSON recibido:
{
    "code" : 200,
    "message" : "Pelicula Eliminada :("
}
