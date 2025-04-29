Crea el Flujo e interaccion Cliente-Servidor para un CRUD basico de una tienda de peliculas:

    1.Crear una pelicula.

    2.Consulta una pelicula por su id.

    3.Actualiza el ano, director y duracion de una pelicula por su id

    4.Borra una pelicula por su id.

DESCRIPCION>  Crear una pelicula:
METODO HTTTP> POST
URI> TIENDA/PELICULA
JSON ENVIADO>
    {
        "id" : 20,
        "nombre" : Interstellar ,
        "director" : Christopher Nolan,
        "ano" : 2014,
        "duracion" : 169,
        "genero" : Ciencia Ficcion
    }
JSON RECIBIDO>
    {
        "code" : 200,
        "msg" : "Pelicula Publicada",
    }
/////////////////////////////////////////////////////////////////////////

DESCRIPCION> Consulta una pelicula por su id.
METODO HTTTP> GET
URI> TIENDA/PELICULA/20
JSON ENVIADO>
    {


    }

JSON RECIBIDO>
    {
        "id" : 20,
        "nombre" : Interstellar ,
        "director" : Christopher Nolan,
        "ano" : 2014,
        "duracion" : 169,
        "genero" : Ciencia Ficcion
    }
/////////////////////////////////////////////////////////////////////////
DESCRIPCION> Actualiza el ano, director y duracion de una pelicula por su id
METODO HTTTP> PUT
URI> TIENDA/PELICULA/20
JSON ENVIADO>
    {
        "ano" : 2015
        "director" : Guillermo del Toro
        "duracion" : 170

    }
JSON RECIBIDO>
    {
        "code" : 201,
        "msg" : "Pelicula Actualizada",
    }
/////////////////////////////////////////////////////////////////////////

DESCRIPCION>  Borra una pelicula por su id:
METODO HTTTP> DELETE
URI> TIENDA/PELICULA/20
JSON ENVIADO>
    {

    }
JSON RECIBIDO>
    {
        "code" : 203,
        "msg" : "Pelicula Eliminada",
    }
/////////////////////////////////////////////////////////////////////////