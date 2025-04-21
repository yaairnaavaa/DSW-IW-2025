# 📘 Comandos Git



---

## 1. `git init`

**Descripción:**  
Inicializa un nuevo repositorio Git en el directorio actual.

**Ejemplo de uso:**  
```bash
git init
```

---

## 2. `git clone`

**Descripción:**  
Clona un repositorio existente desde una URL.

**Ejemplo de uso:**  
```bash
git clone https://github.com/usuario/proyecto.git
```

---

## 3. `git status`

**Descripción:**  
Muestra el estado de los archivos en el directorio de trabajo y el área de preparación (staging).

**Ejemplo de uso:**  
```bash
git status
```

---

## 4. `git add`

**Descripción:**  
Agrega archivos al área de preparación para incluirlos en el próximo commit.

**Ejemplo de uso:**  
```bash
git add archivo.txt
```

---

## 5. `git commit`

**Descripción:**  
Guarda los cambios del área de preparación en el historial del repositorio.

**Ejemplo de uso:**  
```bash
git commit -m "Agrega nueva funcionalidad"
```

---

## 6. `git push`

**Descripción:**  
Envía los commits locales a un repositorio remoto.

**Ejemplo de uso:**  
```bash
git push origin main
```

---

## 7. `git pull`

**Descripción:**  
Obtiene y fusiona los cambios del repositorio remoto al local.

**Ejemplo de uso:**  
```bash
git pull origin main
```

---

## 8. `git branch`

**Descripción:**  
Lista las ramas existentes o crea una nueva rama.

**Ejemplo de uso:**  
```bash
git branch nueva-rama
```

---

## 9. `git checkout`

**Descripción:**  
Cambia a otra rama o restaura archivos.

**Ejemplo de uso:**  
```bash
git checkout nueva-rama
```

---

## 10. `git merge`

**Descripción:**  
Fusiona los cambios de una rama con otra.

**Ejemplo de uso:**  
```bash
git merge nueva-rama
```

---

## 11. `git log`

**Descripción:**  
Muestra el historial de commits del repositorio.

**Ejemplo de uso:**  
```bash
git log
```

---

## 12. `git remote`

**Descripción:**  
Gestiona conexiones a repositorios remotos.

**Ejemplo de uso:**  
```bash
git remote add origin https://github.com/usuario/proyecto.git
```

---

## 13. `git fetch`

**Descripción:**  
Descarga cambios del repositorio remoto sin fusionarlos.

**Ejemplo de uso:**  
```bash
git fetch origin
```

---

## 14. `git diff`

**Descripción:**  
Muestra las diferencias entre los archivos modificados y el último commit.

**Ejemplo de uso:**  
```bash
git diff
```

---

## 15. `git reset`

**Descripción:**  
Deshace cambios en el área de preparación o en commits anteriores.

**Ejemplo de uso:**  
```bash
git reset archivo.txt
```

---

## 16. `git rm`

**Descripción:**  
Elimina archivos del directorio de trabajo y del índice.

**Ejemplo de uso:**  
```bash
git rm archivo.txt
```

---

## 17. `git stash`

**Descripción:**  
Guarda temporalmente los cambios que no están listos para hacer commit.

**Ejemplo de uso:**  
```bash
git stash
```

---

## 18. `git tag`

**Descripción:**  
Crea etiquetas para marcar puntos específicos en la historia del repositorio (como versiones).

**Ejemplo de uso:**  
```bash
git tag v1.0
```

---

## 19. `git config`

**Descripción:**  
Configura opciones y valores para el entorno Git.

**Ejemplo de uso:**  
```bash
git config --global user.name "Tu Nombre"
```

---

## 20. `git revert`

**Descripción:**  
Revierte un commit específico creando un nuevo commit que deshace los cambios.

**Ejemplo de uso:**  
```bash
git revert abc1234
```
