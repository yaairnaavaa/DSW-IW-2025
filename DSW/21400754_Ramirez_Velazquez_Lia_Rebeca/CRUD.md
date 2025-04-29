#  ***********************  ACTIVIDAD CRUD    *********************

# 1. Creación de pelicula
- Método HTTP: POST
- URI: /movies
- Json enviado:
```json
{
    "id" : "12",
    "nombre" : "Moonrise Kingdom",
    "director" : "Wes Anderson",
    "año" : "2007",
    "duración" : "100 min",
    "genero" : "Aventura"
}
```
- Json recibido:

```json
{
    "code" : 200,
    "msg" : "Pelicula Creada",
}
```

----

# 2. Consulta de pelicula por su ID
- Método HTTP: GET
- URI: /movies/10
- Json enviado:
```json
{

}
```
- Json recibido:
```json
{
    "code" : 200,
    "data" : {
         "id" : "10",
         "nombre" : "Oppen Haimer",
         "director" : "Christopher Nolan",
         "año" : "2024",
         "duración" : "130 min",
         "genero" : "Historia"
    },
}
```

----

# 3. Actualiza el año, director y duración de una película por su id
- Método HTTP: PUT
- URI: /movies/12
- Json enviado:
```json
{
    "director" : "Martin Scorccese",
    "año" : "2010",
}
```
- Json recibido:
```json
{
    "code" : 200,
    "msg" : "Pelicula actualizada"
}
```

---

# 4. Borra una película por su id.
- Método HTTP: DELETE
- URI: /movies/12
- Json enviado:
```json
{

}
```
- Json recibido:
```json
{
    "code" : 200,
    "msg" : "Pelicula eliminada"
}
```