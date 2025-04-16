
# Comandos de Git más utilizados

A continuación se muestran los 20 comandos de Git más usados, incluyendo una breve descripción y un ejemplo de caso de uso para cada uno.

---

## 1. `git init`
**Descripción:** Inicializa un nuevo repositorio Git en el directorio actual.  
**Ejemplo de caso de uso:** Estás comenzando un nuevo proyecto y quieres empezar a usar control de versiones con Git, así que ejecutas `git init` para crear el repositorio.

---

## 2. `git clone`
**Descripción:** Clona un repositorio remoto a tu máquina local.  
**Ejemplo de caso de uso:** Quieres trabajar en un proyecto hospedado en GitHub, por lo que usas `git clone https://github.com/usuario/proyecto.git` para obtener una copia local.

---

## 3. `git status`
**Descripción:** Muestra el estado actual del repositorio, incluyendo archivos modificados o preparados para commit.  
**Ejemplo de caso de uso:** Deseas saber qué archivos has modificado antes de hacer un commit, así que ejecutas `git status`.

---

## 4. `git add`
**Descripción:** Agrega archivos al área de preparación (staging area).  
**Ejemplo de caso de uso:** Has hecho cambios en `main.js` y deseas incluirlo en el próximo commit, así que ejecutas `git add main.js`.

---

## 5. `git commit`
**Descripción:** Registra los cambios agregados en el repositorio con un mensaje.  
**Ejemplo de caso de uso:** Luego de preparar tus archivos, ejecutas `git commit -m "Corrige errores en formulario"` para guardar esos cambios.

---

## 6. `git push`
**Descripción:** Envía los commits locales al repositorio remoto.  
**Ejemplo de caso de uso:** Has hecho cambios en tu rama principal y quieres compartirlos con el equipo, así que ejecutas `git push origin main`.

---

## 7. `git pull`
**Descripción:** Descarga y fusiona cambios desde el repositorio remoto.  
**Ejemplo de caso de uso:** Antes de comenzar a trabajar, ejecutas `git pull origin main` para asegurarte de tener la última versión del código.

---

## 8. `git branch`
**Descripción:** Muestra, crea o elimina ramas en el repositorio.  
**Ejemplo de caso de uso:** Quieres comenzar a trabajar en una nueva funcionalidad sin afectar el código principal, así que ejecutas `git branch nueva-funcionalidad`.

---

## 9. `git checkout`
**Descripción:** Cambia de una rama a otra o restaura archivos.  
**Ejemplo de caso de uso:** Necesitas revisar la rama `desarrollo`, por lo que ejecutas `git checkout desarrollo`.

---

## 10. `git merge`
**Descripción:** Fusiona el historial de otra rama con la rama actual.  
**Ejemplo de caso de uso:** Terminaste una funcionalidad en una rama secundaria y deseas integrarla a `main`, así que ejecutas `git merge nueva-funcionalidad`.

---

## 11. `git log`
**Descripción:** Muestra el historial de commits del repositorio.  
**Ejemplo de caso de uso:** Quieres revisar quién realizó el último cambio en un archivo, así que usas `git log`.

---

## 12. `git reset`
**Descripción:** Revierte cambios en el área de preparación o en los commits.  
**Ejemplo de caso de uso:** Has agregado archivos por error al área de staging, y usas `git reset archivo.txt` para quitarlos.

---

## 13. `git revert`
**Descripción:** Crea un nuevo commit que revierte un commit anterior sin alterar el historial.  
**Ejemplo de caso de uso:** Uno de los commits recientes generó errores, así que ejecutas `git revert 1a2b3c4` para deshacerlo de forma segura.

---

## 14. `git fetch`
**Descripción:** Descarga los cambios desde el repositorio remoto, sin fusionarlos automáticamente.  
**Ejemplo de caso de uso:** Quieres inspeccionar cambios antes de fusionarlos, así que ejecutas `git fetch origin`.

---

## 15. `git remote`
**Descripción:** Administra los repositorios remotos configurados.  
**Ejemplo de caso de uso:** Deseas verificar la URL del repositorio remoto, así que ejecutas `git remote -v`.

---

## 16. `git diff`
**Descripción:** Muestra los cambios entre versiones, ramas o archivos.  
**Ejemplo de caso de uso:** Antes de hacer un commit, usas `git diff` para revisar qué líneas exactas han cambiado.

---

## 17. `git stash`
**Descripción:** Guarda temporalmente los cambios no confirmados.  
**Ejemplo de caso de uso:** Necesitas cambiar de rama rápidamente, pero sin perder tu trabajo actual, así que usas `git stash`.

---

## 18. `git tag`
**Descripción:** Marca puntos específicos en la historia del repositorio como versiones.  
**Ejemplo de caso de uso:** Finalizaste una versión estable y deseas marcarla, así que ejecutas `git tag v1.0`.

---

## 19. `git config`
**Descripción:** Configura parámetros de Git como nombre de usuario y correo electrónico.  
**Ejemplo de caso de uso:** Al instalar Git por primera vez, ejecutas `git config --global user.name "Tu Nombre"` para establecer tu identidad.

---

## 20. `git rm`
**Descripción:** Elimina archivos del repositorio y del sistema de archivos.  
**Ejemplo de caso de uso:** Deseas eliminar un archivo obsoleto del proyecto, así que usas `git rm archivo-viejo.txt`.

---
