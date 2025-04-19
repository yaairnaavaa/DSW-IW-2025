# Comandos Básicos de Git

---

## 1. `git clone <url>`
**Descripción**: Crea una copia local de un repositorio remoto, incluyendo todo el historial y las ramas. Se usa para empezar a trabajar con un proyecto existente.  
**Ejemplo**:
```bash
git clone https://github.com/usuario/repo.git  # Clona un repositorio usando protocolo HTTPS
git clone git@github.com:usuario/repo.git     # Clona usando SSH (más seguro)
git clone --branch main repo.git              # Clona solo una rama específica (más rápido)
```
**Ejemplo de caso de uso**:  
Una nueva colaboradora desea contribuir a un proyecto de código abierto. Usa `git clone` para obtener una copia del repositorio y empezar a trabajar en su propia rama.

## 2. `git init`
**Descripción**: Inicializa un repositorio Git en el directorio actual. Ideal para nuevos proyectos.  
**Ejemplo**:
```bash
git init              # Crea un repositorio estándar
git init --bare       # Crea un repositorio bare (para servidores)
```
**Ejemplo de caso de uso**:  
Has comenzado a trabajar en un nuevo proyecto personal. Ejecutas `git init` para empezar a rastrear cambios desde el inicio.

## 3. `git add <archivo>`
**Descripción**: Añade cambios del directorio de trabajo al área de preparación para el próximo commit.  
**Ejemplo**:
```bash
git add archivo.txt          # Añade un archivo específico al staging
git add .                    # Añade todos los archivos modificados y nuevos
git add -p                   # Modo interactivo para seleccionar cambios parciales
```
**Ejemplo de caso de uso**:  
Después de modificar varios archivos, usas `git add -p` para revisar y añadir solo partes específicas de los cambios antes de hacer commit.

## 4. `git commit`
**Descripción**: Crea un nuevo commit con los cambios del área de preparación.  
**Ejemplo**:
```bash
git commit -m "Estructura del desarrollo"
git commit -am "Actualización de estilos"
git commit --amend
```
**Ejemplo de caso de uso**:  
Después de añadir cambios, ejecutas `git commit -m "Agrega validación de formularios"` para documentar el propósito de esos cambios.

## 5. `git status`
**Descripción**: Muestra el estado actual del repositorio: archivos modificados, preparados o sin seguimiento.  
**Ejemplo**:
```bash
git status
git status -s
```
**Ejemplo de caso de uso**:  
Antes de hacer commit, revisas el estado del proyecto con `git status` para asegurarte de no olvidar ningún archivo.

## 6. `git push`
**Descripción**: Sube los commits locales al repositorio remoto.  
**Ejemplo**:
```bash
git push origin main
git push -u origin feature
git push --force-with-lease
```
**Ejemplo de caso de uso**:  
Has terminado una funcionalidad nueva y haces `git push origin feature/nueva-interfaz` para compartir tu trabajo con el equipo.

## 7. `git pull`
**Descripción**: Descarga y fusiona los últimos cambios del repositorio remoto.  
**Ejemplo**:
```bash
git pull origin main
git pull --rebase origin main
```
**Ejemplo de caso de uso**:  
Al empezar el día, ejecutas `git pull` para asegurarte de estar trabajando con la versión más reciente del proyecto.

## 8. `git branch`
**Descripción**: Gestiona ramas en el repositorio (crear, listar o eliminar).  
**Ejemplo**:
```bash
git branch
git branch -a
git branch -d ramitax
```
**Ejemplo de caso de uso**:  
Estás por comenzar una nueva característica, así que ejecutas `git branch nueva-funcionalidad` para trabajar sin afectar el código principal.

## 9. `git checkout`
**Descripción**: Cambia entre ramas, crea nuevas ramas o restaura archivos a estados anteriores.  
**Ejemplo**:
```bash
git checkout develop
git checkout -b nuevaRama
git checkout HEAD~2 -- doc.txt
```
**Ejemplo de caso de uso**:  
Quieres revisar una versión anterior de un archivo, por lo que ejecutas `git checkout HEAD~1 -- config.json`.

