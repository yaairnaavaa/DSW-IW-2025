# 1. Crear una película.
* ## Descripcion
Crear una pelicula

* ## Metodo HTTP
POST

* ## URI
api/peliculas

* ## Json enviado
{
    "id" : 1,
    "nombre" : Titanic,
    "director" : James Cameron,
    "año" : 1998,
    "duración" : 1:39,
    "genero" : Romantica
}

* ## Json recibido
{
    "code" : 200,
    "msg" : "Pelicula Creada",
}

---

# 2. Consulta una película por su id.
* ## Descripcion
Consultar una pelicula por su id

* ## Metodo HTTP
GET

* ## URI
api/peliculas/1

* ## Json enviado
{

}

* ## Json recibido
{
    "code" : 200,
    "data" : {
        "id" : 1,
        "nombre" : Titanic,
        "director" : James Cameron,
        "año" : 1998,
        "duración" : 1:39,
        "genero" : Romantica
    }
}
---

# 3. Actualiza el año, director y duración de una película por su id
* ## Descripcion
Actualizar el año, director y duración de una pelicula por su id

* ## Metodo HTTP
PUT

* ## URI
api/peliculas/1

* ## Json enviado
{
    "director" : Alberto Pardo,
    "año" : 2003,
    "duración" : 24:24,
}

* ## Json recibido
{
    "code" : 201,
    "msg" : "Pelicula Actualizada"
}

---

# 4. Borra una película por su id.
* ## Descripcion
Eliminar una pelicula por su id

* ## Metodo HTTP
DELETE

* ## URI
api/peliculas/1

* ## Json enviado
{

}

* ## Json recibido
{
    "code" : 200,
    "msg" : "Pelicula Eliminada"
}