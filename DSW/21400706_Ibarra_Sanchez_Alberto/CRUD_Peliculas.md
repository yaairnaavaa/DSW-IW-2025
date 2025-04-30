# CRUD basico de peliculas

## Estructura de la pelicula

```bash
{
    "id" : Number,
    "nombre" : String,
    "director" : String,
    "año" : Number,
    "duración" : Number,
    "genero" : String
}
```

## Creacion de una pelicula

**Método HTTP:** POST
**URI:** /peliculas

**JSON enviado**
```bash
{
    "id" : 1,
    "nombre" : "Jurassic Park",
    "director" : "Steven Spielberg",
    "año" : 1993,
    "duración" : 127,
    "genero" : "Ciencia ficción"
}
```

**JSON recibido**
```bash
{
    "code": 200,
    "msj": "Pelicula creada con exito"
}
```

## Consultar peliculas

**Método HTTP:** GET
**URI:** /peliculas/id - /peliculas/5

**JSON enviado**
```bash
{

}
```

**JSON recido**
```bash
{
    "code" : 200,
    "data" : {
        "id" : 5,
        "nombre" : "Rocky",
        "director" : "John G. Avildsen",
        "año" : 1976,
        "duración" : 119,
        "genero" : "Deportes"
    }
}
```

## Actualizar una pelicula

**Método HTTP:** PUT
**URI:** /peliculas/id - /peliculas/3

**JSON enviado**
```bash
{
    "director" : "Guillermo del Toro",
    "duración" : 127
}
```

**JSON recibido**
```bash
{
    "code": 200,
    "msj": "Pelicula actualizada con exito"
}
```

## Eliminar una pelicula

**Método HTTP:** DELETE
**URI:** /peliculas/id - /peliculas/4

**JSON enviado**
```bash
{

}
```

**JSON recibido**
```bash
{
    "code": 200,
    "msj": "Pelicula eliminada con exito"
}
```