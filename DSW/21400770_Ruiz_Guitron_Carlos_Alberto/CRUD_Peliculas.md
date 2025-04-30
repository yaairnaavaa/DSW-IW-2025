# Estructura basica  de peliculas: 
{
    "id" : Number,
    "nombre" : String,
    "director" : String,
    "año" : Number,
    "duración" : Number,
    "genero" : String
}

# Crear una película.
{
    Método HTTP: POST

    URI: /pelicula

    Json enviado:
    {
        "id"       : 100,
        "nombre"   : "Gladiator",
        "director" : "Ridley s"
        "año"      : 1997,
        "duración" : 155,
        "genero"   : "pélpum, acción, drama historico"
    }

    Json recibido:
    {
        "code" : 200,
        "msg"  : "Pelicula agreda correctamente"
    }
}


# Consulta una película por su id.
{
    Método HTTP: GET

    URI: /pelicula/100

    Json enviado:
    {
        
    }

    Json recibido:
    {
        "code" : 200,
        "data" {
            "id"       : 100,
            "nombre"   : "Gladiator",
            "director" : "Ridley s"
            "año"      : 1997,
            "duración" : 155,
            "genero"   : "pélpum, acción, drama historico"
        }
    }
}

# Actualiza el año, director y duración de una película por su id
{
    Método HTTP: PUT

    URI: /pelicula/100

    Json enviado:
    {
        "director" : "Ridley Scott"
        "año"      : 1998,
    }

    Json recibido:
    {
        "code" : 200,
        "msg"  : "Pelicula actualizada"
        "data" {
            "id"       : 100,
            "nombre"   : "Gladiator",
            "director" : "Ridley Scott"
            "año"      : 1998,
            "duración" : 155,
            "genero"   : "pélpum, acción, drama historico"
        }
    }
}
# Borra una película por su id.
{
    Método HTTP: DELETE

    URI: /pelicula/100

    Json enviado:
    {

    }

    Json recibido:
    {
        "code" : 200,
        "msg"  : "Pelicula Eliminada"
    }
}