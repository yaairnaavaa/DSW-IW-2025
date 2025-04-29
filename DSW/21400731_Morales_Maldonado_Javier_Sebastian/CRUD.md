## Actividad: Crea el Flujo e interacción Cliente-Servidor para un CRUD básico de una tienda de películas:
**Descripción:** Crear una película.

**Método HTTP:** POST

**URI:** /pelicula/

**Json enviado:**
```bash
{
    "id" : 1,
    "nombre" : Cars,
    "director" : "John Lasseter",
    "año" : 2006,
    "duración" : 117,
    "genero" : "Infantil/Comedia"
}
```
**Json recibido:**
```bash
{
    "code" : "200",
    "msg" : "Pélicula creada"
}
```

**Descripción:** Consulta una película por su id.

**Método HTTP:** GET

**URI:** /pelicula/1

**Json enviado:**
```bash
{
    
}
```
**Json recibido:**
```bash
{
    "code" : 200,
    "data" : {
        "id" : 1,
        "nombre" : "Cars",
        "director" : "John Lasseter",
        "año" : 2006,
        "duración" : 117,
        "genero" : "Infantil/Comedia"
    }
}
```
**Descripción:** Actualiza el año, director y duración de una película por su id

**Método HTTP:** PUT

**URI:** /pelicula/1

**Json enviado:**
```bash
{
    "nombre" : "Cars 2",
    "año" : 2011
}
```
**Json recibido:**
```bash
{
    "code" : "201",
    "msg" : "Pélicula actualizada"
}
```

**Descripción:** Borra una película por su id.

**Método HTTP:** DELETE

**URI:** /pelicula/1

**Json enviado:**
```bash
{
    
}
```
**Json recibido:**
```bash
{
    "code" : "200",
    "msg" : "Pélicula eliminada"
}
```