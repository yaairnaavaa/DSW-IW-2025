# Comandos Git

## 1. `git init`
**Descripción:** Crea un nuevo repositorio Git.
**Ejemplo de uso:** `git init` para inicializar un proyecto nuevo en Git.

## 2. `git clone`
**Descripción:** Crea una copia local de un repositorio remoto.
**Ejemplo de uso:** `git clone https://github.com/user/repo.git` para clonar un repositorio remoto.

## 3. `git add`
**Descripción:** Agrega cambios al área de preparación (staging area) para su posterior commit.
**Ejemplo de uso:** `git add file.txt` para agregar un archivo al staging area.

## 4. `git commit`
**Descripción:** Guarda los cambios en el repositorio local con un mensaje que describe los cambios.
**Ejemplo de uso:** `git commit -m "Agregado archivo de configuración"` para guardar los cambios con un mensaje de descripción.

## 5. `git status`
**Descripción:** Muestra el estado actual del repositorio, incluyendo archivos modificados, archivos en el área de preparación, etc.
**Ejemplo de uso:** `git status` para ver el estado actual del repositorio.

## 6. `git log`
**Descripción:** Muestra el historial de commits del repositorio.
**Ejemplo de uso:** `git log` para ver el historial de commits del repositorio.

## 7. `git branch`
**Descripción:** Muestra, crea o elimina ramas en el repositorio.
**Ejemplo de uso:** `git branch nueva-rama` para crear una nueva rama.

## 8. `git checkout`
**Descripción:** Cambia de una rama a otra o restaura archivos.
**Ejemplo de uso:** `git checkout master` para cambiar a la rama principal.

## 9. `git merge`
**Descripción:** Fusiona el historial de otra rama con la rama actual.
**Ejemplo de uso:** `git merge nueva-rama` para fusionar la rama nueva-rama con la rama actual.

## 10. `git remote`
**Descripción:** Administra los repositorios remotos configurados.
**Ejemplo de uso:** `git remote -v` para ver la lista de repositorios remotos configurados.

## 11. `git fetch`
**Descripción:** Descarga los cambios desde el repositorio remoto, sin fusionarlos automáticamente.
**Ejemplo de uso:** `git fetch origin` para descargar los cambios desde el repositorio remoto origin.

## 12. `git pull`
**Descripción:** Descarga y fusiona los cambios desde el repositorio remoto.
**Ejemplo de uso:** `git pull origin master` para descargar y fusionar los cambios desde el repositorio remoto origin y la rama master.

## 13. `git push`
**Descripción:** Envía los commits locales al repositorio remoto.
**Ejemplo de uso:** `git push origin master` para enviar los commits locales a la rama master del repositorio remoto origin.

## 14. `git reset`
**Descripción:** Revierte cambios en el área de preparación o en los commits.
**Ejemplo de uso:** `git reset --hard` para revertir todos los cambios en el área de preparación y en los commits.

## 15. `git revert`
**Descripción:** Crea un nuevo commit que revierte un commit anterior sin alterar el historial.
**Ejemplo de uso:** `git revert HEAD~1` para revertir el commit anterior.

## 16. `git clean`
**Descripción:** Elimina archivos y directorios no rastreados por Git.
**Ejemplo de uso:** `git clean -f` para eliminar archivos y directorios no rastreados por Git.

## 17. `git tag`
**Descripción:** Crea, lista o elimina etiquetas en el repositorio.
**Ejemplo de uso:** `git tag v1.0.0` para crear una etiqueta con el nombre v1.0.0.

## 18. `git diff`
**Descripción:** Muestra los cambios entre versiones, ramas o archivos.
**Ejemplo de uso:** `git diff master..nueva-rama` para ver los cambios entre la rama master y la rama nueva-rama.

## 19. `git stash`
**Descripción:** Guarda temporalmente los cambios no confirmados.
**Ejemplo de uso:** `git stash` para guardar los cambios no confirmados.

## 20. `git show`
**Descripción:** Muestra la información de un commit o un objeto Git.
**Ejemplo de uso:** `git show HEAD` para ver la información del commit actual.
