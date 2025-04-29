
# 🚀 Comandos Básicos de Git

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
mkdir nuevo-proyecto && cd nuevo-proyecto
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

## 4. `git add .`

**Descripción:**  
Agrega todos los archivos modificados al área de preparación (staging area).

**Uso:**  
```bash
git add .
```

**Ejemplo:**  
```bash
git add .
```

---

## 5. `git commit -m`

**Descripción:**  
Registra los cambios en el repositorio con un mensaje.

**Uso:**  
```bash
git commit -m "Mensaje del commit"
```

**Ejemplo:**  
```bash
git commit -m "Añadir nueva funcionalidad de usuario"
```

---

## 6. `git log --oneline`

**Descripción:**  
Muestra el historial de commits de manera compacta, con un solo mensaje por línea.

**Uso:**  
```bash
git log --oneline
```

**Ejemplo:**  
```bash
git log --oneline
```

---

## 7. `git diff`

**Descripción:**  
Muestra los cambios entre el área de preparación y los archivos de trabajo.

**Uso:**  
```bash
git diff
```

**Ejemplo:**  
```bash
git diff index.html
```

---

## 8. `git branch -a`

**Descripción:**  
Lista todas las ramas locales y remotas.

**Uso:**  
```bash
git branch -a
```

**Ejemplo:**  
```bash
git branch -a
```

---

## 9. `git checkout -b`

**Descripción:**  
Crea una nueva rama y cambia a ella.

**Uso:**  
```bash
git checkout -b <nombre-de-rama>
```

**Ejemplo:**  
```bash
git checkout -b nueva-funcionalidad
```

---

## 10. `git merge --no-ff`

**Descripción:**  
Fusiona ramas y garantiza que se cree un commit de merge, incluso si la fusión es lineal.

**Uso:**  
```bash
git merge --no-ff <rama>
```

**Ejemplo:**  
```bash
git merge --no-ff nueva-funcionalidad
```

---

## 11. `git remote -v`

**Descripción:**  
Muestra las URL de los repositorios remotos asociados al proyecto.

**Uso:**  
```bash
git remote -v
```

**Ejemplo:**  
```bash
git remote -v
```

---

## 12. `git push origin --delete`

**Descripción:**  
Elimina una rama remota.

**Uso:**  
```bash
git push origin --delete <nombre-de-rama>
```

**Ejemplo:**  
```bash
git push origin --delete feature-antigua
```

---

## 13. `git pull --rebase`

**Descripción:**  
Obtiene y aplica los cambios remotos sobre la rama local, rebaseando las confirmaciones.

**Uso:**  
```bash
git pull --rebase
```

**Ejemplo:**  
```bash
git pull --rebase origin main
```

---

## 14. `git fetch --all`

**Descripción:**  
Obtiene todos los cambios de todas las ramas remotas sin hacer merge.

**Uso:**  
```bash
git fetch --all
```

**Ejemplo:**  
```bash
git fetch --all
```

---

## 15. `git reset --hard`

**Descripción:**  
Restablece el repositorio a un estado anterior, eliminando los cambios locales.

**Uso:**  
```bash
git reset --hard <commit>
```

**Ejemplo:**  
```bash
git reset --hard HEAD~2
```

---

## 16. `git rm --cached`

**Descripción:**  
Elimina un archivo del área de seguimiento sin eliminarlo del sistema de archivos.

**Uso:**  
```bash
git rm --cached <archivo>
```

**Ejemplo:**  
```bash
git rm --cached archivo.conf
```

---

## 17. `git mv`

**Descripción:**  
Mueve o renombra archivos controlados por Git.

**Uso:**  
```bash
git mv <archivo-antiguo> <archivo-nuevo>
```

**Ejemplo:**  
```bash
git mv archivo1.txt archivo-renombrado.txt
```

---

## 18. `git tag -a`

**Descripción:**  
Crea una etiqueta anotada en un commit específico.

**Uso:**  
```bash
git tag -a <nombre> -m "Mensaje de etiqueta"
```

**Ejemplo:**  
```bash
git tag -a v1.0 -m "Versión inicial"
```

---

## 19. `git cherry-pick`

**Descripción:**  
Aplica un commit específico de otra rama en la rama actual.

**Uso:**  
```bash
git cherry-pick <commit-id>
```

**Ejemplo:**  
```bash
git cherry-pick a1b2c3d4
```

---

## 20. `git rebase -i`

**Descripción:**  
Realiza un rebase interactivo para reorganizar, modificar o combinar commits.

**Uso:**  
```bash
git rebase -i <commit-id>
```

**Ejemplo:**  
```bash
git rebase -i HEAD~3
```

---
