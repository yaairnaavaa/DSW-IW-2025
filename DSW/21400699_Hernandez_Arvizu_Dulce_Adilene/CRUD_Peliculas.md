
# CRUD Peliculas 

---

**Crea el Flujo e interacción Cliente-Servidor para un CRUD básico de una tienda de películas:**

## 1. ``Crear una película.``

**Método HTTP:** POST

**URI:** /peliculas

**Json enviado:**

``` bash
{
    "id" : 1,
    "nombre" : El castillo vagabundo,
    "director" : Hayao Miyazaki,
    "año" : 2004,
    "duración" : 1:59,
    "genero" : Infantil/Fantasia
}
```

**Json recibido:**

``` bash
{
    "code": 200,
    "msg": "Pelicula creada exitosamente",
}
```

---

## 2. ``Consulta una película por su id.``

**Método HTTP:** GET

**URI:** /peliculas/6

**Json enviado:**

``` bash
{
     { }
}
```

**Json recibido:**

``` bash
{
    "code": 200,
    "data": {
        "id" : 1,
        "nombre" : El castillo vagabundo,
        "director" : Hayao Miyazaki,
        "año" : 2004,
        "duración" : 1:59,
        "genero" : Infantil/Fantasia }
}
```

---

## 3. ``Actualiza el año, director y duración de una película por su id.``

**Método HTTP:** PUT

**URI:** /peliculas/1

**Json enviado:**

``` bash
{
{
  "director": "H. Miyazaki",
  "año": 2005,
  "duración": "2:00"
}

}
```

**Json recibido:**

``` bash
{
{
  "code": 200,
  "msg": "Película actualizada correctamente"
}
}
```
---

## 4. ``Borra una película por su id.``

**Método HTTP:** DELETE

**URI:** /peliculas/1

**Json enviado:**

``` bash
{
  { }  
}
```

**Json recibido:**

``` bash
{
 
{
  "code": 200,
  "msg": "Película eliminada exitosamente"
}

}
```