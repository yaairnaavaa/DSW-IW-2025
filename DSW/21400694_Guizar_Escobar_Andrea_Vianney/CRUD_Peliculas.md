
# Actividad CRUD básico películas

## Crea el flujo e interacción Cliente - Servidor para un CRUD básico de una tienda de películas.
- Crear una película.
- Consulta una película por su id.
- Actualiza el año, director y duración de una película por su id.
- Borra una película por su id.

## Estructura cada película.
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
---
## Creación de una película
**Descripción:** Permite al cliente registrar una nueva película, se envían los datos completos de la película en formato JSON y se confirma la creación.

**Método HTTP:** `POST`

**URI:** `/movies`

**JSON enviado:**
```bash
{
    "id" : 1,
    "nombre" : "El cadáver de la novia",
    "director" : "Tim Burton",
    "año" : 2005,
    "duración" : 77,
    "genero" : "Fantástico Gótico"
}
```

**JSON recibido:**
```bash
{
    "code" : 200,
    "msg" : "Película creada"
}
```
---
## Consultar una película por su id
**Descripción:** Permite al cliente solicitar información de una película específica por su id, se devuelven todos los datos de la película si esta existe.

**Método HTTP:** `GET`

**URI:** `/movies/{id}`
- `/movies/2`

**JSON enviado:**  
```bash
{

}
```

**JSON recibido:**
```bash
{
    "code" : 200,
    "data" : {
        "id" : 2,
        "nombre" : "Mi madrina es una hechicera",
        "director" : "Ezekiel Norton",
        "año" : 2005,
        "duración" : 46,
        "genero" : "Comedia"
    }
}
```
---
## Actualizar el año, director y duración de una película por su id.
**Descripción:** Permite actualizar campos específicos, en este caso el año, director y duración de una película existente por su id, se realizan los cambios y se confirma la actualización.

**Método HTTP:** `PUT`

**URI:** `/movies/{id}`
- `/movies/2`

**JSON enviado:**
```bash
{
    "director" : "Terry Klassen",
    "año" : 2004,
    "duración" : 47
}
```

**JSON recibido:**
```bash
{
    "code" : 201,
    "msg" : "Película actualizada"
}

```
---
## Borra una película por su id.
**Descripción:** Permite eliminar una película del por su id, cuando se realiza, se muestra un mensaje de confirmación.

**Método HTTP:** `DELETE`

**URI:** `/movies/{id}`
- `/movies/2`

**JSON enviado:**  
```bash
{

}

```

**JSON recibido:**
```bash
{
    "code" : 201,
    "msg" : "Película eliminada"
}

```
---
## 21400694 - Guizar Escobar Andrea Vianney
