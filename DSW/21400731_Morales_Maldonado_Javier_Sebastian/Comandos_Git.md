# Comandos más utilizados de Git

Morales Maldonado Javier Sebastian - 21400731

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
**Descripción:** Agrega cambios al área de staging (preparación).  
**Ejemplo de caso de uso:** Has terminado de modificar un archivo y quieres prepararlo para commit, por lo que usas `git add archivo.txt`.

---

## 5. `git commit`
**Descripción:** Guarda permanentemente los cambios del área de staging en el historial del repositorio.  
**Ejemplo de caso de uso:** Estás listo para guardar tus cambios con el mensaje "Corrección de errores", así que ejecutas `git commit -m "Corrección de errores"`.

---

## 6. `git push`
**Descripción:** Envía tus commits locales al repositorio remoto.  
**Ejemplo de caso de uso:** Deseas subir tus cambios recientes a GitHub, por lo que usas `git push origin main`.

---

## 7. `git pull`
**Descripción:** Obtiene los últimos cambios del repositorio remoto y los fusiona con tu rama local.  
**Ejemplo de caso de uso:** Antes de empezar a trabajar, quieres asegurarte de tener la versión más reciente del proyecto, así que ejecutas `git pull origin main`.

---

## 8. `git branch`
**Descripción:** Lista, crea o elimina ramas en el repositorio.  
**Ejemplo de caso de uso:** Necesitas crear una nueva rama para desarrollar una característica, por lo que usas `git branch nueva-funcionalidad`.

---

## 9. `git checkout`
**Descripción:** Permite navegar entre ramas o restaurar archivos.  
**Ejemplo de caso de uso:** Quieres cambiar a la rama de desarrollo, así que ejecutas `git checkout desarrollo`.

---

## 10. `git merge`
**Descripción:** Combina los cambios de una rama con la rama actual.  
**Ejemplo de caso de uso:** Has terminado una funcionalidad en tu rama y quieres fusionarla con la rama principal, por lo que usas `git merge mi-funcionalidad`.

---

## 11. `git log`
**Descripción:** Muestra el historial de commits del repositorio.  
**Ejemplo de caso de uso:** Necesitas revisar los cambios recientes en el proyecto, así que ejecutas `git log --oneline` para ver un resumen.

---

## 12. `git diff`
**Descripción:** Muestra las diferencias entre archivos, commits o ramas.  
**Ejemplo de caso de uso:** Quieres ver exactamente qué cambios has hecho en un archivo antes de hacer commit, por lo que usas `git diff archivo.txt`.

---

## 13. `git reset`
**Descripción:** Deshace cambios moviendo el HEAD a un commit específico.  
**Ejemplo de caso de uso:** Te diste cuenta que el último commit fue un error y quieres deshacerlo (manteniendo los cambios), así que ejecutas `git reset --soft HEAD~1`.

---

## 14. `git rm`
**Descripción:** Elimina archivos del repositorio y del sistema de archivos.  
**Ejemplo de caso de uso:** Necesitas eliminar un archivo obsoleto del proyecto, por lo que usas `git rm archivo-viejo.txt`.

---

## 15. `git stash`
**Descripción:** Guarda temporalmente cambios sin hacer commit.  
**Ejemplo de caso de uso:** Tienes cambios sin terminar pero necesitas cambiar de rama urgentemente, así que usas `git stash` para guardarlos temporalmente.

---

## 16. `git tag`
**Descripción:** Crea etiquetas para marcar versiones específicas.  
**Ejemplo de caso de uso:** Has llegado a un hito importante en tu proyecto y quieres marcarlo como versión 1.0, por lo que usas `git tag v1.0`.

---

## 17. `git fetch`
**Descripción:** Descarga cambios del repositorio remoto sin fusionarlos.  
**Ejemplo de caso de uso:** Quieres ver qué cambios hay en el repositorio remoto sin afectar tu trabajo local, así que ejecutas `git fetch origin`.

---

## 18. `git remote`
**Descripción:** Administra las conexiones a repositorios remotos.  
**Ejemplo de caso de uso:** Necesitas agregar un nuevo repositorio remoto, por lo que usas `git remote add upstream URL`.

---

## 19. `git rebase`
**Descripción:** Reaplica commits sobre otra rama base.  
**Ejemplo de caso de uso:** Quieres mantener un historial lineal al integrar tus cambios a la rama principal, así que usas `git rebase main`.

---

## 20. `git config`
**Descripción:** Configura las preferencias de Git.  
**Ejemplo de caso de uso:** Es tu primera vez usando Git y necesitas configurar tu nombre y email, por lo que ejecutas:
```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu@email.com"
```