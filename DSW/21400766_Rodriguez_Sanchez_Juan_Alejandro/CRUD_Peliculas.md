# Creación de una película

---

**Metodo HTTP:** POST

**URI:** /movies

**Json enviado:** 
```json
    {
        "id" : 1,
        "nombre" : "Terminator",
        "director" : "Steven Spilberg",
        "año" : 1992,
        "duración" : 2,
        "genero" : "Ciencia Ficción"
    }
```

**Json recibido:**
```json
    {
        "code" : 100,
        "Msj" : "Pelicula añadida"
    }
```

---

# Consulta de una película

---

**Metodo HTTP:** GET

**URI:** /movies/2

**Json enviado:** 
```json
   {

   }
```

**Json recibido:**
```json
    {
        "code" : 200,
        "data" :{
                    "id" : 1,
                    "nombre" : "Terminator",
                    "director" : "Steven Spilberg",
                    "año" : 1992,
                    "duración" : 2,
                    "genero" : "Ciencia Ficción"
                }
    }
```

---

# Consulta de una película

---

**Metodo HTTP:** PUT

**URI:** /movies/3

**Json enviado:** 
```json
    {
        "año" : 1990
    }
```

**Json recibido:**
```json
    {
        "code" : 101,
        "Msj" : "Datos de la Pelicula actualizados"
    }
```

---

# Consulta de una película

---

**Metodo HTTP:** DELETE

**URI:** /movies/2

**Json enviado:** 
```json
    {
   
    }
```

**Json recibido:**
```json
    {
        "code" : 100,
        "Msj" : "Pelicula eliminada"
    }
```

---