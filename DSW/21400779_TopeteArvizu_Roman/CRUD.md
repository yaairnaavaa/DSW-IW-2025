```json

Descripción: CREACION DE UNA PELICULA

Método HTTP: POST

URI: /movies

Json enviado:

{
    "id" : 1,
    "nombre" : "Babadook",
    "director" : "Jennifer Kent",
    "año" : 2014,
    "duración" : 94,
    "genero" : "Horror"
}


Json recibido:

{
    "code" : 200,
    "msg" : "Movie created",
}


Descripción: CONSULTA DE UNA PELICULA POR ID

Método HTTP: GET

URI: /movies/1

Json enviado:

{

}

Json recibido:

{
    "code": 200,

    "data":  {
    "id" : 1,
    "nombre" : "Babadook",
    "director" : "Jennifer Kent",
    "año" : 2014,
    "duración" : 94,
    "genero" : "Horror"
    }
}





Descripción: Actualiza el año, director y duración de una película por su id

Método HTTP: PUT

URI: /movies/1

Json enviado:

{
    "year": 2020,
    "director": "Cristopher Nolan",
    "duracion": 120
}


Json recibido:

{
    "code" : "201",
    "msg"  : "Movie successfully updated"   
}


Descripción: Borra una pelicula por su id

Método HTTP: DELETE

URI: /movies/1

Json enviado:
{

}

Json recibido:

{
    "code" : 200,
    "message": "Movie successfully deleted"
    
}