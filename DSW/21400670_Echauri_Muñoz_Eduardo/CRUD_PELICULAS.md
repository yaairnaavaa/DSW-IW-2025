# CRUD de Películas - Flujo Cliente-Servidor
## 1 Crear una película

**Método HTTP:** POST  
**URI:** `/peliculas`

**JSON enviado:**

```json
{
    "id": 1,
    "nombre": "Inception",
    "director": "Christopher Nolan",
    "año": 2010,
    "duración": 148,
    "genero": "Ciencia ficción"
}
```

**JSON recibido:**

```json
{
    "code": 200,
    "msg": "Película creada"
}
```

---

## 2 Consultar una película por ID

**Método HTTP:** GET  
**URI:** `/peliculas/1`

**JSON enviado:**

```json
{}
```

**JSON recibido:**

```json
{
    "code": 200,
    "data": {
        "id": 1,
        "nombre": "Inception",
        "director": "Christopher Nolan",
        "año": 2010,
        "duración": 148,
        "genero": "Ciencia ficción"
    }
}
```

---

## 3 Actualizar una película por ID

**Método HTTP:** PUT  
**URI:** `/peliculas/1`

**JSON enviado:**

```json
{
    "año": 2011,
    "director": "C. Nolan",
    "duración": 150
}
```

**JSON recibido:**

```json
{
    "code": 201,
    "msg": "Película actualizada"
}
```

---

## 4 Borrar una película por ID

**Método HTTP:** DELETE  
**URI:** `/peliculas/1`

**JSON enviado:**

```json
{}
```

**JSON recibido:**

```json
{
    "code": 200,
    "msg": "Película eliminada"
}
```