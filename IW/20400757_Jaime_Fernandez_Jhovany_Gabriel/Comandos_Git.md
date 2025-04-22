# Comandos Git

# Tipo de enfoque

## Configuración general

| Comando | Descripción del comando | Ejemplo de caso de uso |
| --- | --- | --- |
| `git config --global user.name "Name"` | Configura el nombre de la cuenta en Git. | `git config --global user.name "Juan Pérez"` para establecer tu nombre en todos los repositorios. |
| `git config --global user.email "someone@example.com"` | Configura el correo de la cuenta en Git. | `git config --global user.email "juan@example.com"` para que Git use este correo al hacer commits. |
| `git config --global --list` | Muestra los datos configurados previamente con los comandos anteriores. | Revisar que tu nombre y correo estén bien configurados antes de hacer commits. |

## Interacción repositorio

| Comando | Descripción del comando | Ejemplo de caso de uso |
| --- | --- | --- |
| `git clone "url"` | Clona un repositorio desde la URL dicha. | `git clone https://github.com/usuario/proyecto.git` para obtener una copia local del repositorio. |
| `git branch -a` | Muestra las ramas existentes locales y remotas, colocando con un asterisco la rama actual. | Verificar qué ramas existen y en cuál estás trabajando. |
| `git branch [nombre]` | Añade una nueva rama colocando el nombre. | `git branch nueva-funcionalidad` para empezar a trabajar en una nueva función sin afectar la rama principal. |
| `git checkout [nombre]` | Cambia de rama colocando el nombre. | `git checkout develop` para trabajar en la rama de desarrollo. |
| `git branch -m [viejo] [nuevo]` | Cambia el nombre de la rama objetivo al nuevo valor. | `git branch -m dev desarrollo` para renombrar la rama `dev` a `desarrollo`. |
| `git branch -d [nombre]` | Elimina la rama objetivo. | `git branch -d useless-branch` para borrar una rama que ya no es necesaria o creaste por error. |
| `git merge [rama]` | Mezcla la rama en la que estás con la rama objetivo. | `git merge feature-login` para integrar los cambios de `feature-login` a tu rama actual. |
| `git merge [rama] --no-ff` | Aplica el No Fast Forward, dejando el merge como un commit separado. | `git merge feature-login --no-ff` para mantener un historial de merges más claro. |
| `git rebase [rama]` | Integra los cambios de la rama `rama` en tu rama actual, reescribiendo el historial. | `git rebase main` para aplicar los últimos cambios de `main` sobre tu rama. |
| `git rebase --abort` | Aborta un rebase. | Usar si hay conflictos durante un rebase y deseas cancelarlo. |

## Estados de archivos Git

| Comando | Descripción del comando | Ejemplo de caso de uso |
| --- | --- | --- |
| `git status` | Muestra el estado actual de los archivos y la rama activa. | Comprobar qué archivos han sido modificados antes de hacer un commit. |
| `git add [archivo.txt]` | Añade un archivo en específico o todos con `.` | `git add index.html` o `git add .` para preparar archivos antes de un commit. |
| `git add -A` | Añade todos los cambios (nuevos, eliminados y modificados) al área de preparación. | Actualizar completamente el índice antes de un commit. |
| `git add -u` | Añade solo archivos modificados o eliminados (ya rastreados). | Preparar solo los archivos modificados y eliminados para un commit. |
| `git ls-files` | Muestra los archivos que Git está siguiendo. | Verificar qué archivos están bajo control de versiones. |
| `git reset HEAD [archivo.txt]` | Saca un archivo del área de preparación. | `git reset HEAD index.html` para quitar el archivo del próximo commit. |
| `git checkout -- [archivo.txt]` | Revierte cambios locales a la última versión confirmada. | `git checkout -- style.css` para descartar los cambios hechos en ese archivo. |
| `git help log` | Muestra la ayuda del comando `log` | Entender las opciones disponibles del comando `git log` |
| `git log` | Muestra el historial de commits. | Revisar los últimos cambios en el proyecto. |
| `git log --abbrev-commit` | Muestra los commits con hashes abreviados. | Ver historial de forma más compacta. |
| `git log --oneline --graph --decorate` | Muestra el historial de forma visual y resumida. | Ver el flujo del proyecto con ramas y merges de forma clara. |
| `git rm --cached [archivo.txt]` | Desvincula un archivo del repositorio sin borrarlo localmente. | `git rm --cached config.env` para dejar de seguir un archivo sensible. |
| `git commit -am "Mensaje"` | Añade y confirma todos los archivos rastreados modificados. | `git commit -am "Corrige errores de estilo en CSS"` para hacer un commit rápido. |

## Modificación de archivos

| Comando | Descripción del comando | Ejemplo de caso de uso |
| --- | --- | --- |
| `git mv [archivo] [nuevo]` | Cambia el nombre o mueve un archivo. | `git mv app.js src/app.js` para mover `app.js` a una carpeta llamada `src` |
| `git rm [archivo]` | Elimina el archivo del proyecto (si está rastreado) | `git rm main.css` para borrar el archivo y registrar su eliminación en el próximo commit. |

### Información rescatada de:

Taylor, J. T., & Myers, J. M. (2022, agosto). *Git Complete: the definitive, step-by-step guide to Git*. Udemy. Recuperado 9 de abril de 2025, de [https://www.udemy.com/course/git-complete](https://www.udemy.com/course/git-complete/?couponCode=ST13MT80425G2)
Curso Git comprado con anterioridad debido a una actividad de certificación en la materia Desarrollo de Servicios Web