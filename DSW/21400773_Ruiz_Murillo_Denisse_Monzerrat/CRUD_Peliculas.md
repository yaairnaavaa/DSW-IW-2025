#CRUD_Pelicula

**Descripcion:** Mostrar una pelicula
**Metodo HTTP:** GET
**URI:** /pelicula/2
**JSON Enviado:**
```
{

}
```
**JSON Recibido:** 
```
{
    "code": 200,
    "data":
        {
        "id": 2,
        "nombre": "Barbie: Escuela de Princesas",
        "director": "Ezekiel Norton",
        "año": 2011,
        "duracion": 81,
        "genero": "Fantasía y familiar"
        }
}
```

**Descripcion:** Agregar una pelicula
**Metodo HTTP:** POST
**URI:** /pelicula
**JSON Enviado:**
```
{
    "nombre": "Barbie: Escuela de Princesas",
    "director": "Ezekiel Norton",
    "año": 2011,
    "duracion": 81,
    "genero": "Fantasía y familiar"
}
```
**JSON Recibido:** 
```
{
    "code":200,
    "msg":"Pelicula agregada exitosamente"
}
```
**Descripcion:** Actualizar una pelicula
**Metodo HTTP:** PUT
**URI:**/pelicula/2
**JSON Enviado:**
```
    {
        "año":2012
    }
```
**JSON Recibido:** 
```
{
    "code":200,
    "data":
    {
        "id": 2,
        "nombre": "Barbie: Escuela de Princesas",
        "director": "Ezekiel Norton",
        "año": 2012,
        "duracion": 81,
        "genero": "Fantasía y familiar"
    }
}
```
**Descripcion:** Eliminar una pelicula
**Metodo HTTP:** DELETE

**URI:** /pelicula/2
**JSON Enviado:**
```
{
    
}
```
**JSON Recibido:** 
```
{
    "code":200,
    "msg":"Pelicula eliminada exitosamente"	
}
```

