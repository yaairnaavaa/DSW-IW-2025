Crear el flujo e interaccion Cliente-Servidor para un CRUD basico de una tienda de peliculas

1.- Crear una pelicula
2.- Consultar Pelicula por ID
3.- Actualizar año, Director y duracion de una pelicula por su ID
4.- Borra una pelicula por ID

~Estructura para pelicula~

{
	"id" : Number,
	"nombre" : String,
	"director" : String,
	"año" : Number,
	"duración" : Number,
	"genero" : String	
}

~Estructura de cada punto~

Descripcion: Creacion de una pelicula
Metodo HTTP: POST
URI: /peliculas
JSON Enviado:
{
	"id" : 1,
	"nombre" : Wallace and Gromit: The Curse of the Were-Rabbit,
	"director" : Nick Park
	"año" : 2005,
	"duración" : 85 min,
	"genero" : Animacion	
}
JSON Recibido:
{
    "code" : 200,
    "msg" : "Pelicula Creada"
}


Descripcion: Consultar Pelicula por ID
Metodo HTTP: GET
URI: /peliculas/1
JSON Enviado:
{

}
JSON Recibido:
{
    "code" : 200,
    "data" : {
        	"id" : 1,
            "nombre" : Wallace and Gromit: The Curse of the Were-Rabbit,
            "director" : Nick Park
            "año" : 2005,
            "duración" : 85 min,
            "genero" : Animacion
            }
}

Descripcion: Actualizar año de pelicula
Metodo HTTP: PUT
URI: /peliculas/1
JSON Enviado:
{
    "año" : 2000
}
JSON Recibido:
{
    "code" : 200,
    "msg" : "Pelicula Actualizada"
}

Descripcion: Actualizar Director de pelicula
Metodo HTTP: PUT
URI: /peliculas/1
{
    "director" : Steve Box
}
JSON Recibido:
{
    "code" : 200,
    "msg" : "Pelicula Actualizada"
}

Descripcion: Actualizar duracion de pelicula
Metodo HTTP: PUT
URI: /peliculas/1
{
    "duracion" : 100min
}
JSON Recibido:
{
    "code" : 200,
    "msg" : "Pelicula Actualizada"
}

Descripcion: Eliminar una pelicula
Metodo HTTP: Delete
URI: /peliculas/1
JSON Enviado:
{

}
JSON Recibido:
{
    "code" : 200,
    "msg" : "Pelicula Eliminada"
}