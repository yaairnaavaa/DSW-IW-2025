# Comandos de GIT

## 1. git init
* **Descripción:** Inicializa un nuevo repositorio de Git en el directorio actual. Crea una subcarpeta .git donde Git guarda el historial y la configuración del repositorio. 
* **Ejemplo:** En la carpeta del proyecto abrir la terminal y ejecutar git init

## 2. git clone \<URL\>
* **Descripción:** Crea una copia local de un repositorio remoto ubicado en la <URL>. Esto descarga todo el historial del repositorio. 
* **Ejemplo:** git clone https://github.com/yaairnaavaa/DSW-IW-2025

## 3. git add <archivo(s)>
* **Descripción:**  Agrega uno o más archivos al área de staging. Esto prepara los cambios en esos archivos para el próximo commit. Puedes usar git add . para agregar todos los cambios en el directorio actual y sus subdirectorios.
* **Ejemplo:** git add mi_archivo.txt o  git add .

## 4. git commit -m "\<mensaje\>"
* **Descripción:** Guarda los cambios realizados en el área de staging en el historial del repositorio local. El mensaje describe los cambios realizados en este commit.
* **Ejemplo:** git commit -m "Descripción del commit"

## 5. git status
* **Descripción:** Muestra el estado del directorio de trabajo y del área de staging. Te informa sobre los archivos modificados, los que están en staging y los que no están rastreados por Git.
* **Ejemplo:** git status

## 6. git log
* **Descripción:** Muestra el historial de commits del repositorio. Puedes ver información como el autor, la fecha y el mensaje de cada commit.
* **Ejemplo:** git log o git log --oneline (Para una vista más compacta)

## 7. git branch
* **Descripción:** Lista todas las ramas (branches) en tu repositorio local. La rama activa actual estará marcada con un asterisco *.
* **Ejemplo:** git branch

## 8. git checkout \<rama\>
* **Descripción:** Cambia a la rama especificada. Esto actualiza los archivos en tu directorio de trabajo para que coincidan con la última instantánea de esa rama
* **Ejemplo:** git checkout main

## 9. git checkout -b <nueva_rama>
* **Descripción:** Crea una nueva rama y cambia a ella al mismo tiempo.
* **Ejemplo:** git checkout -b feature/nueva-funcionalidad.

## 10. git merge \<rama\>
* **Descripción:** Combina los cambios de la <rama> especificada en la rama activa actual. Esto se usa para integrar el trabajo realizado en diferentes ramas. 
* **Ejemplo:** git merge develop (si se esta en la rama main y se quieren combinar los cambios de la rama develop)

## 11. git push \<remoto\> \<rama\>
* **Descripción:** Sube los commits de tu rama local especificada al repositorio remoto.
* **Ejemplo:** git push origin main

## 12. git pull \<remoto\> \<rama\>
* **Descripción:** Descarga los cambios del repositorio remoto y los integra en tu rama local actual. Es una combinación de git fetch (descargar los cambios) y git merge (integrarlos).
* **Ejemplo:** git pull origin main

## 13. git fetch \<remoto\>
* **Descripción:** Descarga los commits y las referencias (como ramas y etiquetas) del repositorio remoto, pero no intenta integrarlos en tus ramas locales. Esto te permite ver los cambios que hay en el remoto antes de decidir si quieres combinarlos. 
* **Ejemplo:** git fetch origin

## 14. git remote -v
* **Descripción:**  Muestra la lista de repositorios remotos configurados para tu repositorio local, junto con sus URLs. La -v (verbose) muestra las URLs para las operaciones de fetch y push.
* **Ejemplo:** git remote -v

## 15. git branch -d \<rama\>
* **Descripción:** Elimina la rama local especificada. Solo puedes eliminar una rama si ya ha sido mergeada en la rama activa actual o si usas -D (forzado). 
* **Ejemplo:** git branch -d feature/vieja

## 16. git reset --hard \<commit\>
* **Descripción:** Restaura tu directorio de trabajo y el área de staging al estado del <commit> especificado, eliminando todos los commits posteriores. Mucho cuidado con este comando que se pueden perder datos.
* **Ejemplo:** git reset --hard HEAD~1 (Vuelve al commit anterior)

## 17. git reset --soft \<commit\>
* **Descripción:** Restaura el HEAD al commit especificado, pero deja los cambios en el área de staging. Esto te permite rehacer el commit pero mantener los cambios para volver a commitarlos.
* **Ejemplo:** git reset --soft HEAD~1

## 18. git stash
* **Descripción:** Guarda temporalmente los cambios sin commitear en un área especial llamada "stash". Esto es útil cuando necesitas cambiar de rama rápidamente sin commitear cambios incompletos.
* **Ejemplo:** git stash

## 19. git stash list
* **Descripción:** Muestra la lista de stashes guardados.
* **Ejemplo:** git stash list

## 20. git stash apply
* **Descripción:** Aplica el stash más reciente (o uno específico si se proporciona su identificador) a el directorio de trabajo. Los cambios se restauran, pero permanecen en el stash. Se usa git stash pop para aplicar y eliminar el stash al mismo tiempo.
* **Ejemplo:** git stash apply o git stash apply stash@{2}