## 10. `git merge`
**Descripción**: Fusiona los cambios de una rama con la rama actual.  
**Ejemplo**:
```bash
git merge main/login
git merge --no-ff release
git merge --abort
```
**Ejemplo de caso de uso**:  
Después de que un compañero termina su trabajo en una rama, ejecutas `git merge` para integrarlo a la rama principal.

## 11. `git log`
**Descripción**: Muestra el historial de commits del repositorio.  
**Ejemplo**:
```bash
git log
git log --oneline --graph
git log -p
```
**Ejemplo de caso de uso**:  
Necesitas identificar qué commit introdujo un bug, así que revisas el historial con `git log`.

## 12. `git diff`
**Descripción**: Muestra diferencias entre el directorio de trabajo, el área de preparación y commits.  
**Ejemplo**:
```bash
git diff
git diff --cached
git diff main..feature
```
**Ejemplo de caso de uso**:  
Antes de hacer commit, ejecutas `git diff` para revisar los cambios exactos línea por línea.

## 13. `git reset`
**Descripción**: Revierte el repositorio a un estado anterior según el modo (soft, mixed, hard).  
**Ejemplo**:
```bash
git reset --soft HEAD~1
git reset --mixed HEAD~1
git reset --hard HEAD~1
```
**Ejemplo de caso de uso**:  
Cometiste un error en el último commit. Usas `git reset --soft HEAD~1` para corregirlo manteniendo los cambios en staging.

## 14. `git stash`
**Descripción**: Guarda temporalmente cambios sin comprometerlos.  
**Ejemplo**:
```bash
git stash
git stash list
git stash pop
```
**Ejemplo de caso de uso**:  
Tienes trabajo sin terminar, pero necesitas cambiar de rama urgentemente. Guardas tus cambios con `git stash`.

## 15. `git remote`
**Descripción**: Administra conexiones con repositorios remotos.  
**Ejemplo**:
```bash
git remote -v
git remote add upstream URL
git remote rename origin primary
```
**Ejemplo de caso de uso**:  
Al trabajar en un fork de un proyecto, añades el repositorio original como `upstream` para poder sincronizarlo.

## 16. `git fetch`
**Descripción**: Descarga cambios del repositorio remoto sin fusionarlos.  
**Ejemplo**:
```bash
git fetch origin
git fetch --prune
git fetch --all
```
**Ejemplo de caso de uso**:  
Quieres ver si hay ramas nuevas en el remoto antes de hacer pull, así que usas `git fetch`.

## 17. `git rebase`
**Descripción**: Reorganiza commits sobre otra base para mantener un historial limpio.  
**Ejemplo**:
```bash
git rebase main
git rebase -i HEAD~3
git rebase --abort
```
**Ejemplo de caso de uso**:  
Reordenas y renombras tus últimos commits antes de compartir la rama con el equipo, usando `git rebase -i`.

## 18. `git tag`
**Descripción**: Crea marcadores específicos en el historial, normalmente para versiones.  
**Ejemplo**:
```bash
git tag v1.0.0
git tag -a v1.1.0 -m "Release estable"
git tag -d v0.9
```
**Ejemplo de caso de uso**:  
Antes de lanzar una nueva versión del software, etiquetas el último commit con `git tag v2.0.0`.

## 19. `git config`
**Descripción**: Ajusta opciones de configuración locales o globales del entorno Git.  
**Ejemplo**:
```bash
git config --global user.name "Monita"
git config --global core.editor "code --wait"
git config --list
```
**Ejemplo de caso de uso**:  
Cambias tu nombre de usuario global para que aparezca correctamente en todos tus commits futuros.

## 20. `git restore`
**Descripción**: Restaura archivos al estado de un commit anterior, útil para deshacer cambios.  
**Ejemplo**:
```bash
git restore doc.txt
git restore --staged doc.txt
git restore --source=HEAD~2 doc.txt
```
**Ejemplo de caso de uso**:  
Has hecho cambios indeseados en un archivo. Usas `git restore doc.txt` para dejarlo como estaba antes.
