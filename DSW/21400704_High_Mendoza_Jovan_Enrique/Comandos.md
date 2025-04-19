
# 📘 Comandos  de Git

---

## 1. `git init`

**Descripción:**  
Inicializa un nuevo repositorio de Git en el directorio actual.

**Uso:**  
```bash
git init
```

**Ejemplo:**  
```bash
mkdir mi-proyecto && cd mi-proyecto
git init
```

---

## 2. `git clone`

**Descripción:**  
Clona un repositorio existente desde una URL.

**Uso:**  
```bash
git clone <url-del-repositorio>
```

**Ejemplo:**  
```bash
git clone https://github.com/usuario/repositorio.git
```

---

## 3. `git status`

**Descripción:**  
Muestra el estado de los archivos en el repositorio.

**Uso:**  
```bash
git status
```

**Ejemplo:**  
```bash
git status
```

---

## 4. `git add`

**Descripción:**  
Agrega archivos al área de preparación (staging area).

**Uso:**  
```bash
git add <archivo>
```

**Ejemplo:**  
```bash
git add index.html
```

---

## 5. `git commit`

**Descripción:**  
Registra los cambios en el repositorio.

**Uso:**  
```bash
git commit -m "mensaje"
```

**Ejemplo:**  
```bash
git commit -m "Agrega archivo index"
```

---

## 6. `git log`

**Descripción:**  
Muestra el historial de confirmaciones (commits).

**Uso:**  
```bash
git log
```

**Ejemplo:**  
```bash
git log
```

---

## 7. `git diff`

**Descripción:**  
Muestra los cambios realizados que no han sido confirmados.

**Uso:**  
```bash
git diff
```

**Ejemplo:**  
```bash
git diff index.html
```

---

## 8. `git branch`

**Descripción:**  
Muestra, crea o elimina ramas.

**Uso:**  
```bash
git branch
```

**Ejemplo:**  
```bash
git branch nueva-rama
```

---

## 9. `git checkout`

**Descripción:**  
Cambia de rama o restaura archivos.

**Uso:**  
```bash
git checkout <rama>
```

**Ejemplo:**  
```bash
git checkout main
```

---

## 10. `git merge`

**Descripción:**  
Fusiona ramas.

**Uso:**  
```bash
git merge <rama>
```

**Ejemplo:**  
```bash
git merge nueva-rama
```

---

## 11. `git remote`

**Descripción:**  
Gestiona conexiones con repositorios remotos.

**Uso:**  
```bash
git remote add origin <url>
```

**Ejemplo:**  
```bash
git remote add origin https://github.com/usuario/repositorio.git
```

---

## 12. `git push`

**Descripción:**  
Envía cambios locales al repositorio remoto.

**Uso:**  
```bash
git push origin <rama>
```

**Ejemplo:**  
```bash
git push origin main
```

---

## 13. `git pull`

**Descripción:**  
Obtiene y fusiona cambios del repositorio remoto.

**Uso:**  
```bash
git pull origin <rama>
```

**Ejemplo:**  
```bash
git pull origin main
```

---

## 14. `git fetch`

**Descripción:**  
Descarga cambios del repositorio remoto sin fusionar.

**Uso:**  
```bash
git fetch
```

**Ejemplo:**  
```bash
git fetch origin
```

---

## 15. `git reset`

**Descripción:**  
Deshace commits o saca archivos del área de preparación.

**Uso:**  
```bash
git reset <archivo>
```

**Ejemplo:**  
```bash
git reset index.html
```

---

## 16. `git rm`

**Descripción:**  
Elimina archivos del repositorio y del sistema de archivos.

**Uso:**  
```bash
git rm <archivo>
```

**Ejemplo:**  
```bash
git rm archivo.txt
```

---

## 17. `git mv`

**Descripción:**  
Mueve o renombra archivos controlados por Git.

**Uso:**  
```bash
git mv archivo1.txt archivo2.txt
```

**Ejemplo:**  
```bash
git mv viejo.html nuevo.html
```

---

## 18. `git config`

**Descripción:**  
Configura opciones de Git (como nombre y correo).

**Uso:**  
```bash
git config --global user.name "Tu Nombre"
```

**Ejemplo:**  
```bash
git config --global user.email "tu@email.com"
```

---

## 19. `git stash`

**Descripción:**  
Guarda cambios temporales sin hacer commit.

**Uso:**  
```bash
git stash
```

**Ejemplo:**  
```bash
git stash save "Trabajo temporal"
```

---

## 20. `git tag`

**Descripción:**  
Crea etiquetas para marcar versiones específicas.

**Uso:**  
```bash
git tag <nombre>
```

**Ejemplo:**  
```bash
git tag v1.0
```
