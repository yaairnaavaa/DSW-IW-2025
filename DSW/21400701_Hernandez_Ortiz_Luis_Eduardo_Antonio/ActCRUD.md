1.- CREAR PELICULA:
Descripcion:
Se crea una nueva pelicula con el metodo post
Metodo HTTP: POST

URI: /Peliculas

Json enviado:
{
    "id" : 1,
    "nombre" : La toalla del mojado,
    "director" : Frankie,
    "año" : 1980,
    "duracion" : 30,
    "genero" : Dificil
}
Json recibido:
{
    "code" : 200,
    "msg" : "Pelicula creada"
}

2.- Consulta una pelicula por su id:
Descripcion:
Consukta de una pelicula poniendo su id en el URI
Metodo HTTP: GET

URI: /Peliculas/1

Json enviado:
{

}
Json recibido:
{
    "code" : 200,
    "data" : {
                "id" : 1,
                "nombre" : "La toalla del mojado",
                "director" : "Frankie",
                "año" : 1980,
                "duracion" : 30,
                "genero" : "Dificil"
             }
}

3.- Actualiza el año,director y duracion de una pelicula por su id:
Descripcion:
Actualiza una pelucula con su id en el URI y mandandole los datos actualizados
Metodo HTTP: PUT

URI: /Peliculas/1

Json enviado:
{
    "director" : "Frankie Rivers",
    "año" : 1970,
    "duracion" : 180,   
}
Json recibido:
{
    "code" : 201,
    "msg" : "Pelicula actualizada"
}

4.- Borra una pelicula por su id:
Descripcion:
Eliminar una pelicula mediante su id poniendolo en el URI
Metodo HTTP: DELETE

URI: /Peliculas/1

Json enviado:
{
    
}
Json recibido:
{
    "code" : 200,
    "msg" : "Pelicula eliminada"
}
