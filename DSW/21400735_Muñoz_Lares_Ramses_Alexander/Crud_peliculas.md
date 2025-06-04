# Crud Basico Cliente-Servidor. Mi tiendita de pelis

## Crea el Flujo e interacción Cliente-Servidor para un CRUD básico de una tienda de películas:
- Crear una película.
- Consulta una película por su id.
- Actualiza el año, director y duración de una película por su id
- Borra una película por su id.

## Estructura cada película:
``` json
{
    "id" : Number,
    "nombre" : String,
    "director" : String,
    "año" : Number,
    "duración" : Number,
    "genero" : String
}
```
## Estructura de cada punto:

- Descripción: 
- Método HTTP: 
- URL: 
- Json enviado:
- Json recibido:

## Crear una Pelicula
- Descripción: 
    Se desea crear una pelicula empleando el metodo POST mediante informacion proveniente de un JSON.
- Método HTTP: POST
- URL: /pelicula
- Json enviado:
``` json
{
    "id" : 1,
    "nombre" : "Scarface",
    "director" : "Brian De palma",
    "año" : 1983,
    "duración" : 165,
    "genero" : "accion"
}
```
- Json recibido:
``` json
{
    "code" : 200,
    "msg"  : "Pelicula Agregada"
}
```
## Consulta una película por su id

- Descripción: 
    Se desea consutar una pelicula mediante el id empleando el metodo GET.
- Método HTTP: GET
- URL: /pelicula/2
- Json enviado:
``` json
{


}
```
- Json recibido:
``` json
{
    "id" : 2,
    "nombre" : "El lobo de wall street",
    "director" : "Martin Scorsese",
    "año" : 2013,
    "duración" : 180,
    "genero" : "Drama, Comedia"
}
```
## Actualiza el año, director y duración de una película por su id

- Descripción: 
    Se desea Actualizar parametros especificos de una pelicula mediante el id empleando el metodo PUT.
- Método HTTP: PUT
- URL: /pelicula/1
- Json enviado:
``` json
{
    "director" : "Pancho Pantera",
    "año" : 2015,
    "duración" : 179
}
```
- Json recibido:

``` json
{
    "code" : 200,
    "msg"  : "Pelicula Actualizada"
}
```
## Borra una película por su id.

- Descripción: 
    Se desea Eliminar una pelicula mediante el id empleando el metodo DELETE.
- Método HTTP: DELETE
- URL: /pelicula/1
- Json enviado:
``` json
{


}
```
- Json recibido:
``` json
{
    "code" : 200,
    "msg"  : "Pelicula Eliminada"
}
```
e todo.