# CRUD de Películas - Flujo Cliente-Servidor

## 1. Crear una película

**Descripción:** Crear una película.

- **Método HTTP:** `POST`  
- **URI:** `/peliculas`  
- **JSON enviado:**

```json
{
  "nombre": "Inception",
  "director": "Christopher Nolan",
  "año": 2010,
  "duración": 148,
  "genero": "Ciencia ficción"
}
```

- **JSON recibido:**

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

---

## 2. Consultar una película por su ID

**Descripción:** Consulta una película por su id.

- **Método HTTP:** `GET`  
- **URI:** `/peliculas/1`  
- **JSON enviado:**

```json
{
}
```

- **JSON recibido:**

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

---

## 3. Actualizar una película por su ID

**Descripción:** Actualiza el año, director y duración de una película por su id.

- **Método HTTP:** `PUT`  
- **URI:** `/peliculas/1`  
- **JSON enviado:**

```json
{
  "año": 2011,
  "director": "C. Nolan",
  "duración": 150
}
```

- **JSON recibido:**

```json
{
  "id": 1,
  "nombre": "Inception",
  "director": "C. Nolan",
  "año": 2011,
  "duración": 150,
  "genero": "Ciencia ficción"
}
```

---

## 4. Borrar una película por su ID

**Descripción:** Borra una película por su id.

- **Método HTTP:** `DELETE`  
- **URI:** `/peliculas/1`  
- **JSON enviado:**

```json
{
}
```

- **JSON recibido:**

```json
{
  "mensaje": "Película con id 1 eliminada correctamente."
}
```

---


