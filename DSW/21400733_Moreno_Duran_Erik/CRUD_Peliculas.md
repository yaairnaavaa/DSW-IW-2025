
## Crear una pelicula

Descripción: Crear una pelicula con el metodo POST, enviando la informacion en un JSON

Método HTTP: POST

URI: /pelicula

Json enviado: 
```JSON
{
    "id" : 123,
    "nombre" : "Star wars",
    "director" : "No se",
    "año" : 1999,
    "duración" : 98,
    "genero" : "Ciencia ficcion"
}
```

Json recibido:
```JSON
{
    "code" : 200,
    "msg" : "Pelicula Creada",
}
```

## Consulta una película por su id

Descripción: Consultar una pelicula con el metodo get pasando la id por la URI

Método HTTP: GET

URI: /pelicula/123

Json enviado:

```JSON
{

}
```

Json recibido:
```JSON
{
    "code" : 200,
    "data" {
        "id" : 123,
        "nombre" : "Star wars",
        "director" : "No se",
        "año" : 1999,
        "duración" : 98,
        "genero" : "Ciencia ficcion"
    }
}
```

## Actualiza el año, director y duración de una película por su id

Descripción: Actualizar la informacion de la pelicula por su id con el metodo PUT

Método HTTP: PUT

URI: /pelicula/123

Json enviado: 
```JSON
{
    "director" : "sigo sin saber",
    "año" : 1995,
    "duración" : 105,
}
```

Json recibido:
```JSON
{
    "code" : 201,
    "msg" : "Pelicula Actualizada",
}
```

## Borra una película por su id

Descripción: Eliminar una pelicula con el metodo DELETE por su id

Método HTTP: DELETE

URI: /pelicula/id

Json enviado: 

```JSON
{

}
```

Json recibido:
```JSON
{
    "code" : 200,
    "msg" : "Pelicula Eliminada",
}
```