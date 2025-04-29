## CRUD DE PELICULAS

## Creación de una pelicula
- **Método HTTP**: POST
- **URI**: /movies
**Json enviado:**
```json
{
    "id" : 1,
    "nombre" : “Minecraft”,
    "director" : “Robert”,
    "año" : 2024,
    "duración" : 100,
    "genero" : “Infantil”
}
```
**Json recibido:**
```json
{
    "code" : 200,
    "msg" : "Pelicula creada",
}
```

## Consultar película por id
- **Método HTTP**: GET
- **URI**: /movies/1
**Json enviado:**
```json
{
}
```
**Json recibido:**
```json
{
    "id" : 1,
    "nombre" : “Minecraft”,
    "director" : “Robert”,
    "año" : 2024,
    "duración" : 100,
    "genero" : “Infantil”
}
```

## Actualizar película por id
- **Método HTTP**: PUT
- **URI**: /movies/1
**Json enviado:**
```json
{
“director”: “Jhon”
“duración”:120
}
```
**Json recibido:**
```json
{
    "code" : 200,
    "msg" : "Pelicula Actualizada",
}
```

## Eliminar película por id
- **Método HTTP**: DELETE
- **URI**: /movies/1
**Json enviado:**
```json
{
}
```
**Json recibido:**
```json
{
    "code" : 200,
    "msg" : "Pelicula Eliminada",
}
```
