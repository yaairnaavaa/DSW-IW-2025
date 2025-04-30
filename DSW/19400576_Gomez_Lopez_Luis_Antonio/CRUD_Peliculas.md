## CRUD de Peliculas

## Crea el Flujo e interacción Cliente-Servidor para un CRUD básico de una tienda de películas:
- Crear una película.
- Consulta una película por su id.
- Actualiza el año, director y duración de una película por su id
- Borra una película por su id.

<br>

##  Crear una película
**Descripcion:** Creacion de un registro de pelicula por medio de un GET y obteniendo como resultado la confirmacion de la creacion

**Metodo HTTP:** POST

**URL:** /movie/add

**Json Enviado**

```json
{
    "id" : 9,
    "nombre" : "El Santo VS Las Momias",
    "director" : "Guillermo del Toro",
    "año" : 2015,
    "duración" : 180,
    "genero" : "Acción, Comedia, Cine mexicano"
}
```
**Json Recibido**
```json
{
    "succes":true,   
    "msg":"Registro insertado correctamente"
}
```  
<br>

## Consulta una película por su id
**Descripcion:** Consulta de un registro existente por medio de la ID

**Metodo HTTP:** GET

**URL:** /movie?id=9

**Json Enviado**

```json
    
```
**Json Recibido**
```json
{
    "id" : 9,
    "nombre" : "El Santo VS Las Momias",
    "director" : "Guillermo del Toro",
    "año" : 2015,
    "duración" : 180,
    "genero" : "Acción, Comedia, Cine mexicano"
}
```
<br>

## Actualiza el año, director y duración de una película por su id
**Descripcion:** Modificar un registro existente por medio de la ID

**Metodo HTTP:** PUT

**URL:** /movie/update?id=9

**Json Enviado**

```json
    {
    "director" : "Guillermo del Toro y James Gunn",
    "año" : 2023,
    "duración" : 200,
}
```
**Json Recibido**
```json
{
    "id" : 9,
    "nombre" : "El Santo VS Las Momias",
    "director" : "Guillermo del Toro y James Gunn",
    "año" : 2023,
    "duración" : 200,
    "genero" : "Acción, Comedia, Cine mexicano"
}
```
<br>

## Borra una película por su id.
**Descripcion:** Eliminar un registro existente por medio de su ID

**Metodo HTTP:** DELETE

**URL:** /movie/delete?id=9

**Json Enviado**

```json
    
```
**Json Recibido**
```json
{
    "succes":true,   
    "msg":"Registro eliminado correctamente"
}
```