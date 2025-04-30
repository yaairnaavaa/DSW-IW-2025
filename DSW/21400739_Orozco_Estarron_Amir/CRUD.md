#CRUD DE PELICULAS

## 1.Crear una pelicula
### Descripcion: 
    Envio de los datos de la nueva pelicula
### Metodo HTTP: 
    POST
### URI: 
    /books
### JSON ENVIADO:
    {
        "id" : 1,
        "nombre" : "CORALINE",
        "Director" : "Neil Gaiman",
        "anio" : 2002,
        "duracion" : 100,
        "genero" : "Fantasia y terror"
    }
### JSON RECIBIDO
    {
        "code" : 200,
        "msg" : "Pelicula creada",
    }

## 2.Consultar una pelicula por su ID
### Descripcion: 
    Consultar una pelicula por su ID
### Metodo HTTP: 
    GET
### URI:
    /books/2
### JSON ENVIADO:
    {

    }
### JSON RECIBIDO
    {
    "code" : 200,
    "data" : {
               "id" : 2,
               "nombre" : "Los increibles 2",
               "Director" : "Brad bird",
               "anio" : 2004,
               "duracion": 126,
               "genero" : "Animado"
             }
}

## 3.Actualiza el año, director y duracion de una pelicula por su id
### Descripcion: 
    Enviar datos actualizados
### Metodo HTTP: 
    PUT
### URI:
    /books/2
### JSON ENVIADO:
    {
    "anio" : 2005,
    "director" : "Neil Gaiman",
    "duracion" : 130
}
### JSON RECIBIDO
    {
    "code" : 201,
    "msg" : "Pelicula actualizada"
    }

## 4.Borra una pelicula por su id.
### Descripcion: 
    Eliminar una pelicula por su id
### Metodo HTTP: 
    DELETE
### URI:
    /books/3
### JSON ENVIADO:
    {

    }
### JSON RECIBIDO
    {
    "code" : 200,
    "msg" : "pelicula eliminada"
    }