# Actividad

Crea el Flujo e interacción Cliente-Servidor para un CRUD básico de una tienda de películas:

- Crear una película.
- Consulta una película por su id.
- Actualiza el año, director y duración de una película por su id
- Borra una película por su id.

**Estructura cada película:**

```json
{
    "id" : Number,
    "nombre" : String,
    "director" : String,
    "año" : Number,
    "duración" : Number,
    "genero" : String
}
```

**Estructura cada punto:**

## Crear una película

- **Método HTTP**: POST
- **URI**: /movies

**Json enviado**:

```json
{
  "id": 1,
  "nombre": "Inception",
  "director": "Christopher Nolan",
  "año": 2010,
  "duración": 148,
  "genero": "Sci-Fi"
}
```

**Json recibido**:

```json
{
  "code": 200,
  "msg": "Película Creada"
}
```

## Consultar una película por id

- **Método HTTP**: GET
- **URI**: /movies/1

**Json enviado**:

```json
{}
```

**Json recibido**:

```json
{
  "code": 200,
  "data": {
    "id": 1,
    "nombre": "Inception",
    "director": "Christopher Nolan",
    "año": 2010,
    "duración": 148,
    "genero": "Sci-Fi"
  }
}
```

## Actualizar una película por id

- **Método HTTP**: PUT
- **URI**: /movies/1

**Json enviado**:

```json
{
  "año": 2012,
  "director": "Christopher Nolan",
  "duración": 150
}
```

**Json recibido**:

```json
{
  "code": 201,
  "msg": "Película actualizada"
}
```

## Eliminar una película por id

- **Método HTTP**: DELETE
- **URI**: /movies/1

**Json enviado**:

```json
{}
```

**Json recibido**:

```json
{
  "code": 200,
  "msg": "Película eliminada"
}
```
