## Actividad
# Oscar Gabriel Hernandez Samaniega

# CREAR PELICULA

Descripción: Crear una pelicula

Método HTTP: POST

URI: /peliculas

Json enviado:

{
    "id": 1,
    "nombre": "Inception",
    "director": "Christopher Nolan",
    "año": 2010,
    "duración": 148,
    "genero": "Ciencia ficción"
}

Json recibido:

{
    "code" : 200,
    "msg" : "Pelicula añadida",
}

# CONSULTAR PELICULA

Descripción: consultar pelicula

Método HTTP: GET

URI: /peliculas/1

Json enviado:

{

}

Json recibido:

{
    "code" : 200,
    "data" : {
                "nombre": "Inception",
                "director": "Christopher Nolan",
                "año": 2010,
                "duración": 148,
                "genero": "Ciencia ficción"
             }
}

# ACTUALIZAR PELICULA

Descripción: Actualizar una pelicula

Método HTTP: PUT

URI: /peliculas/1

Json enviado:

{
    "año" : 2011,
    "genero" : "Accion"
}

Json recibido:

{
    "code" : 201,
    "msg" : "Pelicula actualizada"
}

# ELIMINAR PELICULA

Descripción: Eliminar una pelicula

Método HTTP: DELETE

URI: /peliculas/1

Json enviado:

{

}

Json recibido:

{
    "code" : 200,
    "msg" : "Pelicula eliminada"
}

